Title: Situación de los Tickets en Racer 4biz
Description: En este documento, veremos las posibles acciones que se pueden realizar en el tratamiento de un ticket.

# Situación de los Tickets en Racer 4biz 

En este documento, veremos las posibles acciones que se pueden realizar para tratar un ticket dentro de la aplicación Racer 4Biz.

## Antes de empezar

- [x] Instalar la aplicación Racer 4biz en Android o IOS  
- [x] Tener un usuario registrado en el sistema a través de la aplicación

Además, es necesario realizar algunas configuraciones en la plataforma 4biz de Webservice, Unidad y Tickets.

**Webservice**

Acceder a la funcionalidad a través del menú principal Sistema > Webservice > Operación Webservice.  
En la pestaña Búsqueda de Operaciones, buscar por cada uno de los webservices abajo, a continuación, en cada uno hacer clic en el botón "Agregar grupo" e incluir el (los) grupo(s) que el (los) asistente(s) están vinculados:

    - request_add_attachments
    - request_updateRequestList
    - request_userLocation
    - request_saveRequest
    - request_uploadAttachment
    - request_getByUser
    - request_saveRequestNote
    - request_updateRequestNoteList
    - request_updateRequestListGroups
    - request_uploadSignature
    - parameter_query
    - registerdevice_query
    
El webservice de request_updateStatus deberá estar configurado con la siguiente información:
    
    - ID estándar para la justificación de la modificación de la llamada;
    - Agregar los grupos que tienen permiso para modificar el estado de una llamada;

Haga clic en el botón "Guardar" después de configurar los grupos en cada webservice.

**Unidad**

Acceder a la funcionalidad a través del menú principal Registros Generales > Administración de Personal > Unidad.  
Buscar por unidad en la pestaña Búsqueda de Unidad y seleccionar la elegida.
En la pestaña Registro de Unidad con la unidad ya elegida, haga clic en el botón "Obtener Coordenadas".
Hacer clic en "Guardar".

**Tickets**

Es necesario tener permiso para ver, capturar y realizar las acciones posibles dentro del ticket.  
Para reclasificar un ticket, el usuario tiene que pertenecer a un grupo ejecutor, en la pantalla de grupo vincular el Flujo a la opción de "Cambiar SLA", además de tener el permiso para "crear" en el flujo de la actividad destino, cuando la reclasificación incluya un intercambio de actividad y se trate de un escenario de flujos diferentes.  
El grupo deberá tener permiso para suspender en el flujo de la actividad.  
El administrador puede habilitar el parámetro para enviar un correo electrónico específico:
    - 290 - ID de plantilla de correo electrónico enviada al suspender una solicitud de servicio;

El administrador puede habilitar la obligatoriedad del campo para el complemento de la suspensión:

    - 372 - Habilitar el complemento obligatorio al suspender la solicitud

El administrador deberá haber registrado las Justificaciones de Solicitud para suspender el Ticket.  
El administrador deberá habilitar el parámetro que limita el tiempo de apertura de un Ticket después de su cierre:

    - 171 - Límite de días para la reapertura de Tickets de servicio;

El administrador puede habilitar el parámetro para el envío de correo electrónico específico:

    - 291 - ID de plantilla de correo electrónico enviada al reactivar una solicitud de servicio;

El administrador deberá habilitar los siguientes parámetros para recibir las notificaciones Push:

    - 350 - Habilita el envío de notificaciones para teléfonos;
    - 352 - Habilita el envío de notificaciones para teléfonos durante la creación de solicitudes;
    - 353 - Habilita el envío de notificaciones para teléfonos durante la actualización de solicitudes informando los servicios cercanos;  
    - 460 - Habilita el envío de notificaciones para teléfonos durante la actualización de solicitudes.

## Procedimiento

Abra la aplicación Racer 4biz en el teléfono. Inicie sesión en la aplicación y acceda a los tickets.

### Detalles del ticket

Al acceder a un ticket, tendrá acceso a todos los detalles, acciones e información del ticket elegido. Tenemos la siguiente información:

1. Un símbolo que indica el tipo de ticket;	
2. La situación del ticket;
3. La prioridad del ticket;
4. La tarea del ticket;
5. El grupo actual del ticket;
6. El SLA del ticket;
7. El tiempo límite para la entrega del ticket;
8. El solicitante del Ticket. Se muestra con su avatar, su nombre y su teléfono. 
Al seleccionar el solicitante, se abre una pantalla con una flecha para volver y la siguiente información:

       - El avatar del solicitante;
       - El nombre del solicitante;
       - El Símbolo y el nombre llamada, que al ser seleccionado redirecciona el teléfono para realizar una llamada al número registrado;
       - El Símbolo y el nombre Mensaje, que al ser seleccionado redirecciona el teléfono para enviar un mensaje al número registrado;
       - El Símbolo y el nombre Correo electrónico, que al ser seleccionado redirecciona el teléfono para enviar un Correo electrónico al correo electrónico registrado;
       - El teléfono del solicitante; 
       - El correo electrónico del solicitante;
       - La dirección del solicitante.

9. El responsable del Ticket. Se muestra con su avatar, su nombre y su teléfono. Al seleccionar el responsable se abre una pantalla con una flecha para volver y la siguiente información:

       - El avatar del responsable;
       - El nombre del responsable;
       - El Símbolo y el nombre llamada, que al ser seleccionado redirecciona el teléfono para realizar una llamada al número registrado;
       - El Símbolo y el nombre Mensaje, que al ser seleccionado redirecciona el teléfono para enviar un mensaje al número registrado;
       - El Símbolo y el nombre Correo electrónico, que al ser seleccionado redirecciona el teléfono para enviar un Correo electrónico al correo electrónico registrado;
       - El teléfono del responsable; 
       - El correo electrónico del responsable;
       - La dirección del responsable.

10. La descripción del ticket;
11. Lugar de destino: Muestra el nombre de la ubicación seguido de un mapa con la ubicación de la unidad del solicitante del ticket;
12. Formulario de seguimiento: Al ser seleccionado, se abre una pantalla con una flecha para volver con el Título: Cuestionario y número de ticket abierto. La existencia de un cuestionario será definida por el administrador en la aplicación a través de la configuración del portafolio o del flujo. Si hay formulario, las preguntas se definirán por el administrador del contrato y se llenarán durante el servicio del ticket;

        - Respuestas del formulario de creación: Esta función puede contener las respuestas del formulario de creación.

13. Adjunto. Al ser seleccionado, se abre una pantalla con una flecha para volver con el Título: Adjuntos.

    !!! note "NOTE"
    
       Si aún no hay ningún archivo adjunto insertado en el ticket:  
        
            - Aparecerá un mensaje: No se ha agregado ningún archivo adjunto;
            - Un botón Añadir archivo adjunto. Que cuando se selecciona, se abre una opción para seleccionar el archivo deseado en el teléfono. Al seleccionar el archivo, se muestra el mensaje: ¡Nuevo Adjunto añadido con éxito! Y el Botón de Ok.
            
        Si se ha añadido un archivo adjunto al ticket:
        
            - La aplicación mostrará la cantidad de archivos adjuntos;
            - Al seleccionar la pestaña Archivos adjuntos, se mostrará el nombre del archivo adjunto;
            - Un botón con 3 puntitos que, al ser seleccionado, muestra la opción Eliminar adjunto, que al ser seleccionada, muestra una ventana con el Título Eliminar adjunto, el mensaje ¿Está seguro de que desea eliminar este documento adjunto? , el botón Cancelar (que vuelve a la pantalla anterior) y el botón Confirmar (que elimine el archivo adjunto del ticket).
            
            
14. Artículos de conocimiento. Al ser seleccionado, se abre una pantalla con flecha para volver con el Título: “Conocimiento” y una Lupa que, al ser seleccionada, abre un campo de búsqueda que permite introducir el nombre a buscar en la base de conocimientos.

        - La búsqueda se realiza mediante el título del archivo adjunto o mediante la parte del contenido del conocimiento;
        - Para que la aplicación enumere correctamente los conocimientos, asegúrese de que la indexación de la base de conocimientos esté actualizada en la aplicación;
        - Si el ticket no tiene ningún conocimiento vinculado, se mostrará el mensaje: El ticket seleccionado no tiene ningún conocimiento vinculado a él. Y el botón OK.
        - Se presentará el Título: Base de Conocimientos y una lista con los conocimientos. Cada elemento de la lista tendrá: El autor; El nombre del conocimiento; La descripción del conocimiento; Un botón para Vincular el conocimiento si no está vinculado al ticket; Un símbolo de vinculado y un botón para Desvincular si está vinculado al ticket.

15. Portafolio de servicios y contrato. Al ser seleccionado, se abre una pantalla con flecha para volver, con el Título: Portafolio/contrato y la siguiente información:

        - Una caja con el Título: Portafolio y el nombre del portafolio; 
        - Una caja con el Título: Servicio y el nombre del servicio;
        - Una caja con el Título: Actividad y el nombre de la actividad;
        - Una caja con el Título: Contrato y la descripción del contrato;

16. Comentarios. Al ser seleccionado, se abre una pantalla con flecha para volver con el Título: Comentarios y la siguiente información:

    1. Si no hay ningún comentario, aparecerá el siguiente mensaje: No hay comentario y el botón Ok;
    
       En la pantalla aparecerá el mensaje: No hay ningún comentario en la lista y un botón: Agregar comentario. Al seleccionar el botón, se abrirá una nueva pantalla con flecha para volver, Título Agregar comentario y la siguiente información:
       
           - Clave para seleccionar si el campo es Público;
           - Al seleccionar esta opción, el autor del comentario permite la visualización por parte del solicitante;
           - Clave para seleccionar si es para enviar el comentario por correo electrónico;
           - El envío de correo electrónico depende de la correcta parametrización de la aplicación;
           - Cuadro para introducir el comentario;
           - Título: Lanzar horas (opcional);
           - Campo para seleccionar la fecha, que abre un calendario;
           - Campo para introducir la hora;
           - Botón Enviar;
            Si el campo comentario no se ha rellenado, se muestra un mensaje: Debe introducir una descripción para el comentario. Y el botón Ok.
            Si todo es correcto, se agrega el comentario y se muestra el mensaje: Comentario enviado con éxito. Y el botón Ok que vuelve a la pantalla anterior; 

    2. Si hay comentarios, se mostrará la lista de comentarios de la siguiente manera:  
    
           - Nombre del autor del comentario;
           - El comentario;
           - Fecha y hora del comentario;
           - Botón Responder, que abre la misma pantalla de añadir comentario;
           - Botón 3 puntitos, con las opciones de Editar (abre la misma pantalla de añadir comentario, pero con la información del comentario rellenada) y Eliminar comentario (muestra un mensaje: ¿Está seguro de que desea eliminar este comentario? Y una opción para Cancelar y otra para Confirmar);
           - Botón con signo +, que abre la pantalla de añadir comentario;
           
17. Historial del Ticket. Cuando se selecciona, se abre una pantalla con flecha para volver, Título: Historial del Ticket y una lista con la siguiente información:

        - Fecha del cambio;
        - Nombre de quien hizo el cambio;
        - Hora del cambio;
        - IP de la máquina que hizo el cambio;
        - La acción se ha ejecutado en el cambio;
        - El detalle del cambio;

18. Acción. Al ser seleccionado, se abre una pantalla con flecha para volver, Título: Acción y la siguiente información:

    1. Campo para seleccionar la Acción, que puede ser: Aprobar Ticket o Rechazar Ticket;
    
           - Las acciones presentadas dependen del diseño de flujo determinado para la actividad creada.
           
19. Título: Dirigir a Grupo, seguido de un campo para selección con el Título: Seleccionar grupo, que al ser seleccionada presenta una lista con todos los grupos registrados;
20. Botón: Guardar y Salir, que al ser seleccionado presenta un cuadro con el Título: ¿Desea guardar y salir?, el Mensaje: Todos los cambios se guardarán y volverá a la pantalla de lista. Y los botones Atrás y Guardar y Salir;
21. Botón: Guardar y Siguiente, que al ser seleccionado presenta un cuadro con el Título: Éxito, el Mensaje: Avanzado para la siguiente etapa y el botón OK.


## Trabajando en el ticket

Para acceder a las posibilidades de acciones dentro de un ticket en la aplicación, seleccionaremos uno de los tickets en la cola. Para las siguientes acciones abordaremos el caso de un ticket **en marcha**.

### Capturar ticket

!!! warning "ATENCIÓN"

    Para capturar un ticket, debe estar abierto y verificado. El usuario puede registrarse en más de un ticket. Mostraremos más adelante en este documento cómo realizar el check-in.
    
1. Al hacer clic en un ticket de la lista, se mostrará la pantalla con los detalles de esta solicitud. En la parte superior de la pantalla, hay un botón con 3 puntos donde se mostrarán las opciones del ticket.  
2. Seleccione "Capturar Ticket".  
3. Al seleccionar esta opción, se abrirá un pop-up con el mensaje: Capturar ticket número #0000. Puede cancelar la captura, así volverá a la pantalla del ticket seleccionado, o puede confirmar la captura y guardar esta información. El ticket estará entonces bajo su responsabilidad.  

!!! note "NOTA"

        El usuario puede capturar más de un ticket a la vez.

### Suspender ticket

!!!note "NOTA""

        Para hacer efectiva la suspensión, el usuario deberá tener permiso para tal acción, además de poseer una justificación de suspensión previamente registrada.

1. Al hacer clic en un ticket de la lista, se mostrará la pantalla con los detalles de esta solicitud. En la parte superior de la pantalla, hay un botón con 3 puntos donde se mostrarán las opciones del ticket.  
2. Seleccione "Suspender Ticket".  
3. Al seleccionar la opción de suspender ticket, se abre una nueva pantalla con los campos:

- Campo para seleccionar justificación;  
- Campo para introducir un comentario.

4. Después de rellenar los campos requeridos, haga clic en Guardar.

!!! warning "ATENCIÓN"

        - Si el campo de justificación no se rellena, se muestra un pop-up con el texto: Por favor, debe seleccionar una justificación para la suspensión del ticket. Ok. No permitiendo guardar la acción y permaneciendo en la misma pantalla.
        - Si el campo de comentario no se rellena, se muestra un pop-up con el texto: Por favor, debe introducir un complemento para la suspensión del ticket. Ok. No permitiendo guardar la acción y permaneciendo en la misma pantalla.  
        - Si todo está correcto, se mostrará un mensaje al final de la pantalla con el texto: Suspensión realizada. Id: 0000000. Botón Ok que vuelve a la pantalla del ticket.
        
### Completar ticket  

1. Al hacer clic en un ticket de la lista, se mostrará la pantalla con los detalles de esta solicitud. En la parte superior de la pantalla, hay un botón con 3 puntos donde se mostrarán las opciones del ticket.  
2. Seleccione "Concluir Ticket".  
3. Al seleccionar la opción de suspender ticket, se abre una nueva pantalla con los campos:

- Campo para seleccionar la causa;  
- Campo para seleccionar la solución. La lista solo se carga después de seleccionar el campo causa;
- Campo opcional para introducir un comentario.

4. Después de rellenar los campos requeridos, haga clic en Guardar.

!!! warning "ATENCIÓN"

        - Si el campo causa no está seleccionado, se muestra un pop-up con el título: Atención. Mensaje: Por favor, seleccione la Causa y botón Ok. No permitiendo guardar la acción y permaneciendo en la misma pantalla.
        - Si el campo solución no está seleccionado, se muestra un pop-up con el título: Atención. Mensaje: Por favor, seleccione la Solución y botón Ok. No permitiendo guardar la acción y permaneciendo en la misma pantalla.
        - Si todo es correcto y la acción está completa, volvemos a la pantalla de ticket con la situación del ticket como completada.
        
### Cancelar ticket        

1. Al hacer clic en un ticket de la lista, se mostrará la pantalla con los detalles de esta solicitud. En la parte superior de la pantalla, hay un botón con 3 puntos donde se mostrarán las opciones del ticket 
2. Seleccione "Cancelar Ticket".  
3. Al seleccionar la opción de cancelar ticket, se abre una nueva pantalla con los campos:

- Campo para seleccionar la causa;  
- Campo para seleccionar la solución. La lista solo se carga después de seleccionar el campo causa;
- Campo opcional para introducir un comentario.

4. Después de rellenar los campos requeridos, haga clic en Guardar.

!!! warning "ATENCIÓN"

        - Si el campo causa no está seleccionado, se muestra un pop-up con el título: Atención. Mensaje: Por favor, seleccione la Causa y botón Ok. No permitiendo guardar la acción y permaneciendo en la misma pantalla.
        - Si el campo solución no está seleccionado, se muestra un pop-up con el título: Atención. Mensaje: Por favor, seleccione la Solución y botón Ok. No permitiendo guardar la acción y permaneciendo en la misma pantalla.
        - Si todo es correcto y la acción está completa, volvemos a la pantalla de ticket con la situación del ticket como cancelada.
        
### Realizar check-in        

El check-in es el medio utilizado para identificar el camino recorrido para el servicio de un ticket abierto de Solicitud/Incidente. Para utilizarlo es necesario que el usuario haya habilitado la opción disponible para el servicio.

!!! note "NOTA"

       El check-in no es obligatorio para el servicio del ticket por parte del agente

	Al seleccionar la opción realizar check-in, se muestra un pop-up con el mensaje: "¿Está seguro de que desea realizar check-in en este ticket?". Si desea continuar con el check-in, haga clic en "Guardar". Si desea cancelar el check-in, haga clic en "Cancelar".

### Realizar check-out

El check-out es el medio utilizado para identificar el cierre del camino recorrido para el servicio de un ticket abierto de Solicitud/Incidente. Para usarlo, es necesario que el agente tenga permiso de ejecución en el ticket.

!!! note "NOTA"

        El check-out (desbloqueo) no es obligatorio para el cierre del servicio del ticket por parte del agente
        
!!! note "NOTA"

        Si es necesario, un asistente con acceso a la aplicación web podrá realizar el check-out (desbloqueo) del servicio
        
 	Al seleccionar la opción realizar check-out, se muestra un pop-up con el mensaje: "¿Está seguro de que desea realizar check-out en este ticket?". Si desea continuar con el check-out, haga clic en "Guardar". Si desea cancelar el check-out, haga clic en "Cancelar".
 
### Asignar ticket

1. Al hacer clic en un ticket de la lista, se mostrará la pantalla con los detalles de esta solicitud. En la parte superior de la pantalla, hay un botón con 3 puntos donde se mostrarán las opciones del ticket.  
2. Seleccione "Asignar Ticket".  
3. Al seleccionar la opción de cancelar ticket, se abre una nueva pantalla con los campos:

- Campo para seleccionar el usuario;  
- Campo para seleccionar el grupo;  
- Campo para introducir una justificación.

4. Después de rellenar los campos requeridos, haga clic en Guardar.

!!! warning "ATENCIÓN"

        - Si el campo de solución no está seleccionado, se muestra un pop-up con el Texto: Por favor, seleccione el grupo para la asignación del ticket y el botón Ok. No permitiendo guardar la acción y permaneciendo en la misma pantalla. 
        - Si el campo de justificación no se rellena, se muestra un pop-up con el Texto: Por favor, introduzca una justificación para la asignación del ticket y el botón Ok. No permitiendo guardar la acción y permaneciendo en la misma pantalla. 
        - Si todo es correcto, se muestra un mensaje al final de la pantalla con el texto: Asignación realizada con éxito. Botón Ok que vuelve a la pantalla del ticket. 
        
### Reclasificar ticket

1. Al hacer clic en un ticket de la lista, se mostrará la pantalla con los detalles de esta solicitud. En la parte superior de la pantalla, hay un botón con 3 puntos donde se mostrarán las opciones del ticket.  
2. Seleccione "Reclasificar Ticket".  
3. Al seleccionar la opción de reclasificar ticket, se abre una nueva pantalla con los campos:

- Campo para seleccionar portafolio;  
- Campo para seleccionar servicio. La lista solo se carga después de seleccionar el campo de portafolio;  
- Campo para seleccionar actividad. La lista solo se carga después de seleccionar el campo servicio;  
- Campo para seleccionar contrato. La lista solo se carga después de seleccionar el campo actividad;  
- Campo para introducir justificación.

!!! note "NOTA"

        - Si uno de los campos no está lleno, se muestra un pop-up con el Texto: ¡Atención! La Actividad y el Contrato deben seleccionarse y el botón Ok. No permitiendo guardar la acción y permaneciendo en la misma pantalla. 
        - Si el campo de justificación no se rellena, se muestra un pop-up con el Texto: Por favor, debe proporcionar una justificación para la Reclasificación del ticket y botón Ok. No permitiendo guardar la acción y permaneciendo en la misma pantalla. 
        - Si todo es correcto, se muestra un pop-up con el Texto: ¿Desea seguir siendo responsable del ticket? Y los botones No y Sí. Si el botón No está seleccionado, la aplicación permanece en la misma pantalla.  
        - Si se selecciona el botón Sí, aparecerá un mensaje al final de la pantalla con el texto: Ticket reclasificado con éxito. Botón Ok que vuelve a la pantalla del ticket.
        
!!! warning "ATENCIÓN"

        - El grupo de usuario debe tener permiso para reclasificarse en el flujo de la actividad;  
        - El ticket a reclasificar debe estar en la situación Abierto o En Progreso.
        
### Reabrir ticket

Si el ticket ya está cerrado, tendrá la opción de volver a abrirlo a través del botón de 3 puntitos del ticket, donde aparecerá la opción "Reabrir ticket".

!!! note "NOTA"

    - La aplicación no muestra la opción de reapertura en dos casos: cuando el usuario no tiene permiso en el flujo para reabrir el ticket y cuando haya expirado el plazo límite para la reapertura del ticket.  
    - El ticket debe estar cerrado.  
    - No se permite reabrir un ticket con la situación Cancelado.
    
Al seleccionar la opción de reabrir ticket se abre una nueva pantalla con:  

- Campo para introducir motivo de reapertura;  
- Botón de "Reabrir".

!!! note "NOTA"

    - Si el campo no se rellena, se muestra un pop-up con el Texto: Debe indicar un motivo para la Reapertura del ticket y botón Ok.  
    - Si todo es correcto, se muestra un mensaje al final de la pantalla con el texto: Reapertura realizada. ID 0000. Botón Ok que vuelve a la pantalla del ticket.
    
### Evaluar servicio

Si el ticket ya está cerrado, puede evaluar el servicio solicitado.
!!! note "NOTA"

    - El ticket debe estar cerrado;  
    - El ticket no podrá haber sido cancelado.
    
Hay dos tipos de evaluación de servicio:  

1. Predeterminado - Configurando en el servicio x contrato el campo Correo electrónico de Finalización = Solicitud Atendida (ID2 del modelo de correo electrónico).
   - La opción Predeterminado permite reabrir el ticket por la encuesta de satisfacción, configurando el parámetro: 295 - Reabrir Solicitud mediante la Encuesta de Satisfacción (Valores posibles: S o N, Default: N);
   - Configurar el parámetro 139 - Plazo en días para responder la encuesta de satisfacción referente a las solicitudes de servicio (Ejemplo: 7) con la cantidad de días para responder a la encuesta de satisfacción después del cierre del servicio.  
   
2. Por el registro de encuesta - Registrando una encuesta del tipo Actividad/Satisfacción y vinculando la encuesta a una actividad. El registro de la encuesta tiene fecha de finalización, por lo tanto, el parámetro 139 no se tiene en cuenta en este caso.

Al seleccionar la opción de evaluar el servicio, se abre una nueva pantalla con:  
-  4 caritas que representan una escala de muy insatisfecho hasta muy satisfecho. Las caritas son del tipo botones para ser seleccionados y, al hacer clic, cada una presenta un nombre;  
- Campo para introducir comentario.  
    
Si todo está bien, haga clic en "Enviar evaluación". La evaluación se envía y vuelve a la pantalla del ticket.  

### Reactivar ticket

Si un ticket está suspendido, puede reactivarlo para poder realizar las acciones normales de un ticket.  
Para ello, encuentre el ticket y presione el botón con 3 puntitos y seleccione la opción "Reactivar ticket".  
Al seleccionar la opción reactivar ticket, se muestra un pop-up con el Título: "Reactivar ticket #00000". Tiene la opción de confirmar o cancelar la reactivación.  
Una vez reactivado, tendrá las acciones disponibles para el tratamiento de la solicitud en cuestión.
