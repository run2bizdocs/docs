Title: Realizando o deploy do 4biz

# Realizando o deploy do 4biz

Faça o download do pacote WAR do 4biz e do Neuro no portal do parceiro. Envie para o servidor utilizando scp para pasta /tmp. A instalação do 4biz consiste nos seguintes passsos:

1. Fazer o deploy do pacote 4biz Workflow
2. Fazer o deploy do pacote Builder
3. Realizar a configuração inicial do 4biz Workflow

Descomprima o pacote do 4biz Workflow caso esrteja no formato .zip:

``` shell
unzip 4biz-Helium-BETA-01.war.zip
```

Copie para o servidor de aplicação na pasta `standalone/deployments`:

``` shell
cp 4biz-Helium-BETA-01.war /opt/wildfly/standalone/deployments/
```
Observe o log `/opt/wildfly/standalone/log/server.log` com a opção `tail -f` até que a mensagem abaixo apareça:

``` shell
2019-11-14 17:20:37,731 INFO  [org.jboss.as.server] (DeploymentScanner-threads - 1) WFLYSRV0010: Deployed "4biz-Helium-BETA-01.war" (runtime-name : "4biz-Helium-BETA-01.war")
```

A mensagem acima confirma que o deploy foi realizado. O mesmo se aplica ao pacote do Builder. Copie o neuro para pasta `standalone/deployments`:

``` shell
cp citsmart-neuro-web-1.3.4.1.war /opt/wildfly/standalone/deployments/
```

Observe o log `/opt/wildfly/standalone/log/server.log` com a opção `tail -f` até que a mensagem abaixo apareça:

``` shell
2019-11-14 17:37:43,647 INFO  [org.jboss.as.server] (DeploymentScanner-threads - 2) WFLYSRV0010: Deployed "citsmart-neuro-web-1.3.4.1.war" (runtime-name : "citsmart-neuro-web-1.3.4.1.war")
```

## Acessando o 4biz pela primeira vez

Após a realização do deploy, acesse o 4biz através do URL: se foi configurado um domínio, acesse pelo caminho https://DOMINIO:PORTA/4biz, caso tenha feito a configuração via IP, acesse https://ENDERECO_IP:PORTA/4biz.

Exemplo:

```sh
http://192.168.0.40:8080/4biz
```
ou

```sh
https://192.168.0.40:8443/4biz
```

!!! info "Navegadores Suportados"
    Para o bom funcionamento do sistema, você deverá utilizar as seguintes versões mínimas dos principais browsers: **Microsoft EDGE** (Edge 42.17134.0 / Microsoft EdgeHTML 17.17134 ou superior); **Google Chrome** (versão versão 76.0.3809.132 ou superior); **Mozila Firefox** (versão 69.0 ou superior).

## Próximo passo

[Finalizar instalação][1]

[1]:/pt-br/4biz-helium/get-started/installation-and-upgrade/perform-installation/setup-4biz.html
