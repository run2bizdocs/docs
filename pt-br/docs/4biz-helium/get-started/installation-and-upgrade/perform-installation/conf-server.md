Title: Configurando o servidor de aplicação

# Configurando o servidor de aplicação

As configurações do servidor de aplicação podem ser feitas de duas formas: via jboss-cli ou editando o arquivo xml. Não existe diferença técnica em nenhuma das opções, e a escolha vai de cada administrador. Abaixo ambos exemplos de configuração.

!!! Warning "ATENÇÃO"

    Fique atento às variáveis para alterá-las de acordo com as configurações do seu ambiente.

## Configurando servidor via jboss-cli

Conecte-se ao jboss-cli (considerando-se que o servidor esteja rodando) executando o comando abaixo:

``` shell
/opt/wildfly/bin/jboss-cli.sh --connect
```

Em seguida execute os seguintes comandos substituindo o conteúdo das variáveis pela configuração do seu ambiente. Você deverá ter como resposta `{"outcome" => "success"}`

``` shell
/system-property=mongodb.host:add(value="127.0.0.1")

/system-property=mongodb.port:add(value="27017")

/system-property=mongodb.user:add(value="admin")

/system-property=mongodb.password:add(value="admin")

/system-property=citsmart.protocol:add(value="http")

/system-property=citsmart.host:add(value="my.cloud4biz.com")

/system-property=citsmart.port:add(value="8080")

/system-property=citsmart.context:add(value="4biz")

/system-property=citsmart.login:add(value="4biz.local\\\consultor")

/system-property=citsmart.password:add(value="senhaConsultor")

/system-property=citsmart.inventory.id:add(value="inventory")

/system-property=citsmart.evm.id:add(value="evm")

/system-property=citsmart.evm.enable:add(value=true)

/system-property=citsmart.inventory.enable:add(value=true)

/system-property=citsmart.port.updateparameters:add(value="9000")

/system-property=citsmart.inventory.pagelength:add(value="100")

/system-property=rhino.scripts.directory:add(value="")

/system-property=jboss.as.management.blocking.timeout:add(value="600")

/system-property=org.quartz.properties:add(value="$\{jboss.server.config.dir\}/quartz.properties")

/system-property=snmp.oid.repository.directory:add(value="/opt/templates")
```

Após as configurações, para sair do CLI digite `quit`

``` shell
[standalone@localhost:9990 /] quit
[root@server /tmp]#
```
## Configurando o servidor via XML

Para editar o arquivo XML utilizado pelo wildfly na mão, entre no diretório:

``` shell
cd /opt/wildfly/standalone/configuration
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

No arquivo standalone nos atributos: `<system-properties>` incluir uma nova linha e preencher conforme o exemplo:

 ``` xml
 <system-properties>
     <property name="mongodb.host" value="127.0.0.1"/>
     <property name="mongodb.port" value="27017"/>
     <property name="mongodb.user" value="admin"/>
     <property name="mongodb.password" value="admin"/>
     <property name="citsmart.protocol" value="http"/>
     <property name="citsmart.host" value="my.cloud4biz.com"/>
     <property name="citsmart.port" value="8080"/>
     <property name="citsmart.context" value="4biz"/>
     <property name="citsmart.login" value="4biz.local\\\consultor"/>
     <property name="citsmart.password" value="senhaConsultor"/>
     <property name="citsmart.inventory.id" value="inventory"/>
     <property name="citsmart.evm.id" value="evm"/>
     <property name="citsmart.evm.enable" value="false"/>
     <property name="citsmart.inventory.enable" value="false"/>
     <property name="rhino.scripts.directory" value=""/>
     <property name="jboss.as.management.blocking.timeout" value="600"/>
     <property name="citsmart.port.updateparameters" value="9000"/>
     <property name="citsmart.inventory.pagelength" value="100"/>
     <property name="org.quartz.properties" value="${jboss.server.config.dir}/quartz.properties"/>
     <property name="snmp.oid.repository.directory" value="/opt/templates"/>
 </system-properties>
 ```

 Após realizada as configurações, reinicie o serviço para efetivar as mudanças:

``` shell
systemctl restart wildfly
```

## Configurando Firebase

1. O arquivo a seguir tem a função de permitir a comunicação da aplicação com o aplicativo com mensageria via Push sempre que um novo ticket for criado, suspenso, reativo, reclassificado ou encerrado;  

2. Para isso deverá ser colocado em uma das pastas do repositório do 4biz.  

3. Após subir o pacote salve o caminho para utilizá-lo conforme orientado em: Configurando o servidor de aplicação

## Configuração de Mensagem

1. As configurações do servidor de aplicação podem ser feitas de duas formas: via jboss-cli ou editando o arquivo xml. Não existe diferença técnica em nenhuma das opções, e a escolha vai de cada administrador.

2. Conecte-se ao jboss-cli (considerando-se que o servidor esteja rodando) executando o comando a seguir:

	1. Onde no arquivo standalone em <jms-queue> incluir uma nova linha:

	``` xml
	<jms-queue name="advancedSearch" entries="queue/advancedSearch 	    java:jboss/exported/jms/queue/queue/advancedSearch"/>
      Preencher conforme o exemplo:
      <!-- restante do código omitido -->
      <subsystem xmlns="urn:jboss:domain:messaging-activemq:3.0">
            <server name="default">
                  <!-- restante do código omitido -->
    <jms-queue name="advancedSearch"   
         entries="queue/advancedSearch   
         java:jboss/exported/jms/queue/queue/advancedSearch" />
                                               <!-- restante do código omitido -->
            </server>
      </subsystem>
      <!-- restante do código omitido -->
      ```

## Próximo passo

[Configurando o Datasource e Drives de banco][1]

[1]:/pt-br/4biz-helium/get-started/installation-and-upgrade/perform-installation/conf-datasource-and-db.html
