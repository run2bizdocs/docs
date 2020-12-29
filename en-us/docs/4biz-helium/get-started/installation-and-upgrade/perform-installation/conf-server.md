Title: Configuring the application server

# Configuring the application server

Application server settings can be done in two ways: via jboss-cli or by editing the xml file. 
There is no technical difference in any of the options, and the choice is up to each 
administrator. Below are both configuration examples.

!!! Warning "ATTENTION"

    Pay attention to the variables to change them according with your environment settings.

## Configuring server via jboss-cli

Connect to the jboss-cli (assuming the server is running) by executing the command below:

``` shell
[root@server /tmp]# /opt/wildfly/bin/jboss-cli.sh --connect
[standalone@localhost:9990 /]
```

Then run the following commands replacing the variable contents with your environment setting.

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

After the settings, to exit the CLI, type `quit`

``` shell
[standalone@localhost:9990 /] quit
[root@server /tmp]#
```
## Configuring the server via XML

To edit the XML file used by the wildfly access the directory:

``` shell
[root@server /tmp]# /opt/wildfly/standalone/configuration
```
Edit the standalone-full.xml file and include the 4biz logo XML configuration right after the clause below:

``` xml
<server xmlns="urn:jboss:domain:6.0">
    <extensions>
        <extension module="org.jboss.as.clustering.infinispan"/>
        <extension module="org.jboss.as.connector"/>
		...
</extensions>
```

 After the configuration tag close </extensions> include the parameters below:

 ``` xml
 <system-properties>
     <property name="mongodb.host" value="citmongo"/>
     <property name="mongodb.port" value="27017"/>
     <property name="mongodb.user" value="admin"/>
     <property name="mongodb.password" value="admin"/>
     <property name="4biz.protocol" value="http"/>
     <property name="4biz.host" value="my.4bizcloud.com"/>
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

 After configuring, restart the service to implement the changes:

 ``` shell
 [root@server /tmp]# systemctl status wildfly
 ```
 
## Configuring Firebase

1. The following file has the function of allowing the application to communicate with the application with messaging via Push whenever a new ticket is created, suspended, reactivated, reclassified and closed;  

2. For that, it must be placed in one of the Citsmart repository folders;  

3. After uploading the package, save the path to use it as instructed in: Configuring the application server.

## Next step

[Configuring the Datasource and Drives of base][1]

[1]:/en-us/4biz-helium/get-started/installation-and-upgrade/perform-installation/conf-datasource-and-db.html
