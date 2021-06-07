Title: Configuración del Entorno de Desarrollo de 4biz en Linux

Description: Cómo realizar la configuración del entorno 4biz usando SO Ubuntu.

# Configuración del Entorno de Desarrollo de 4biz en Linux

La configuración del producto 4biz con OS Linux es posible. En este documento se mostrará detalladamente el paso a paso de este proceso, desde la instalación de Ubuntu y todas las aplicaciones necesarias hasta el proceso de integración propiamente dicho.


## Antes de empezar  

Para comenzar el procedimiento, se requiere descargar los archivos disponibles en Google Drive https://drive.google.com/drive/folders/1k6f6NtvoAiTwDzQ6trNYHHWo3PSBh0zD  
Debe usar las credenciales de Office 365 de 4biz para acceder a los archivos. A lo largo del procedimiento, también deberás tener acceso al GIT con las credenciales de Central IT. Si no lo tienes, pídeselo a tu gestor.

## Procedimiento  

### Instalación de OS Ubuntu en la máquina

 - Acceda a la página web https://ubuntu.com/#download para descargar Ubuntu. 
Haga clic en el primer botón para descargar la versión de escritorio de Ubuntu. Recuerde utilizar siempre la versión más reciente. 
  
 - Después de descargar el archivo .iso, se requiere descargar Rufus a través del enlace https://rufus.ie/es/ para configurar una unidad USB bootable (o de arranque).  
  
 - Además de Rufus y del archivo .iso de Ubuntu, para crear una unidad USB de arranque, también es necesario tener una unidad flash con un mínimo de 4 gb de almacenamiento.
  
  
**Para configurar la unidad, siga el procedimiento a continuación:**  
  
  
 - Ejecute Rufus.  
 
 - Inserte la unidad en la máquina.
 
 - Rufus actualizará para configurar el dispositivo dentro del campo _Dispositivo_ o _Device_.
 
 - Seleccione la unidad deseada entre las opciones.  
       
!!! note "Nota"  

         Para evitar la elección de un dispositivo incorrecto, asegúrese de que solo hay un dispositivo insertado en la máquina
         
   
 - Después de seleccionar el dispositivo, elija la opción de arranque. Las opciones serán _No arrancable_ y _FreeDOS_. Ya que está creando un dispositivo Ubuntu de arranque, seleccione _FreeDOS_.
 
 - Deje las opciones para _Esquema de partición (MBR)_ y _Sistema de destino (BIOS (o UEFI-CSM))_ como predeterminado. 

 - Haga clic en el botón _SELECT_ junto a la opción _Boot Selection_, busque el archivo .iso de Ubuntu y haga clic en Abrir.  
 
 - El campo _VOLUME LABEL_ se actualizará para reflejar el ISO seleccionado.
 
 - Los otros parámetros deben ser dejados en sus valores predeterminados.  
 
 - Haga clic en _START_ para iniciar el proceso de grabación.  
 
 - Durante el proceso, puede aparecer un mensaje que advierte que Rufus requiere archivos adicionales para completar la grabación de ISO. Seleccione Sí para continuar.  
 
 - Durante el proceso, se le avisará que Rufus ha detectado que el ISO de Ubuntu es una imagen _ISOHybrid_. Mantenga la grabación en el modo de imagen ISO seleccionado y haga clic en OK para continuar.  
 
 - Rufus también le advertirá de que todos los datos del dispositivo USB seleccionado están a punto de ser destruidos. Compruebe si ha seleccionado el dispositivo correcto antes de hacer clic en OK.  
 
 - Espere a que se complete el proceso, que puede tardar unos minutos dependiendo de su máquina. Después de completar, haga clic en _CLOSE_ para cerrar Rufus.  
       
 - Inserte la unidad con ISO en su computadora y reinicie la máquina. La mayoría de las computadoras reconocerán automáticamente la unidad de arranque y mostrarán un mensaje de bienvenida con opciones para seleccionar el idioma, instalar o probar Ubuntu Desktop.  
   
!!! note "Nota"    

    Si la computadora no arranca automáticamente desde la unidad USB, intente mantener pulsado F12 o Delete cuando la computadora se inicie por primera vez. En la mayoría de las máquinas, esto le permitirá seleccionar el dispositivo USB en un menú de inicio específico del sistema. Si no sucede, compruebe la opción de arranque (de boot) en la computadora, seleccionándolo a través de la unidad USB. Si no está seguro, busque un breve mensaje cuando se inicie el sistema, esto generalmente le indicará qué tecla debe pulsarse para abrir el menú de inicio
          
 - Poco después de elegir el idioma, se le pedirá que seleccione el diseño del teclado. Si el instalador no adivina el diseño predeterminado correctamente, utilice el botón _'Detectar diseño del teclado'_ para realizar un breve procedimiento de configuración.  

 - Después de seleccionar Continuar, se le preguntará qué aplicaciones desea instalar para comenzar. Las dos opciones son _'Instalación normal'_ y _'Instalación mínima'_, seleccione la opción _'Instalación normal'_.

 - Debajo de la cuestión del tipo de instalación, hay dos casillas de verificación; una para habilitar actualizaciones durante la instalación y otra para habilitar software de terceros.  
  
 - Habilite la opción _Download updates_ y _Install third-party software._ 
   
 - Para el siguiente paso, se requiere estar conectado a Internet. Si no está conectado a Internet, se le pedirá que seleccione una red inalámbrica, si está disponible. Le recomendamos que se conecte durante la instalación para asegurarse de que su máquina esté actualizada.  

 - Las demás opciones de instalación serán de _Ubicación_ y _detalles de Login

 - Después de que todo esté instalado y configurado, aparecerá una pequeña ventana que le pedirá que reinicie su máquina. Haga clic en _Restart Now_ y retire la unidad flash USB cuando se le solicite.

!!! note "Consejo"  

      Si lo necesita, puede encontrar una lista de atajos de teclado para Ubuntu en el enlace https://pt.wikibooks.org/wiki/Manual_do_Ubuntu/Teclas_de_atalho  

### Instalación de Java

 - Accede al terminal de Ubuntu presionando Ctrl+Alt+T e introduzca la siguiente secuencia:  

<i>sudo add-apt-repository ppa:openjdk-r/ppa  

sudo apt-get update  

sudo apt-get install openjdk-8-jdk</i>              

 - Busque el archivo .bashrc en la carpeta Home y después, pulse Ctrl+H añadiendo al final de él, las dos líneas de abajo para las variables de entorno **JAVA_HOME** y **PATH**:

<i>export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64  

export PATH=$PATH:$JAVA_HOME/bin </i>  

 - Ejecute los siguientes comandos en el terminal:  

<i>source ~/.bashrc  

echo $JAVA_HOME  

echo $PATH  </i>

 - Debería aparecer una pantalla de resultados con los directorios de JAVA_HOME y PATH: 

 - Acceda al Terminal en Ubuntu e introduzca como se indica a continuación para confirmar la instalación:  

<i>java -version 

javac -version </i>

!!! note "Consejo"  

      Puede limpiar la pantalla del terminal presionando Ctrl+L  


### Autenticación del acceso en Artifactory

 - Acceda al siguiente enlace para la autenticación de sus datos de acceso a la red _(Active Directory)_: 

https://artifactory.centralit.com.br:8092/artifactory/webapp/login.html?0  

 - Introduzca sus datos, y después de la autenticación, vaya a la parte superior derecha de la pantalla y haga clic en su nombre de usuario. 
 
 - Introduzca su contraseña de red y haga clic en _"Unlock"_.  
 
 - Copie el fragmento que contiene el nombre de usuario y la contraseña y reemplácelo en _settings.xml_ exactamente en las mismas posiciones previamente indicadas.  

!!! note "Nota" 

      El archivo settings.xml se encuentra dentro de la carpeta config, en la carpeta de Maven.

### Creación de un clon del repositorio CITSmart-ITESM  

 - Acceda al enlace de abajo para la autenticación de sus datos de acceso en SCMManager: 

https://scm.centralit.com.br/scm/#repositoryPanel;4MRv1XSxO9 

 - En el campo Search introduzca: 

<i> citsmart-itsm-enterprise</i>  

 - Copie el enlace en el campo _Checkout_ en la parte inferior de la página para el Git Clone.

 - Abra la carpeta donde desea clonar el repositorio CITSmart y ejecute el Terminal. 

 - Introduzca git clone + el enlace copiado en el campo Checkout y dale el Enter. Se le pedirá la contraseña de red. Este proceso puede tardar unos minutos.   

### Creación del servidor, databases y Login Group Roles en PGADMIN

 - Acceda al siguiente enlace para la creación de los servidores: http://localhost:8081/ 

 - Puede ser necesario crear una nueva cuenta si no tiene registro.

 - Después de acceder, haga clic con el botón derecho encima  _Servers/Create/Server_

 - En la pestaña _General_ y en el campo _Name_, introduzca _dbcitsmart_.

 - En la pestaña _Connection_ introduzca:  
  
 <i>postgres  
 5432  
 postgres  
 postgres  
 post  </i> 

 - En el servidor creado, en el menú izquierdo de la pantalla, haga clic con el botón derecho y cree un Database con el nombre _dbcitsmart_  

 - En Login/Group Roles, en el menú izquierdo de la pantalla, haga clic con el botón derecho encima y seleccione **Create/Login/Group Roles**  

 - En la pestaña General y en el campo Name, introduzca _root_  

 - Repita la operación y cree un **Login/Group Roles** con el nombre _rtsadmin_
 
### Instalación de Docker

 - Acceda al terminal de Ubuntu e introduzca:

 _sudo apt install docker-compose_  

 - Después de la instalación, acceda a la carpeta que contiene las Bases de Datos SQL, Postgres y Oracle y ejecute el terminal introduciendo respectivamente: 

<i>sudo docker ps  

sudo docker exec -it postgres bash  

su postgres  

cd /home  

ls  

psql -l  </i>

 - Todavía con el Terminal abierto, ejecutaremos el Restore del Banco, introduzca como abajo:  

<i>pg_restore -d dbcitsmart dbcitsmart.sql </i>

 - Inmediatamente después, regrese a PgAdmin, haga clic con el botón derecho y dale el Refresh, acceda a **dbcitsmart/Schemas/Tables** y compruebe las tablas migradas por Docker.  

### Instalación de Eclipse  


 - Acceda al siguiente enlace para descargar **Eclipse IDE**: 

https://www.eclipse.org/downloads/packages/release/2020-06/r/eclipse-ide-enterprise-java-developers   

 - En la opción Descargar enlaces, seleccione la versión para **Linux**.  

 - Extraiga el archivo descargado a la carpeta de Desarrollo.

 - En la carpeta donde se extrajo Eclipse, abra el archivo _eclipse.ini_ y edite las opciones como abajo:

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image1.jpg)

 - Ejecuta el archivo Eclipse y selecciona un directorio para que sea tu workspace. Puede marcar la opción **"Use this as the default and do not ask again"** para que la selección del directorio de workspace no se solicite de nuevo.

 

 - Seleccione en **File** la opción **Import**: 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image2.png)

 

 - En la opción Maven, seleccione **Existing Maven Projects.**  
 

 - Introduzca la ruta de acceso al directorio donde se encuentra el repositorio _Citsmart-itsm_: 

 ![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image3.png)
 

 - El Proyecto aparecerá como se muestra a continuación: 


![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image4.png)
  

 - En la pantalla de inicio del eclipse, abre la ventana **Window/Preferences** y completa las opciones de las siguientes pantallas como se muestra a continuación:

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image5.png)


![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image6.png)


![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image7.png)


![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image8.png)


![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image9.png)


![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image10.png)


![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image11.png)

 

 - Localice la opción **Validation**, buscando en la barra de búsqueda, y habilite la opción **Suspend all validators**, como abajo: 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image12.png)
 


 - En la pantalla de inicio del eclipse, haga clic con el botón derecho del ratón en la parte superior del Proyecto, elija **Run As/Run Configurations** y complete las opciones de las siguientes pantallas como se muestra a continuación: 

 
![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image13.png)

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image14.png)
 

 - El siguiente paso será establecer un nuevo Servers como se muestra a continuación: 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image15.png)
 

 - Haga clic en el enlace en azul _"No Servers are available. Click this link to create a new server..."_

 - Elija la opción de la siguiente manera: 
 
![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image16.png)

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image17.png)

!!! note "Nota"

     Haga clic en la barra de progreso y arrastre al lado de la pestaña Servers. 

  
 

 - En la pestaña Markers, haga clic con el botón derecho del ratón en las **Description** que tengan el icono rojo y elija **Remove**: 

 - En la opción del New Server, seleccione **WildFly 12**: 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image18.png)
 

 - En la opción Configuration file, seleccione el archivo xml _standalone-postgres-full.xml_, descargado en OneDrive: 
 

 - En la pantalla de inicio del eclipse, abra la ventana **Window/Preferences**, localice la opción Maven, seleccione la opción **User Settings** y complete como se indica a continuación: 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image19.png)
 

 - Después de instalar WildFly en Servers, aparecerá en Eclipse como se muestra a continuación: 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image20.png)

 

 - Haga doble clic encima de WildFly 12 y complete como se indica a continuación: 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image21.png)


![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image22.png)


![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image23.png)


![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image24.png)


 - En la opción **Program arguments** complete como se indica a continuación:  

<i>-mp "/home/run2biz/Documents/Desenvolvimento/WILDFLY-12.0.0/modules" org.jboss.as.standalone -b localhost --server-config=standalone-postgres-full.xml -Djboss.server.base.dir=/home/run2biz/Documents/Desenvolvimento/WILDFLY-12.0.0/standalone </i>

 

 - En la opción **VM arguments** complete como se indica a continuación: 

<i> "-Dprogram.name=JBossTools: WildFly 12" -server -Xms128m -Xmx2048m -Dorg.jboss.resolver.warning=true -Djava.net.preferIPv4Stack=true -Dsun.rmi.dgc.client.gcInterval=3600000 -Dsun.rmi.dgc.server.gcInterval=3600000 -Djboss.modules.system.pkgs=org.jboss.byteman -Djava.awt.headless=true "-Dorg.jboss.boot.log.file=/home/run2biz/Documents/Desenvolvimento/WILDFLY-12.0.0/standalone/log/boot.log" "-Dlogging.configuration=file:/home/run2biz/Documents/Desenvolvimento/WILDFLY-12.0.0/standalone/configuration/logging.properties" "-Djboss.home.dir=/home/run2biz/Documents/Desenvolvimento/WILDFLY-12.0.0" -Djboss.bind.address.management=localhost -XX:-UseGCOverheadLimit </i>
 

 - Compruebe la información del Directorio según su Directorio. 

 - Aún en la configuración de WildFly 12, complete el Time Limit, como abajo: 

 
![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image25.png)

 - Poco después, haga clic en Guardar. 

 
 - Haga clic con el botón derecho del ratón en la parte superior de WildFly, elija la opción **Add and Remove**, seleccione Citsmart9 y añada:

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image26.png)
 

 - Compruebe el archivo _clean.sh_, descargado en OneDrive: 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image27.png)

!!! note "Nota"  

      La información del Directorio resaltada en negrita debe reemplazarse según su Directorio: 

rm -rf /home/**run2biz/Documents/Desenvolvimento**/workspace/citsmart-itsm-enterprise/target/* 

rm -rf /home/**run2biz/Documents/Desenvolvimento**/WILDFLY-12.0.0/standalone/deployments/* 

rm -rf /home/**run2biz/Documents/Desenvolvimento**/WILDFLY-12.0.0/standalone/data/ 

rm -rf /home/**run2biz/Documents/Desenvolvimento**/WILDFLY-12.0.0/standalone/log/ 

rm -rf /home/**run2biz/Documents/Desenvolvimento**/WILDFLY-12.0.0/standalone/tmp/ 

 - Siga los siguientes pasos para que el Proyecto funcione correctamente. 


 - Ejecute el _clean.sh_ 
 

 - Elimine el Proyecto en WildFly haciendo clic con el botón derecho del ratón y eligiendo **Remove*.

 
 - Vaya al Proyecto, haga clic con el botón derecho del ratón y elija **Refresh**. 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image28.png)

 - También en el Proyecto, haga clic con el botón derecho del ratón y elija**Run as/Run Configuration/Run**. 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image29.png)

 

 - Vaya al Proyecto, haga clic con el botón derecho del ratón y elija **Refresh**. 

 - Haga clic con el botón derecho del ratón en la parte superior de WildFly, elija la opción **Add and Remove**, seleccione Citsmart9 y añada: 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image30.png)

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image31.png)

 

 - Con el Proyecto añadido en Wildfly, haga clic con el botón derecho del ratón en la parte superior de WildFly y elija **Clean**.

 - Aparecerá la pantalla de abajo, marque la opción **Remember my decision** y haga clic en el botón **No**: 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image32.png)
 
![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image33.png)

 

 - El proyecto Citsmart9 aparecerá enWildFly. 


!!! note "Nota"  

      En caso de que el Proyecto no funcione, después de todos los pasos anteriores, haga clic con el botón derecho del ratón en la parte superior del Proyecto, Maven / Update Project y repita nuevamente el Paso a Paso. 

![imagem 1](/pt-br/citsmart-platform-9/get-started/installation-and-upgrade/images-linux/image34.png)
 
 - Acceda al siguiente enlace para CITSmart: 

https://localhost:8443/citsmart 


 - Haga clic en **Advance/Proceed**

 - ¡Listo, el entorno está configurado!
