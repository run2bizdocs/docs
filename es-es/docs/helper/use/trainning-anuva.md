Título: Entrenamiento 

# Entrenamientos

## ¿Qué significa entrenar a mi asistente virtual?

Es el acto de colocar su asistente para entender cómo serán las interacciones con el usuario considerando los diálogos construidos. Cada vez que se añaden nuevas interacciones, es necesario volver a entrenar a su asistente para que pueda reaccionar de la manera esperada en una conversación. 

El único requisito previo para programar un entrenamiento de su asistente virtual es que haya al menos un diálogo creado.

## Antes de empezar  

Asegúrese de que todas las configuraciones de parametrización e infraestructura se hayan realizado correctamente.

## Procedimiento 

### Programar entrenamiento

1.	Después de acceder a la plataforma, acceda al menú Entrenamientos;

2.	Haga clic en el botón Programar;

3.	Defina cuál será el alcance de la actualización que desea, siendo las opciones: Diálogos, Completo, Habilidades (Texto - Botón - Imagen) o Habilidades personalizadas;

4.	Informe el día y hora en que el entrenamiento deberá ser realizado.

> *Nota: Recuerda elegir fechas y horarios que tendrán menos impacto en los servicios en curso, si los hay. *

!!! note "Información"

    El tiempo de duración de cada entrenamiento variará según el volumen de flujos de conversación construidos, pero no se preocupe, tan pronto como se haya completado, su asistente está automáticamente listo para actuar, ya sea en la prueba de conversación dentro de la plataforma o en el entorno de producción.

### Solución de problemas  

<b>Finalizando un Entrenamiento </b>  

Una vez iniciado el entrenamiento, la aplicación no ofrece al usuario la opción de finalizar el proceso, pero a veces puede ser necesario. Las siguientes instrucciones conducen en la realización de esta tarea, que consiste en limpiar la cola de tarea y finalizar la máquina adquirida para este fin.  

    1.	Acceda al servicio Simple Queue Service desde el panel de servicios de AWS
    2.	Busque la cola denominada citsmart-anuvaassistant-training-<ambiente> y selecciónela. Por ejemplo, el nombre para el ambiente "homologation" en la cola sería citsmart-anuvaassistant-training-homologation.
    3.	Haga clic en Actions y seleccione "Purge"  
    4.	Escreva o termo solicitado e clique no botão "Purge"  
    5.	Después de este procedimiento, la cola debe estar limpia.  
    
Para finalizar la instancia adquirida, siga las instrucciones siguientes:  

    1.	Acceder al servicio EC2 en el panel de servicios de AWS  
    2.	Haga clic en el enlace a Instancias (ejecutando)  
    3.	Buscar una instancia que tenga el término "spot"  
    4.	Seleccionar la instancia deseada 
    5.	Hacer clic en Actions y solicitar detener la instancia confirmando la elección en el botón "Stop"  
    6.	Hacer clic en Actions y solicitar finalizar la instancia, confirmando la elección en el botón "Terminate"  
    7.	Después de este procedimiento, un mensaje debería aparecer indicando la instancia eliminada.  
    
<b>El entrenamiento no comienza </b>  

Al intentar iniciar un entrenamiento programado, puede producirse un error y no comenzar el entrenamiento. Una de las causas de esta ocurrencia está relacionada con schedule de python que sufre una rotura, dejando de poner el entrenamiento en la cola.    

    1.	Para confirmar si el error está relacionado con schedule de python, observe la cola de AWS en Simple Queue Service, denominada "citsmart-anuvaassistant-training-homologation"  
    2.	En situaciones normales, la cola en cuestión debería mostrar sus mensajes cerosos.  
    3.	Si se produce un error, la cola mostrará 1 job programado en la columna de mensajes.  
    4.	En este caso, debe detener y reiniciar la instancia EC2 "anuvamultitenancyapihom_app".  
    5.	Después de reiniciar la instancia, elimine el entrenamiento programado y realice una nueva programación.
    
 <b> No se muestra el Ranking de Intents </b>

Este problema ocurre cuando la instancia anuvamultitenancyapihom_app tiene su IP alterada, por cualquier motivo, y este pasa a no constar en las reglas de autorización de acceso del servicio Elasticsearch. En este caso, un mensaje que indica el fallo en la presentación de los rankings aparece en varios puntos de la aplicación.  

Para resolver el problema, la IP de la instancia anuvamultitenancyapihom_app debe añadirse a la lista de autorizados, en las políticas de acceso al servicio Elasticsearch. Para ello, es necesario obtener la IP actual de EC2 anuvamultitenancyapihom_app, acceder al panel del servicio Elasticsearch e incluir la IP en la lista de autorizados. Para obtener la dirección IP, siga el procedimiento siguiente:

    1.	Acceda al panel administrativo de instancias EC2
    2.	Filtre las instancias que se están ejecutando/activas
    3.	Seleccione la instancia en cuestión y copie el número de su IP 
    
Para acceder al panel de Elasticsearch e incluir la IP en la lista:

    1.	Seleccione el menú Analytics > Elasticsearch Service
    2.	En Dashboard, haga clic en My Domains y seleccione el servicio relacionado
    3.	Después de seleccionar el servicio, haga clic en el botón Actions > Modify Access Policy
    4.	En esta página, incluya el número de IP copiado en el vínculo de autorizados y haga clic en el botón Submit para aplicar el cambio.
    
### Pruebas Automatizadas
 
Las pruebas de software se insertan en la gestión del ciclo de vida de las aplicaciones (más conocido como ALM). Es un paso primordial para garantizar la calidad del producto entregado al cliente, o incluso para ser utilizado por el propio equipo de desarrollo para asegurarse de su asertividad.  

Automatizamos para evitar el trabajo manual repetido, obtener un feedback más rápido, ahorrar tiempo ejecutando pruebas repetidamente, y asegurar que siempre estamos ejecutando pruebas de manera consistente con las mismas precondiciones y expectativas.  

En general, las razones para abordar la existencia de pruebas son:

   - Comprobar si el programa cumple con las expectativas del cliente;  

   - Comprobar cualquier error antes de que tus clientes lo vean;  

   - Detectar problemas en el diseño;  

   - Asegúrese de que el sistema es estable;  

   - Garantizar que el trabajo desarrollado por el equipo sea de calidad;  
   
Para la automatización de pruebas del proyecto en cuestión, se está utilizando la herramienta Cypress. Uno de los principales diferenciales de Cypress es que mientras que la mayoría de las herramientas de prueba operan fuera del navegador, ejecutando comandos remotos en la red, Cypress es exactamente lo contrario, se ejecuta en el mismo bucle de ejecución de la aplicación que se está probando. Esto permite una interactividad muy grande.  

Los siguientes procedimientos proporcionan instrucciones de instalación y configuraciones básicas para iniciar e interactuar con este proyecto de pruebas, así como para documentar los criterios y estándares adoptados para la buena práctica en su conducción y las implementaciones siguientes.

<b>1. Prueba funcional</b>

Prueba los requisitos funcionales de la aplicación. En resumen, comprobar si la aplicación es capaz de realizar las funciones para la cual fue desarrollada para hacer, pudiendo abarcar las funcionalidades en todo su alcance, tanto BackEnd como FrontEnd.

<b>2. Instalación y configuración </b>

Preliminarmente, usted ya debe poseer el Node.js instalado y, a nivel de sugerencia el IDE VsCode. Teniendo estos requisitos previos, siga el procedimiento siguiente:
    
   - <b>Crear el directorio de trabajo:</b> Crea un directorio para el proyecto, aquí sugestivamente creamos el directorio <i>cypress-tests $ mkdir cypress-tests</i> 
   - <b>Crear el proyecto:</b> Acceda al directorio que se creó e inicie el proyecto con el comando abajo. Este comando generará toda la estructura inicial requerida: <i>$ npm init -y</i> 
   - <b>Instalar Cypress:</b> Permaneciendo en el directorio del proyecto, instale Cypress según lo indicado: <i>$ npm install cypress</i>  
Si es necesario, se pueden obtener instrucciones completas en la documentación oficial.

!!! note "Nota"  
        
           Si desea instalar una versión específica, como 4.6.2 por ejemplo, haga del siguiente modo: <i>$ npm install cypress@4.6.2</i>
           
 <b>3. Configurar VsCode</b>  

Como se sugirió anteriormente, estaremos utilizando VsCode como IDE para el desarrollo de nuestras pruebas, por lo tanto el mismo ya debe estar instalado previamente. Vamos a añadir al archivo package.json el comando que utilizamos para ejecutar el proyecto. Esto acelerará el procedimiento. Edite el archivo package.json, y en el tema script, añada el comando, según el ejemplo:  
 
 <i> $ "scripts": { "cypress:open": "cypress open"</i>
 <b>4. Ejecutar el proyecto:</b>

Después de haber incluido el comando, según la instrucción anterior, el proyecto se puede ejecutar a través de la línea de comandos:  

<i>$ npm run cypress:open</i>  

o a través de VsCode, por el camino Outline > NPM Scripts > package.json > cypress:open > botón "play"  

<b>5. Estructura de directorios y archivos </b>  

Se propone la siguiente estructura de archivos para mantener un estándar organizacional del proyecto. Sin embargo, no existen restricciones técnicas para otros enfoques, sino que las buenas prácticas se basan en una mera convención para el proyecto en cuestión:

   - <b>I. Fixtures: </b> Directorio destinado a los archivos que contendrán diccionarios con datos que se utilizarán para las pruebas en el llenado de información. Algunas buenas prácticas son:  
    
        - El uso de fixtures es una buena práctica para agilizar el desarrollo y el mantenimiento del proyecto, pues agrega en una única área los datos variables utilizados por el proyecto.  
          
        - Por motivos de organización, se debe tener un archivo fixture para cada archivo de prueba.  
         
        - Deben evitarse los bloques muy extensos. Cuando el volumen es grande, se sugiere su división en temas.  
         
        - Los commands no deben manejar los datos directamente. Los datos deben ser manipulados en las intents.
          
   
   - <b>II. Integration:</b> Directorio destinado a contener las pruebas a realizar, en la aplicación. Algunas buenas prácticas son:  
   
        - Estos archivos deben restringirse a la lógica de las pruebas y de la manipulación de los datos, dejando a cargo de los commands la ejecución de los procedimientos con las debidas interacciones con pantallas y APIs. </br> 
        
        - Por motivos de organización, se debe tener un archivo command para cada archivo de prueba. </br> 

        - Los archivos de prueba no deben manejar los componentes de la pantalla directamente, lo que hace que los archivos de commands estén a cargo. Por lo tanto, no deben importar archivos locators. </br> 
        
        - Los archivos de prueba importan los archivos fixtures, para el manejo de datos y el paso de los mismos a los commands. </br> 

   - <b>III. plugins:</b> Directorio destinado a contener el registro de eventuales plugins utilizados en el proyecto.  
   
   - <b>IV. support:</b> Directorio destinado a contener códigos de soporte a los archivos de prueba, que deben contener los siguientes directorios para mejor agrupamiento:  
     
      - **commands:** Estos archivos son utilizados por las pruebas, ubicadas en el directorio Integration. Deben contener los códigos de los comandos utilizados por las pruebas. Además de los archivos commands individuales para cada archivo de prueba, también tenemos uno de uso Global. Algunas buenas prácticas son:  </br> 
            
            - El uso de commands es una buena práctica para acelerar el desarrollo y el mantenimiento del proyecto, ya que evita códigos redundantes.  
            
            - Por motivos de organización, se debe tener un archivo command para cada archivo de prueba.  
            
            - Los commands no deben manejar los datos directamente. Los datos deben venir a través de parámetros. Por lo tanto, no deben importar archivos fixtures.  
            
            - Los commands importan los archivos locators.  
            
            - Mantener los métodos en orden alfabético facilita la localización y la lectura, además de que intuitivamente lleva a un patrón en la creación de sus nomenclaturas.    

            - El archivo commands de uso global, como su nombre lo indica, debe contener los comandos de pruebas de uso global en el proyecto. Un buen ejemplo para este uso es el método de verificación de URL, que puede ser único y servir a toda la aplicación.  
        
      - **llocators:** Directorio destinado a contener los archivos que registran las direcciones de acceso a los widgets de pantalla, URLs y demás direcciones. Según lo determinado en las buenas prácticas de este proyecto, los archivos de locators deben ser importados y utilizados por los commands. Además de los archivos locators individuales para cada archivo de prueba, también tenemos uno de uso Global. Algunas buenas prácticas son:   
        
            - El uso de locators es una buena práctica para agilizar el desarrollo y el mantenimiento del proyecto, pues agrega en única área las vías de acceso a los widgets de pantalla y URLs. 

            - Los archivos locatorss deben ser importados por los commands.  
            
            - Debe tener un archivo locators para cada archivo de pruebas.  
            
            - Deben evitarse los bloques muy extensos.Cuando el volumen es grande, se sugiere su división en temas.  


   - <b>V. node_modules:</b> Directorio que contiene el registro y archivos de las bibliotecas utilizadas por el proyecto.
      
   - <b>VI. cypress.json:</b> Archivo de configuración central de Cypress. Básicamente contiene valores de variables de ámbito global al sistema. Registre en este archivo las urls a ser manipuladas por el sistema.  
   
   - <b>VII. package.json:</b> Archivo de datos de registros de la aplicación y llamadas a scripts que automatizan sus procesos de arranque.  

   - <b>VIII. package-lock.json:</b> Archivo que registra las dependencias de las bibliotecas externas utilizadas por la aplicación.  
   
   - <b>IX. .gitignore:</b> Archivo que contiene la relación de archivos y/o directorios que no deben ser versionados por el Git.  
   
   - <b>X.index.js:</b> Archivo que contiene las llamadas iniciales del sistema de pruebas.
   
<b>6. Patrones de nomenclaturas </b>  

Se ha adoptado el siguiente estándar para la creación y la denominación de los archivos:  

<i>< contenido > < Módulo > .js  </i>

Ejemplos:  

        - Archivos de fixtures: datasContext.js / datasTheme.js 
        - Archivos de commands: commandsContext.js / commandsLogin.js  
        - Archivos de locators: locatorsLogin.js / locatorsTheme.js    
    
!!! note "Nota"  

        Tenga en cuenta que el plural solo se debe utilizar en el contenido, ya que el contenido normalmente se refiere a más de un elemento. Tenga en cuenta también que la identificación del módulo se inicia con letra mayúscula. 

En esta estructura, tenemos una excepción en cuanto a los archivos de pruebas propiamente dichos, que están contenidos en el directorio Integration. Estos archivos deben seguir el siguiente patrón:  
    
<i>< módulo > .spec.js </i> 
    
Ejemplos:
    
        - context.spec.js  
        - login.spec.js  
        - theme.spec.js 

   
Relacionado
-----------

[Cómo enseñar su Helper](/es-es/helper/use/teach-helper.html)

[Monitorear las interacciones de su Helper](/es-es/helper/use/monitoring-helper.html)

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
