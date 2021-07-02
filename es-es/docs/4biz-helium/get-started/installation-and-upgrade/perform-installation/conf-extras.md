Title: Configuraciones extras de 4biz

# Configuraciones extras de 4biz

A partir de la versión Helium 1.2.24, se insertaron nuevos parámetros:
 
- Parámetro: AUTHENTICATION_PROTOCOL
- Ojetivo: Definir o protocolo de autenticação
- Comportamiento: Define si el sistema se autenticará con parámetros internos o con otro protocolo de autenticación.
- Tipo: varchar
- Valor default: internal
- Tipos válidos: 

	1.	OAUTH2: Para la autenticación de keycloack: esta información sobrescribe cualquier política de seguridad ingresada en el registro de Política de seguridad;
	2.	Internal: Para autenticación definida por el sistema;
 
- Parámetro: AUTHENTICATION_CREATE_USER
- Ojetivo: Defina si el usuario se creará en la aplicación después de iniciar sesión
- Comportamiento: Registra el usuario que inició sesión en la aplicación;
- Tipo: boleano (true or false)
- Valor default: FALSE 
- Valores posibles:
	
	True – grabar
	False -–  no grabar


A partir de la versión Helium 1.2.23, se insertaron nuevos parámetros:
 
- Parámetro: MAXIMUM_LOGIN_FIELD_SIZE
- Ojetivo: Establezca el tamaño máximo aceptable en el campo de inicio de sesión
- Comportamiento: Simplemente evita el inicio de sesión emitiendo un mensaje genérico, inicio de sesión o contraseña no válidos.
- Tipo: numérico
- Valor default: 25
 
- Parámetro: ALLOW_SYMBOLS_AT_LOGIN
- Ojetivo: Defina si el sistema acepta símbolos en el campo de inicio de sesión
- Comportamiento: Simplemente evita el inicio de sesión emitiendo un mensaje genérico, inicio de sesión o contraseña no válidos.
- Tipo: boleano (true or false)
- Valor default: FALSE

Desde la versión Helium 1.2.19, el archivo CITSMART.CFG pasa a llamarse "application.ini" y debe seguir las siguientes pautas:  

1. La actualización de la tabla solo ocurrirá cuando el parámetro LOAD_FACTSERVICEREQUESTRULES de APPLICATION.INI tenga el valor TRUE. En ausencia de esta configuración en el archivo, el sistema asume el valor FALSE para el parámetro. Es decir, el valor predeterminado es NO actualizar la tabla;  
2. Si hay una programación relacionada con una regla de escalamiento de tickets y el parámetro LOAD_FACTSERVICEREQUESTRULES tiene el valor FALSE, el sistema emite la alerta en el LOG: El sistema no puede comenzar a procesar las reglas de escalamiento porque la propiedad LOAD_FACTSERVICEREQUESTRULES (archivo de configuración) es igual a FALSE;  
3. NUEVOS PARÁMETROS PARA APLICACIÓN.INI: Para activar updateParameters, opción para sincronizar los valores de los parámetros en la memoria, en un ambiente agrupado; debemos agregar en el archivo application.ini la siguiente configuración: UPDATEPARAMETERS_PORT =<número de puerto a utilizar> ejemplo: UPDATEPARAMETERS_PORT=2002.

Cree un archivo llamado application.ini en /opt/wildfly/standalone/configuration/ con la información a continuación:

``` shell
RECORDS_LIMIT_TO_GENERATE_REPORT_IN_THE_BACKGROUND = 500
START_MONITORA_INCIDENTES=FALSE
JDBC_ALIAS_REPORTS=
JDBC_ALIAS_BPM=
JDBC_ALIAS_BPM_EVENTOS=
START_VERIFICA_EVENTOS=FALSE
QUANTIDADE_BACKUPLOGDADOS=1000
START_MODE_RULES=FALSE
START_MODE_RULES=FALSE
LOAD_FACTSERVICEREQUESTRULES=TRUE
INICIAR_PROCESSAMENTOS_BATCH=TRUE
```

Dar permiso de usuario wildfly para este archivo:

``` shell
[root@server /tmp]# chown wildfly.wildfly /opt/wildfly/standalone/configuration/application.ini
```

!!! note

	En el archivo application.ini, el valor predeterminado es TRUE (incluso si no está configurado),es decir, si esta opción no existe en el archivo, el sistema usará el valor TRUE para esta propiedad. Establecido en TRUE, habilita el Thread que actualiza la tabla de hechos de solicitud de servicio al inicio del sistema. Establecido en FALSE, la actualización ocurrirá solo después de agregar o cambiar la solicitud de servicio.


## Configuración de Quartz

El procesamiento Batch de 4biz utiliza Quartz para programar y procesar rutinas del sistema. Cree un archivo llamado "quartz.properties" en la ruta `/opt/wildfly/standalone/configuration/`. Las configuraciones difieren para la standalone común, para la standalone configurada en modo de clúster. En cualquier caso, configure wildfly de las siguientes maneras.

### Configuración standalone sin cluster

Si está ejecutando el wildfly en modo standalone, pero sin configuración de clúster, ingrese la siguiente información en el archivo quarts.properties:

``` shell
#===============================================================
#Configure Main Scheduler Properties
#===============================================================
org.quartz.scheduler.instanceName = CitSmartMonitor
org.quartz.scheduler.instanceId = AUTO
#===============================================================
#Configure ThreadPool
#===============================================================
org.quartz.threadPool.threadCount =  5
org.quartz.threadPool.threadPriority = 5
org.quartz.threadPool.class = org.quartz.simpl.SimpleThreadPool
#===============================================================
#Configure JobStore
#===============================================================
org.quartz.jobStore.class = org.quartz.simpl.RAMJobStore
```

### Configuración standalone con cluster configurado

Si tiene una standalone funcionando en modo de clúster, la configuración de quartz varía según la base de datos utilizada. A continuación se encuentran las configuraciones para cada uno de los escenarios posibles. Cualquiera que sea la base de datos, la configuración se aplica al mismo archivo quartz.properties en la misma ruta que ingresó anteriormente.

Configuración de la base de datos Postgres

``` shell
#============================================================================
# Configure Main Scheduler Properties
#============================================================================
org.quartz.scheduler.instanceName = CitSmartMonitor
org.quartz.scheduler.instanceId = AUTO
#============================================================================
# Configure ThreadPool
#============================================================================
org.quartz.threadPool.class = org.quartz.simpl.SimpleThreadPool
org.quartz.threadPool.threadCount = 25
org.quartz.threadPool.threadPriority = 5
#============================================================================
# Configure JobStore
#============================================================================
org.quartz.jobStore.misfireThreshold = 60000
org.quartz.jobStore.class = org.quartz.impl.jdbcjobstore.JobStoreTX
org.quartz.jobStore.driverDelegateClass = org.quartz.impl.jdbcjobstore.PostgreSQLDelegate
org.quartz.jobStore.useProperties = true
org.quartz.jobStore.dataSource = citsmart
org.quartz.jobStore.tablePrefix = QRTZ_
org.quartz.jobStore.isClustered = true
org.quartz.jobStore.clusterCheckinInterval = 20000
org.quartz.dataSource.citsmart.jndiURL= java:/jdbc/citsmart
```

Configuración para la base de datos de Microsoft SQL Server

``` shell
#============================================================================
# Configure Main Scheduler Properties
#============================================================================
org.quartz.scheduler.instanceName = CitSmartMonitor
org.quartz.scheduler.instanceId = AUTO
#============================================================================
# Configure ThreadPool
#============================================================================
org.quartz.threadPool.class = org.quartz.simpl.SimpleThreadPool
org.quartz.threadPool.threadCount = 25
org.quartz.threadPool.threadPriority = 5
#============================================================================
# Configure JobStore
#============================================================================
org.quartz.jobStore.misfireThreshold = 60000
org.quartz.jobStore.class = org.quartz.impl.jdbcjobstore.JobStoreTX
org.quartz.jobStore.driverDelegateClass = org.quartz.impl.jdbcjobstore.MSSQLDelegate
org.quartz.jobStore.useProperties = true
org.quartz.jobStore.dataSource = citsmart
org.quartz.jobStore.tablePrefix = QRTZ_
org.quartz.jobStore.isClustered = true
org.quartz.jobStore.clusterCheckinInterval = 20000
org.quartz.dataSource.citsmart.jndiURL= java:/jdbc/citsmart
```

Configuración para la base de datos Oracle

``` shell
#============================================================================
# Configure Main Scheduler Properties
#============================================================================
org.quartz.scheduler.instanceName = CitSmartMonitor
org.quartz.scheduler.instanceId = AUTO
#============================================================================
# Configure ThreadPool
#============================================================================
org.quartz.threadPool.class = org.quartz.simpl.SimpleThreadPool
org.quartz.threadPool.threadCount = 25
org.quartz.threadPool.threadPriority = 5
#============================================================================
# Configure JobStore
#============================================================================
org.quartz.jobStore.misfireThreshold = 60000
org.quartz.jobStore.class = org.quartz.impl.jdbcjobstore.JobStoreTX
org.quartz.jobStore.driverDelegateClass = org.quartz.impl.jdbcjobstore.oracle.OracleDelegate
org.quartz.jobStore.useProperties = true
org.quartz.jobStore.dataSource = citsmart
org.quartz.jobStore.tablePrefix = QRTZ_
org.quartz.jobStore.isClustered = true
org.quartz.jobStore.clusterCheckinInterval = 20000
```

## Creando directorios para la instalación

Cree todos los directorios a continuación necesarios para el funcionamiento de la solución. Recuerde que el propietario de los directorios debe ser el usuario wildfly.

``` shell

[root@server /tmp]# mkdir -p /opt/citsmart/{ged,kb,twinwords,attachkb,upload}
[root@server /tmp]# chown -R wildfly.wildfly /opt/citsmart/

```

## Próximo paso

[Instalando certificado SSL][1]

[1]:/es-es/4biz-helium/get-started/installation-and-upgrade/perform-installation/install-certificate.html
