Title: Realizando o deploy do 4biz

# Realizando o deploy do 4biz

Faça o download do pacote WAR do 4biz e do Builder no portal do parceiro. Envie para o servidor utilizando scp para pasta /tmp. A instalação do 4biz consiste nos seguintes passsos:

1. Fazer o deploy do pacote 4biz Tracker
2. Fazer o deploy do pacote Builder
3. Realizar a configuração inicial do 4biz Tracker

Descomprima o pacote do 4biz Tracker caso esrteja no formato .zip:

``` shell
[root@server /tmp]# unzip 4bizITSM-Enterprise-8.0.2.0.war.zip
```

Copie para o servidor de aplicação na pasta `standalone/deployments`:

``` shell
[root@server /tmp]# cp 4bizITSM-Enterprise-8.0.2.0.war /opt/wildfly/standalone/deployments/
```
Observe o log `/opt/wildfly/standalone/log/server.log` com a opção `tail -f` até que a mensagem abaixo apareça:

``` shell
2019-11-14 17:20:37,731 INFO  [org.jboss.as.server] (DeploymentScanner-threads - 1) WFLYSRV0010: Deployed "4bizITSM-Enterprise-8.0.2.0.war" (runtime-name : "4bizITSM-Enterprise-8.0.2.0.war")
```

A mensagem acima confirma que o deploy foi realizado. O mesmo se aplica ao pacote do Builder. Copie o builder para pasta `standalone/deployments`:

``` shell
[root@server /tmp]# cp 4biz-builder-web-1.3.2.1.war /opt/wildfly/standalone/deployments/
```

Observe o log `/opt/wildfly/standalone/log/server.log` com a opção `tail -f` até que a mensagem abaixo apareça:

``` shell
2019-11-14 17:37:43,647 INFO  [org.jboss.as.server] (DeploymentScanner-threads - 2) WFLYSRV0010: Deployed "4biz-builder-web-1.3.2.1.war" (runtime-name : "4biz-builder-web-1.3.2.1.war")
```

## Acessando o 4biz pela primeira vez

Após a realização do deploy, acesse o 4biz através do URL: se foi configurado um domínio, acesse pelo caminho https://DOMINIO/4biz, caso tenha feito a configuração via IP, acesse https://ENDERECO_IP/4biz.

!!! info "Navegadores Suportados"
    Para o bom funcionamento do sistema, você deverá utilizar as seguintes versões mínimas dos principais browsers: **Microsoft EDGE** (Edge 42.17134.0 / Microsoft EdgeHTML 17.17134 ou superior); **Google Chrome** (versão versão 76.0.3809.132 ou superior); **Mozila Firefox** (versão 69.0 ou superior).

## Próximo passo

[Finalizar instalação][1]

[1]:/pt-br/4biz-helium/get-started/installation-and-upgrade/perform-installation/setup-4biz.html
