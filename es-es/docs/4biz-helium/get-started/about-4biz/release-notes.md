Title: Notas de Release
Description: Notas de la versión, corrección de errores y mejoras de 4biz.

# Notas de Release

## Versión Helium 1.2.23 (2021/01/05)

!!! warning "ATENCIÓN" 

    Antes de descargar esta versión, consulte las orientaciones en el documento Guía de orientaciones del 4biz Helium versión 1.2.23

Bienvenido a 4biz Helium Versión 1.2.23. Esta versión incluye los siguientes elementos:

|Número         |Tipo       |Descripción        |
|---------------|-----------|-------------------|
|Incidente 5929 |Correctiva |Corrección de seguridad del producto evitando aceptar LDAP Injection, caracteres especiales en el inicio de sesión de usuario y tamaño de inicio de sesión|

Bienvenido a Builder 1.3.5.4 

La versión presentada tiene las siguientes correcciones: 

|Número         |Tipo       |Descripción        |
|---------------|-----------|-------------------|
|10280          |Corrección |Recuperación del valor default de las columnas del objeto de negocio|


## Versión Helium 1.2.22 (2020/12/03)

!!! warning "ATENCIÓN"

    Antes de descargar esta versión, consulte las orientaciones en el documento Guía de orientaciones del 4biz Helium versión 1.2.22

Bienvenido a 4biz Helium Versión 1.2.22. Esta versión incluye los siguientes elementos: 

|Número         |Tipo       |Descripción        |
|---------------|-----------|-------------------|
|10176          |Correctiva |Corrección de componente lookup|
|Incidente 5800 |Correctiva |Corrección de error al limitar un select con comando TOP|
		
Bienvenido a Builder 1.3.6.1 

La versión presentada tiene la siguiente corrección: 

|Número         |Tipo       |Descripción        |
|---------------|-----------|-------------------|
|10476          |Corrección |[My 5802] - Menús laterales de Builder no funcionan correctamente|

## Versión Helium 1.2.13 (2021/01/05)

!!! warning "ATENCIÓN"

    Antes de descargar esta versión, consulte las orientaciones en el documento [Guía de orientaciones del 4biz Helium versión 1.2.13][2]

Bienvenido a 4biz Helium Versión 1.2.13. Esta versión incluye los siguientes elementos:

|Número|Tipo|Funcionalidad|Descripción|
|--------|---------|---------|---------|
|10005|Corrección|Sistema|Correcciones en la Auditoría|
|10008|Corrección|G. de Ticket|Corrección en la visualización del SLA a combinar|
|10011|Corrección|Webservice|Mejora en el webservice de telefonía en cuanto a la sesión del usuario|
|10012|Corrección|G. de Ticket|Corrección en la representación de formularios Builder|
|10013|Corrección|G. de Ticket|Corrección en la visualización de un ticket|
|10019|Corrección|G. de Ticket|Corrección al actualizar la lista Sin Responsable|
|10022|Corrección|G. de Ticket|Corrección en la recuperación de tickets para comentarios|
|10023|Corrección|Webservice|Corrección del mecanismo de telefonía websocket con Builder|
|10031|Corrección|G. de Ticket|Corrección en registros de comentarios reclasificados|
|10034|Corrección|G. de Ticket|Corrección en la visualización de la información del solicitante del ticket|
|10035|Corrección|Webservice|Incluir información sobre el ticket creado en el nuevo modal de telefonía|
|10044|Corrección|Chat|Corrección para avanzar el flujo de chatcall de ticket cancelado/cerrado|
|10047|Corrección|G. de Ticket|[My 5540] – Corrección en el envío de correo electrónico al finalizar el servicio|
|10051|Corrección|G. de Ticket|[My 5317] - Problema con la consulta que no se filtra por grupo|
|10052|Corrección|G. de Ticket|No se esta enumerando los tickets para el usuario que solo tiene el permiso "Puedo comentar"|
|10056|Corrección|G. de Ticket|[My 5405] - Error intermitente al intentar la aprobación vía token|
|10057|Corrección|G. de Portafolio|[My 5351] - Problema con el botón de grabación al editar un Portafolio|
|10058|Corrección|G. de Ticket|[My 5339] - Error al crear ticket mediante la lectura de correo electrónico|
|10061|Corrección|Chat|[My 5450] - Error al iniciar una conversación vía chat|
|10065|Corrección|G. de Ticket|Compruebe si hay errores al buscar por la búsqueda avanzada|
|10083|Corrección|G. de Ticket|Corrección cde clave internacionalizada de tipo SLA en caso de solicitud|
|10093|Corrección|G. de Ticket|Manejar transacciones de cierre en transacitionControlerIMPL|
|10097|Corrección|G. de Ticket|Corrección del mensaje "Espere, cargando ..." en la auditoría|
|10098|Corrección|G. de Ticket|Tratar null pointer en la clase OcorrenciaSolicitacaoBuilder|
|10178|Corrección|Flujo|Creación de campos para programar ejecuciones de Rhino Script|
|10204|Corrección|G. de Portafolio|Corrección en la exclusión de Causa Incidente en el Portafolio|
|10211|Corrección|Sistema|Corrección al agregar una imagen a la galería de imágenes|
|10216|Corrección|G. de Portafolio|Corrección en el campo obligatorio del Portafolio|
|8542|Corrección|G. de Ticket|Visualización de respuestas a comentarios en la exportación CSV|
|8589|Corrección|G. de Ticket|Mostrar los nombres de los archivos adjuntos en el historial de creación de tickets|
|9320|Corrección|G. de Ticket|Incluir en las ocurrencias información sobre inclusión y exclusión de los procesos de negocio|
|9826|Corrección|Sistema|Eliminación del SequenceBlock|
|9839|Corrección|G. de Problema|[My 5160] - Error al agregar el Portafolio de Problema|
|9890|Corrección|G. de Ticket|[My 5408] - Corrección de error al mostrar el nombre del contrato al ver el ticket|
|9915|Corrección|G. de Problema|Error al desvincular el contrato del Portafolio de Problema|
|9955|Corrección|G. de Ticket|[My 5403] -Verifique la falla de auditoría al informar la reclasificación de tickets|
|9949|Corrección|G. de Ticket|[MY 5352] - Verificar el historial de delegación que no se muestra en la pestaña del historial de ticket|
|9965|Corrección|G. de Ticket|Verificar que no muestra el motivo de la reclasificación en el historial|
|9968|Corrección|Sistema|[My 5338] - Entorno VNS lento al enumerar la cola de tickets|
|9957|Corrección|G. de Ticket|[My 5121- 5180 - 5163] Error al insertar el adjunto en el subticket creado por copia|
|9959|Corrección|G. de Ticket|[My 5172]- La paginación de la pantalla del ticket va a cero|   

Bienvenido a Builder 1.3.5.1

La versión presentada tiene las siguientes correcciones:

|Número|Tipo|Descrição|
|--------|---------|---------|
|100175|Corrección|Corrección en la internacionalización en un ambiente clusterizado|
|10049|Corrección|[My 5357]- No se pudieron validar los permisos del botón, incluso con el usuario con permiso|
|9751|Corrección|[My 5153] - Verifique que los archivos que tienen nombres con caracteres especiales no se cargan|

## Versión Helium 1.1.1 (2020/09/14)
Bienvenido a 4biz Helium Versión 1.1.1. Esta versión incluye los siguientes elementos:

|Número|Tipo|Funcionalidad|Descripción|
|--------|---------|---------|---------|
|9635|Corrección|G. Liberación|Se corrigió la visualización del icono de reapertura en la pantalla de búsqueda avanzada de la liberación|
|9594|Corrección|G. Cambio|Error en la lista de cambios debido a la flag Active creada en la tabla de itemtrabajo|
|9607|Corrección|G. Ticket|Error al recuperar la búsqueda avanzada|
|5089|Corrección|G. Ticket|Error en la lectura del correo electrónico del solicitante|
|5002|Corrección|Registro Proyecto|Error al buscar los documentos de registro del proyecto|
|9579|Corrección|G. Problema|Error al resolver un Problema|
|9570|Corrección|G. Ticket|Error al ver el flujo en un ticket|
|4930|Corrección|G. Ticket|Verificar si hay error de cálculo de SLA|
|9408|Corrección|G. Conocimiento|Al acceder al portal de conocimiento con un usuario externo, el visitante intenta cargar el archivo que se encuentra en el conocimiento, la carga no se realiza|
|9412|Corrección|Chat|El chat muestra un error solo en el log al capturar y avanzar el flujo|
|4997|Corrección|G. Ticket|Corrección de duplicación de buzones de correo|
|9378|Corrección|G. Ticket|En el Smart Portal, en el historial de un ticket al buscar el Identificador, el campo no es del tamaño correcto y no se puede digitar. Además presenta el error "No se pudo cargar recurso: el servidor respondió con un estado de 403 ()"|
|9287|Corrección|Registro de Grupo|Error al acceder a la pantalla de Grupo|
|9289|Corrección|Registro de Persona|Pantalla de búsqueda de empleados con un error de Front End al buscar un empleado con un estado igual a "Inactivo"|
|9218|Corrección|G. Conocimiento|El registro de conocimientos no se abre|
|4875|Corrección|Tasker|Se ajustó la vista de sprint vencida|
|9219|Corrección|G. Ticket|Subir archivo adjunto de ticket congelando en la pantalla|
|9221|Corrección|Smart Portal|Corrección del botón de cierre que permanece inerte después de grabar un ticket|
|9282|Corrección|Flujo|Error de flujo al vincular un cuestionario de "Seguimiento", ya sea obligatorio o no|
|4633|Corrección|G. Ticket|El sistema no está creando un ticket con el usuario existente en el sistema|
|9126|Corrección|Webservice|Presentar el cuestionario en la aplicación|
|9217|Corrección|G. Cambio|Portafolio de Cambio no se abre|
|4861|Corrección|G. Ticket|Duplicación de ticket reclasificado|
|4668|Corrección|G. Ticket|Duplicación de la tarea de flujo en la delegación|

|Número|Tipo|Funcionalidad|Descripción|
|--------|---------|---------|---------|
|9201|Mejora|G. Ticket|Inclusión de flag en el elemento de trabajo de flujo para aumentar el rendimiento de la aplicación|
|9583|Mejora|G. Ticket|Cambiar al buscar permisos en la lista de ticket|
|9434|Mejora|Sistema|Eliminar la pantalla de acceso de las herramientas de datos de la aplicación|
|9584|Mejora|G. Ticket|Cambiar cuándo buscar grupos en ejecución en la lista de tickets|
|9427|Mejora|Webservice|Permitir responder cuestionario de creación por la aplicación|
|9440|Mejora|Webservice|Permitir filtrar tickets a través de la aplicación|
|8837|Mejora|Webservice|Crear un servicio web que enumere los grupos que se dirigirán a un ticket|
|9342|Mejora|Webservice|Reclasificar ticket por la aplicación|
|9429|Mejora|Webservice|Aumentar la capacidad del campo Extensión de registro de empleados|
|9428|Mejora|Webservice|Identificar el tipo de cuestionario presentado para la identificación de la aplicación|
|9333|Mejora|Webservice|Presentar información extraída de las acciones del usuario en la aplicación|
|9011|Mejora|Webservice|Permitir opciones de flujo en la aplicación|
|8840|Mejora|Webservice|Crear un servicio web que enumere las razones para suspender un ticket|
|8834|Mejora|Webservice|Crear un servicio web que enumere las Unidades para su selección|
|8839|Mejora|Webservice|Cree un servicio web que enumere las categorías de soluciones para resolver un ticket en la aplicación|
|8832|Mejora|Webservice|Presentar información de cierre y responsable de consumo de la aplicación|
|9297|Mejora|G. Ticket|Eliminación de tickets innecesarios en el método filterContract de la clase ServiceResquestIncident - Se eliminó la restauración de proveedores y clientes dentro de la iteración del contrato|
|9010|Mejora|Webservice|Eliminar el archivo adjunto de la aplicación|
|8413|Mejora|Registro de Persona|Crear y Buscar Persona|
|8838|Mejora|Webservice|Crear un servicio web que enumere las causas para resolver un ticket|
|9313|Mejora|G. Ticket|Incluir la gestión de colas para la extracción de datos en "Búsqueda avanzada"|
|8833|Mejora|Webservice|Servicio web que le permite delegar un ticket a un analista|
|9222|Mejora|G. Ticket|Performance - Reemplazar employeecontract con materialized view|
|8855|Mejora|Webservice|Permitir enumerar usuarios y grupos que se pueden delegar en un ticket|
|8836|Mejora|Webservice|Crear un servicio web que enumere la ubicación de una unidad del ticket|
|8835|Mejora|Webservice|Crear un servicio web que enumere la fuente de contacto del ticket|
|8426|Mejora||Colocar el nombre del cliente que ha obtenido la licencia del entorno al final de la página|

Bienvenido a Builder 1.3.5.0. La versión presentada tiene las siguientes correcciones:

|Número|Tipo|Descripción|
|--------|---------|---------|
|7814|Corrección|Refactoría de integración con ITSM para permitir la flexibilidad de la URL externa del Builder|
|8416|Corrección|Corrección del error al utilizar el flujo ESI como componente en el flujo de trabajo|

|Número|Tipo|Descripción|
|--------|---------|---------|
|7751|Mejora|Ajustar los nombres de las propiedades de los componentes del portugués al inglés|
|7774|Mejora|Error de traducción en el BUILDER --> ESI|


## Versión Helium 1.0.2 (2020/04/27)
Bienvenido a 4biz Helium Versión 1.0.2 Esta versión incluye los siguientes elementos:

|Número|Tipo|Funcionalidad|Descripción|
|--------|---------|---------|---------|
|8968|Corrección|Center|Corrección en la devolución de la lista de Portafolios cuando se habilita el parámetro 293 que filtra el portafolio por grupos de acceso|
|4818|Corretiva|Tiempo de Atención|Corrección en la programación de una actividad para vincular al SLA registrado|

[2]:/es-es/4biz-helium/get-started/about-4biz/Guidance-4biz-Helium1213.zip
