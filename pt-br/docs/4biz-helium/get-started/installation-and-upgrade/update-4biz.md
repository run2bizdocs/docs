Title: Atualização do 4biz on-premisses

# Atualização do 4biz/builder

Este procedimento tem por objetivo demonstrar o passo-a-passo da atualização do produto 4biz/Builder em servidores de aplicação Wildfly.

Para efeito desde documento, iremos utilizar como exemplo o seguinte cenário:

Atualizar o 4biz da versão `4biz-Helium-1.0.0.war.zip` para a versão `4biz-Helium-1.0.1.war.zip` e builder da versão `4biz-builder-1.3.5.0.war.zip` para `4biz-builder-1.3.5.1.war.zip`. Note que você não precisa realizar o deploy de todos os pacotes de uma vez, você poderá atualizar apenas um dos componentes. De toda forma, verifique a versão correta do(s) pacote(s) em seu servidor e use os comandos abaixo apontando para as respectivas versões.

## Pré-requisito

- [X] Ter instalado o servidor de aplicação Wildfly com base no documento [Instalação on-premisses][1].

- [X] Ter realizado o download dos pacotes ***4biz-Helium-1.0.1.war.zip*** e builder ***4biz-builder-1.3.5.1.war.zip*** diretamente do portal do parceiro.

## Procedimento

**1 - Pare o serviço do Wildfly**

```sh
systemctl stop wildfly
```

Verifique se algum serviço Java está em execução;

```sh
ps aux | grep java
```

**2 - Copie e extraia o(s) arquivo(s) baixado(s)**

Transfira os novos pacotes via sftp o diretório `tmp` do seu servidor Linux. Logo após realize a extração:

```sh
unzip 4biz-Helium-1.0.1.war.zip
```
O arquivo extraído estará neste formato:

```sh
[root@server]# 4biz-Helium-1.0.1.war
```

**3 - Remova o(s) deploy(s) antigo(s)**

Acesse o diretório de deploys do Wildfly

```sh
cd /opt/wildfly/standalone/deployments
```

Remova o(s) pacote(s) que sera(m) substituído(s)

```sh
rm -Rf 4biz-Helium-1.0.0.war*
```

```sh
rm -Rf 4biz-builder-1.3.5.0.war*
```

!!! warning "ATENÇÃO"
    Note que tanto o pacote do produto quanto o arquivo ".deployed" precisam ser removidos. Caso você esteja realizando o deploy de apenas um componente, remova apenas o arquivo do item relacionado. Se você quiser realizar o deploy novamente na mesma versão, remova apenas o arquivo ".deployed" - essa opção pode ser feita também à quente.

**4 - Remova os diretórios temporários**

```sh
rm -Rf data tmp log
```

**5 - Crie os diretórios temporários novamente**

```sh
mkdir {data, tmp, log}
```

Atribua a permissão de dono ao usuário `wildlfy`

```sh
chown -R wildfly:wildfly data tmp log
```
**6 - Remova caches e limpe a memória Swap (opcional)**

É recomendado realizar a limpeza de caches e memória Swap

 - **Limpar memória Swap**

```sh
swapoff -a
```

- **Limpar Caches**

```sh
sysctl vm.drop_caches=1
```

```sh
sysctl vm.drop_caches=3
```

**7 - Copie o(s) novo(s) pacote(s) WAR para o diretório Deployments**

```sh
cp 4biz-Helium-1.0.1.war /opt/wildfly/standalone/deployments/
```

```sh
cp 4biz-builder-1.3.5.1.war /opt/wildfly/standalone/deployments/
```

**8 - Inicie o serviço do Wildfly**

```sh
systemctl start wildfly
```

**9 - Acompanhe o processo de deploy**

```sh
tail -f /opt/wildfly/standalone/log/server.log
```

## Conclusão

Após seguir este procedimento acreditamos que você implantou com sucesso a última versão do produto.


[1]:https://docs.run2biz.com/pt-br/4biz-helium/get-started/installation-and-upgrade/overview.html
