Title: Configurando o Datasource e Drives de banco

# Configurando o Datasource e Drives de banco

Antes de criar um datasource, é necessário adicionar um módulo de um banco de dados ao sistema. Cada banco tem seu próprio driver de conexão, mas as configurações de todos partem do mesmo princípio: fazer o download do driver do fabricante, copiá-lo para o wildfly, configurar no sistema. As configurações serão feitas via jboss-cli, mas todas elas podem ser feitas também via XML no arquivo standalone-full.xml caso deseje.

No exemplo abaixo usaremos o driver do PostgreSQL. Cada banco de dados possui seu próprio método de configuração, recomendamos procurar na documentação do fabricante do banco de dados de sua escolha caso seja diferente de nossa documentação.

O download do driver JDBC do PostgreSQL pode ser encontrado no endereço https://jdbc.postgresql.org no link downloads. A versão do driver utilizado pela 4biz é a 4.1 build 9.3 Build 1104.

```sh
[root@server /tmp]# wget https://jdbc.postgresql.org/download/postgresql-9.3-1104.jdbc41.jar
```

Acesse novamente o jboss-cli para adicionar o driver com comando abaixo (considerando que você tenha feito o download para pasta `/tmp`):

```sh
[standalone@localhost:9990 /] module add --name=org.postgres --resources=/tmp/postgresql-9.3-1104.jdbc41.jar --dependencies=javax.api,javax.transaction.api
```

Com esse comando, o driver será adicionado automaticamente a pasta `/opt/wildfly-12.0.0.Final/modules/org/postgres/main/`

Continue no CLI e execute o comando abaixo para incluir um datasource:

```sh
[standalone@localhost:9990 /] /subsystem=datasources/jdbc-driver=postgres:add(driver-name="postgres",driver-module-name="org.postgres",driver-xa-datasource-class-name=org.postgresql.xa.PGXADataSource
```

## Criando o banco de dados do 4biz

Independente da arquitetura do banco (se instalado no nesmo servidor ou separado) os passos abaixo servem para se criar um banco de dados e um usuário para o 4biz. No procedimento partimos do pressuposto que você tenha acesso ao SGBD. Acesse o PostgreSQL com comando abaixo:

```sh
[root@server /tmp]#  su - postgres
bash-4.2$
bash-4.2$ psql
psql (9.6.15)
Type "help" for help.

postgres=#
```
Crie um usuário e senha para acesso ao banco do 4biz (substitua a SUA_SENHA com uma senha de preferência):

```sh
postgres=# create user 4bizdbuser with password 'SUA_SENHA';
CREATE ROLE
postgres=#
```
Crie um banco de dados para o 4biz:

```sh
postgres=# create database 4biz_db with owner 4bizdbuser encoding 'UTF8' tablespace pg_default;
CREATE DATABASE
postgres=#
```
Dê permissão para o usuário do 4biz:

```sh
postgres=# alter role 4bizdbuser superuser;
ALTER ROLE
postgres=#
```

Saia do PSQL e do shell do usuário postgres:

```sh
postgres=# \q
bash-4.2$ exit
exit
[root@server /tmp]#
```
Caso o banco esteja rodando no mesmo servidor, é necessário liberar a conexão para o usuário do 4biz. Edite o arquivo  `/var/lib/pgsql/9.6/data/pg_hba.conf` e inclua a seguinte linha:

```sh
# Database administrative login by Unix domain socket
local   all             postgres                                ident
```
!!! Warning "ATENÇÃO"

    Não altere a linha `local  all postgres  peer` que vem por padrão, inclua a linha acima logo abaixo desta.


Se o banco de dados estiver rodando em outro servidor é necessário liberar a conexão a partir do Wildfly. Para isso inclua a seguinte linha no mesmo arquivo pg_hba.conf, substituindo o pelo endereço de IP do servidor wildfly:

```sh
host 4biz_db 4bizdbuser WILDFLY_IP_ADDRESS/32 md5

```

## Configurando o datasource para o 4biz

Existem oito entradas de datasource para o 4biz_db, sendo que quatro são para o 4biz e quatro para o 4biz Builder. O usuário e senha é 4bizdbuser e SUA_SENHA criados no passo anterior. Caso tenha criado usuário, senha e banco de nomes diferentes, altere nos comandos abaixo.

Conecte no jboss-cli e execute os seguintes comandos:

### Datasource 4biz

```sh
/subsystem=datasources/data-source="/jdbc/4biz":add(jndi-name="java:/jdbc/4biz",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=blocking-timeout-wait-millis,value=60000)
/subsystem=datasources/data-source="/jdbc/4biz":write-attribute(name=idle-timeout-minutes,value=5)
```

### Datasource 4bizFlow

```sh
/subsystem=datasources/data-source="/jdbc/4bizFluxo":add(jndi-name="java:/jdbc/4bizFluxo",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=blocking-timeout-wait-millis,value=60000)
/subsystem=datasources/data-source="/jdbc/4bizFluxo":write-attribute(name=idle-timeout-minutes,value=5)
```

### Datasourece 4biz_reports

```sh
/subsystem=datasources/data-source="/jdbc/4biz_reports":add(jndi-name="java:/jdbc/4biz_reports",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=blocking-timeout-wait-millis,value=60000)
/subsystem=datasources/data-source="/jdbc/4biz_reports":write-attribute(name=idle-timeout-minutes,value=5)
```

### Datasource 4bizBpmEventos

```sh
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":add(jndi-name="java:/jdbc/4bizBpmEventos",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=blocking-timeout-wait-millis,value=60000)
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":write-attribute(name=idle-timeout-minutes,value=5
```

### Datasource 4biz-builder

```sh
/subsystem=datasources/data-source="/env/jdbc/4biz-builder":add(jndi-name="java:/env/jdbc/4biz-builder",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=blocking-timeout-wait-millis,value=60000)#
```

### Datasource 4biz-builder-app1

```sh
/subsystem=datasources/data-source="/env/jdbc/4biz-builder-app1":add(jndi-name="java:/env/jdbc/4biz-builder-app1",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=blocking-timeout-wait-millis,value=60000)
```

### Datasource 4biz-builder-app2

```sh
/subsystem=datasources/data-source="/env/jdbc/4biz-builder-app2":add(jndi-name="java:/env/jdbc/4biz-builder-app2",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=blocking-timeout-wait-millis,value=60000)
```
### Datasource 4biz-builder-app3

```sh
/subsystem=datasources/data-source="/env/jdbc/4biz-builder-app3":add(jndi-name="java:/env/jdbc/4biz-builder-app3",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.4biz.com:5432/4biz_db",user-name="4bizdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=min-pool-size,value=10)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=max-pool-size,value=300)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=pool-prefill,value=true)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
/subsystem=datasources/data-source="/env\/jdbc\/4biz-builder":write-attribute(name=blocking-timeout-wait-millis,value=60000)
```

Antes de sair do jboss-cli, execute o comando reload para aplicar as alterações e faça um teste de conexão com a base de dados:

```sh
[standalone@localhost:9990 /]: reload
```
E faça um teste de conexão com todos os bancos com os comandos abaixo. Lembrando que o resultado precisa ser `"outcome" => "success"`:

``` sh
/subsystem=datasources/data-source="/jdbc/4biz":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4bizFluxo":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4biz_reports":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4bizBpmEventos":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4biz-builder":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4biz-builder-app1":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4biz-builder-app2":test-connection-in-pool
/subsystem=datasources/data-source="/jdbc/4biz-builder-app3":test-connection-in-pool
```

## Próximo passo

[Configurando o Wildfly][1]

[1]:/pt-br/4biz-helium/get-started/installation-and-upgrade/perform-installation/conf-wildfly.html
