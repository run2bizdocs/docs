Title: Configuring Datasource and Drives of bank

Configuring Datasource and Drives of bank
===========================================

Before creating a datasource, it's necessary to add a database module to the system. Each base 
has its own connection driver, but all settings are based on the same principle: download the 
driver from the manufacturer, copy it to wildfly and configure on the system. The settings will 
be made via jboss-cli, but they can all be made via XML in the standalone-full.xml file if you 
wish for it.

In the example below we'll use the PostgreSQL driver. Each database has its own configuration 
method, we recommend looking in the database manufacturer's documentation of your choice if it 
differs from our documentation.

The PostgreSQL JDBC driver download can be found at https://jdbc.postgresql.org at the downloads 
link. The driver version used by 4biz is 4.1 build 9.3 Build 1104.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
[root@server /tmp]# wget https://jdbc.postgresql.org/download/postgresql-9.3-1104.jdbc41.jar
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Access jboss-cli again to add the driver with the command below
(considering you have downloaded it to folder `/tmp`):

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
[standalone@localhost:9990 /] module add --name=org.postgres --resources=/tmp/postgresql-9.3-1104.jdbc41.jar --dependencies=javax.api,javax.transaction.api
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

With this command, the driver will be automatically added to the folder
`/opt/wildfly-12.0.0.Final/modules/org/postgres/main/`

Continue to the CLI and run the command below to add a datasource:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
[standalone@localhost:9990 /] /subsystem=datasources/jdbc-driver=postgres:add(driver-name="postgres",driver-module-name="org.postgres",driver-xa-datasource-class-name=org.postgresql.xa.PGXADataSource
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creating the 4biz database
------------------------------------

Regardless of the database architecture (whether installed on the same server or separately) the 
steps below are for creating a database and user for 4biz. In the procedure we assume that 
you have access to the DBMS. Access PostgreSQL with the command below:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
[root@server /tmp]#  su - postgres
bash-4.2$
bash-4.2$ psql
psql (9.6.15)
Type "help" for help.

postgres=#
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Create a password and user to get access to the 4biz base (replace YOUR_PASSWORD with a 
preferred password):

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
postgres=# create user 4bizdbuser with password 'YOUR_PASSWORD';
CREATE ROLE
postgres=#
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Create a database to the 4biz:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
postgres=# create database 4biz_db with owner 4bizdbuser encoding 'UTF8' tablespace pg_default;
CREATE DATABASE
postgres=#
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Give permission to the 4biz user:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
postgres=# alter role 4bizdbuser superuser;
ALTER ROLE
postgres=#
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Leave the PSQL and shell of the postgres user:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
postgres=# \q
bash-4.2$ exit
exit
[root@server /tmp]#
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If the base is running on the same server, it's necessary to release the connection to the 
4biz user. Edit the file
`/var/lib/pgsql/9.6/data/pg_hba.conf` and include the following line:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# Database administrative login by Unix domain socket
local   all             postgres                                ident
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

!!! Warning "ATTENTION"

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do not change the `local all postgres peer` line that comes by default, include the line above 
just below this one.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If the database is running on another server, it's necessary to release the connection from the 
Wildfly. To do this, add the following line in the same pg_hba.conf file, replacing it with the 
Wildfly server IP address:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
host 4biz_db 4bizdbuser WILDFLY_IP_ADDRESS/32 md5
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Configuring the datasource to 4biz
-----------------------------------------

There are eight datasource entries for 4biz_db, four for 4biz and four for 4biz 
Builder. The user and password is 4bizdbuser and YOUR_PASSWORD created in the previous step. 
If you have created a different user, password, and database, change it in the commands below.

Conect in the jboss-cli and run the following commands:

### Datasource 4biz

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/subsystem=datasources/data-source="/jdbc/4biz":add(jndi-name="java:/jdbc/4biz",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=blocking-timeout-wait-millis,value=60000)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=idle-timeout-minutes,value=5)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

### Datasource 4bizFlow

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/subsystem=datasources/data-source="/jdbc/4bizFluxo":add(jndi-name="java:/jdbc/4bizFluxo",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=blocking-timeout-wait-millis,value=60000)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=idle-timeout-minutes,value=5)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

### Datasourece 4biz_reports

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/subsystem=datasources/data-source="/jdbc/4biz_reports":add(jndi-name="java:/jdbc/4biz_reports",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=blocking-timeout-wait-millis,value=60000)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=idle-timeout-minutes,value=5)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

### Datasource 4bizBpmEventos

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":add(jndi-name="java:/jdbc/4bizBpmEventos",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=blocking-timeout-wait-millis,value=60000)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=idle-timeout-minutes,value=5
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

### Datasource 4biz-builder

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/subsystem=datasources/data-source="/env/jdbc/4biz-builder":add(jndi-name="java:/env/jdbc/4biz-builder",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=blocking-timeout-wait-millis,value=60000)#
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

### Datasource 4biz-builder-app1

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/subsystem=datasources/data-source="/env/jdbc/4biz-builder-app1":add(jndi-name="java:/env/jdbc/4biz-builder-app1",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=blocking-timeout-wait-millis,value=60000)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

### Datasource 4biz-builder-app2

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/subsystem=datasources/data-source="/env/jdbc/4biz-builder-app2":add(jndi-name="java:/env/jdbc/4biz-builder-app2",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=blocking-timeout-wait-millis,value=60000)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

### Datasource 4biz-builder-app3

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/subsystem=datasources/data-source="/env/jdbc/4biz-builder-app3":add(jndi-name="java:/env/jdbc/4biz-builder-app3",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=blocking-timeout-wait-millis,value=60000)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Before leaving the jboss-cli, run the reload command to apply the changes and test the database 
connection:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
[standalone@localhost:9990 /]: reload
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

And make a connection test with all bases with the commands below. Remember that
the result has to be `"outcome" => "success"`:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/subsystem=datasources/data-source="/jdbc/4biz":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4bizFluxo":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4biz_reports":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4biz-builder":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4biz-builder-app1":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4biz-builder-app2":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4biz-builder-app3":test-connection-in-pool
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Next step
-------------

[Configuring the
Wildfly](/en-us/4biz-helium/get-started/installation-and-upgrade/perform-installation/conf-wildfly.html)
