title: Crear flujo de trabajo
Description: Es posible crear flujos de trabajo que mejor se adecuan a la realidad del usuario

# Crear flujo de trabajo

 Es posible crear flujos de trabajo que mejor se adecuan a la realidad del usuario, personalizando los escenarios de cada organización.

Procedimiento
------------

1.  Acceder al menú principal Tracker \> Diseño de Flujo;

2.  Hacer clic en "Nuevo";

3.  En la pestaña "Datos del Flujo" es necesario completar los datos obligatorios: nombre
    del flujo (su identificador interno, debe ser informado sin espacio, acentos y caracteres especiales); el proceso al que está vinculado (el flujo estará sólo para el proceso al que está vinculado) y la opción para permitir la reapertura de un servicio independientemente de la configuración de grupo. También se puede ver qué versión se encuentra el flujo.  
    En la pestaña también se encuentra el campo "Scripts Timeout (segundos): Campo Obligatorio donde se deben informar los segundos según la regla. A partir de la versión 2.0.0, el sistema detiene la ejecución de un script de Rhino desde un flujo de 4biz o Builder que lleva más tiempo que el definido en el atributo "Scripts Timeout (segundos)". El valor por defecto de este atributo se puede configurar en el parámetro HINO_TIMEOUT_EXCECUTION (en segundos) del archivo APPLICATION.INI. Si el parámetro no está configurado en el archivo, el sistema tiene un valor predeterminado de 90 segundos. Los flujos existentes antes de la instalación de la nueva versión se inicializaron a 90 segundos.

4.  En la pestaña "Diagrama" se muestra la herramienta para dibujar el flujo insertando los elementos que representan el escenario deseado. Para ello, basta hacer clic en el elemento y arrastrarlo al área de dibujo. Al hacer esto, se mostrará una pantalla para definir las propiedades. Debemos tener en cuenta que siempre un flujo comienza con el elemento "Evento Inicio" y termina con el elemento "Evento Fin".

    !!! Abstract "IMPORTANTE"
        
	    Los caminos condicionales de un flujo deben definirse en la conexión (Flujo de Secuencia). 
	    Para acceder a estas opciones, haga clic una vez en la conexión y después en el icono de propiedades.
	    Es posible identificar la conexión (Ej.: aprobada) e indicar una Condición, Acción o Estado. [Ver Construir                         Expresiones][2].

5.  Las propiedades de un elemento se pueden definir al hacer doble clic en el elemento y luego en el icono que aparece junto al mismo (icono de propiedades). Defina los datos de esta propiedad al informar los datos necesarios en cada una de las pestañas de la pantalla de propiedades. Aquí también se libera vincular un conocimiento al flujo en la "Base de conocimiento" e implementar funcionalidades en el flujo sobre la actividad actividad al hacer clic en la pestaña "Interfaz";

    !!! Abstract "ATENCIÓN"

        La pestaña "Interfaz" permite elegir el modo de interacción (formulario estándar, cuestionario o formulario builder) que             se aplicará al servicio. Sin embargo, si no ocurre la vinculación de ninguna plantilla de solicitud de servicio en esta pestaña, el sistema subentendirá y aplicará las configuraciones de un formulario estándar, habilitado para vincular el elemento de configuración, cambio, problema y solicitud relacionada con el ticket en la pantalla de gestión de tickets. Podemos citar también otra regla referente a esta pestaña: las normativas aquí configuradas tendrán prioridad en relación a las marcas del template de solicitud de servicio, ya que es un complemento del flujo.  

6.  Además, la funcionalidad admite importar flujos al hacer clic en el botón "Importar". Puede importar en el formato "JSON" o "XML".

7.  Después de definir el flujo, haga clic en el botón "Grabar" para efectuar la operación.

Relacionado
------------

[Registrar plantilla de ticket](/es-es/4biz-helium/platform-administration/questionnaires/ticket-template.html)


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021

[2]:/es-es/4biz-helium/workflow/configuration/expressions-creator.html
