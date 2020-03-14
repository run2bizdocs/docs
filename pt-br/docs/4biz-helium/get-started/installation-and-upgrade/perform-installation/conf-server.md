Title: Configurando o servidor de aplicação

# Configurando o servidor de aplicação

As configurações do servidor de aplicação podem ser feitas de duas formas: via jboss-cli ou editando o arquivo xml. Não existe diferença técnica em nenhuma das opções, e a escolha vai de cada administrador. Abaixo ambos exemplos de configuração.

!!! Warning "ATENÇÃO"

    Fique atento às variáveis para alterá-las de acordo com as configurações do seu ambiente.

## Configurando servidor via jboss-cli

Conecte-se ao jboss-cli (considerando-se que o servidor esteja rodando) executando o comando abaixo:

``` shell
[root@server /tmp]# /opt/wildfly/bin/jboss-cli.sh --connect
[standalone@localhost:9990 /]
```

Em seguida execute os seguintes comandos substituindo o conteúdo das variáveis pela configuração do seu ambiente.

``` shell
[standalone@localhost:9990 /] /system-property=mongodb.host:add(value="citmongo")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=mongodb.port:add(value="27017")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=mongodb.user:add(value="admin")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=mongodb.password:add(value="admin")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.protocol:add(value="http")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.host:add(value="my.4biz.com")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.port:add(value="8080")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.context:add(value="4biz")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.login:add(value="4biz.local\\\consultor")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.password:add(value="senhaConsultor")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.inventory.id:add(value="4bizinventory")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.evm.id:add(value="4bizevm")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.evm.enable:add(value=true)
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.inventory.enable:add(value=true)
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.port.updateparameters:add(value="9000")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=4biz.inventory.pagelength:add(value="100")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=rhino.scripts.directory:add(value="")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=jboss.as.management.blocking.timeout:add(value="600")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=org.quartz.properties:add(value="$\{jboss.server.config.dir\}/quartz.properties")
{"outcome" => "success"}
[standalone@localhost:9990 /]/system-property=snmp.oid.repository.directory:add(value="/opt/templates")
{"outcome" => "success"}
```

Após as configurações, para sair do CLI digite `quit`

``` shell
[standalone@localhost:9990 /] quit
[root@server /tmp]#
```
## Configurando o servidor via XML

Para editar o arquivo XML utilizado pelo wildfly na mão, entre no diretório:

``` shell
[root@server /tmp]# /opt/wildfly/standalone/configuration
```
E edite o arquivo stantalone-full.xml e inclua a configuração XML do 4biz logo após a clausula abaixo:

``` xml
<server xmlns="urn:jboss:domain:6.0">
    <extensions>
        <extension module="org.jboss.as.clustering.infinispan"/>
        <extension module="org.jboss.as.connector"/>
		...
</extensions>
```

 Após o fechamento da configuração `</extensions>` inclua o trecho a seguir:

 ``` xml
 <system-properties>
     <property name="mongodb.host" value="citmongo"/>
     <property name="mongodb.port" value="27017"/>
     <property name="mongodb.user" value="admin"/>
     <property name="mongodb.password" value="admin"/>
     <property name="4biz.protocol" value="http"/>
     <property name="4biz.host" value="my.cloud4biz.com"/>
     <property name="4biz.port" value="8080"/>
     <property name="4biz.context" value="4biz"/>
     <property name="4biz.login" value="4biz.local\\\consultor"/>
     <property name="4biz.password" value="senhaConsultor"/>
     <property name="4biz.inventory.id" value="4bizinventory"/>
     <property name="4biz.evm.id" value="4bizevm"/>
     <property name="4biz.evm.enable" value="false"/>
     <property name="4biz.inventory.enable" value="false"/>
     <property name="rhino.scripts.directory" value=""/>
     <property name="jboss.as.management.blocking.timeout" value="600"/>
     <property name="4biz.port.updateparameters" value="9000"/>
     <property name="4biz.inventory.pagelength" value="100"/>
     <property name="org.quartz.properties" value="${jboss.server.config.dir}/quartz.properties"/>
     <property name="snmp.oid.repository.directory" value="/opt/templates"/>
 </system-properties>
 ```

 Após realizada as configurações, reinicie o serviço para efetivar as mudanças:

 ``` shell
 [root@server /tmp]# systemctl status wildfly
 ```

## Próximo passo

[Configurando o Datasource e Drives de banco][1]

[1]:/pt-br/4biz-helium/get-started/installation-and-upgrade/perform-installation/conf-datasource-and-db.html
