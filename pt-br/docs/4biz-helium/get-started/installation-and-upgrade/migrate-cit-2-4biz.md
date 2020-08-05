Title: Migrar CITSmart para 4biz - On-premises

#  Migrar CITSmart para 4biz - On-premises

Cenário: O cliente possui uma instalação on-premises do CITSmart e deseja migrar seu ambiente para o produto 4biz. Para isso, as seguintes alterações precisam ser realizadas:

**- Servidor de Aplicação (Wildfly)**

- Alterar configurações de Subsystems no Wildfly para correto redirecionamento.

**- Aplicação (Citsmart/4biz)**

- Execução de scripts SQL para alterar o contexto "/citsmart" para "/4biz"


## Antes de Começar

- [X] Realizar backup do servidor (Wildfly) e dump da base de dados;

- [X] Baixar pacote 4biz e fazer upload para o servidor (Wildfly)

## Procedimento

### Servidor de aplicação Wildfly

**- Remover configurações antigas e criar novas configurações:**

1 - Acessar o servidor via SSH;

2 - Acessar o o Jboss CLI;

```sh
/opt/wildfly/bin/jboss-cli.sh --connect
```
3 - Remove configurações de datasource do Citsmart;

```sh
/subsystem=undertow/configuration=filter/rewrite=citsmart:remove
```

```sh
/subsystem=undertow/server=default-server/host=default-host/filter-ref=citsmart:remove
```
4 - Criar configurações para o produto 4biz;

```sh
/subsystem=undertow/configuration=filter/rewrite=4biz:add(target="/4biz")
```

```sh
/subsystem=undertow/server=default-server/host=default-host/filter-ref=4biz:add(predicate="regex('\^/?\$') and equals(/4biz)")

```
Reiniciar servidor de aplicação;

```sh
reload
```

5 - Realizar atualização da versão com base no [documento de atualização][1]

### Execução de scripts SQL para alterar o contexto

[1]:https://infra.run2biz.com/app/update-cit-4biz.html
