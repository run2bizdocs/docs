title: Validar y cerrar ticket
Description: Después de la atención del ticket, su ejecución deberá ser validada y el ticket encerrado.

# Validar y cerrar ticket

Después de la atención del ticket, su ejecución deberá ser validada y el ticket encerrado.

Antes de empezar
----------------

Es necesario el registro previo del ticket y tener permiso para validarlo.

Procedimiento
-------------

1.  Acceder a la funcionalidad por el menú principal Procesos \> Gestión de
    Ticket \> Ticket;

2.  Buscar el ticket deseado, seleccionarlo y hacer clic en el icono “Abrir”;

3.  Certificar si la atención del ticket fue realizada de acuerdo con lo que se
    solicitó;

4.  En el area de "Estado", elegir la opción "Resuelta", completar los datos para
    cerrar el ticket;
    
     - Si el tipo de solicitud es "Incidente":
    
       * Categoría de Solución: seleccionar la categoría de solución del incidente;
         
       * Detalle de la Causa: describir los detalles de la causa del incidente;
         
       * Solución Respuesta: describir los detalles de la solución que se realizó 
         para atender el incidente;
         
       * Guardar Solución/Respuesta en la Base de Conocimiento: para que el checkbox 
         "Guardar Solución/Respuesta en la Base de Conocimiento" sea visible, verificar 
         la parametrización del proceso de Gestión del Conocimiento;
         
        !!! abstract "NOTE"
        
            Para reducir las opciones en los campos "Causa" y "Categoría de solución", presentados al cerrar el ticket,  
            la herramienta proporciona el enlace de Causa y Categoría de Solución a servicios específicos.
            Para esto, es necesario crear una "Causa", donde es posible vincular a otras causas relacionadas. Tambien   
            es necesario crear la "Categoría de solución", donde es posible vincular una causa y, dependiendo de ella,  
            traerá todas las causas relacionadas con la causa principal.
            Después, en el Portafolio de servicios que quieras, vinculará las Causas y la Categoría de solución en el  
            servicio que te parece más apropiado.
            Al ejecutar el ticket, al describir los campos de cierre, las opciones para "Causa" y la "Categoría de solución"  
            estará de acuerdo con lo que estaba vinculado al servicio dentro del Portafolio, reduciendo entonces las opciones  
            disponibles, enfocándose solo en lo necesario.        
           
        !!! Abstract "ATENCIÓN"
         
            Para que la opción "Guardar solución/Respuesta en la Base de Conocimiento" 
            esté disponible al marcar la opción "Resuelta" del ticket. Es necesario 
            configurar los parámetros 182 y 192.
    
    
       * Justificación del SLA expirado: la visibilidad de este campo está condicionada 
         al status de SLA caducado para la atención en cuestión;
           
       * Solución Temporal: indicar si la actividad realizada para atender el incidente 
         fue una solución temporal. 
       
    
     - Si el tipo de solicitud es "Solicitud", completar el campo "Solución Respuesta", 
      describir lo que se realizó para atender la solicitud de servicio.
      
    !!! Abstract "ATENCIÓN"
    
        Los pasos de resolución del Ticket pueden ser la sugerencia de un nuevo conocimiento, 
        siendo evaluado previamente para efectividad. Es posible sugerir también un nombre para 
        este nuevo conocimiento en el campo "Título Base de Conocimiento".
    
5.  Haga clic en "Opciones" y definir el paso siguiente de la solicitud:

     -   "Guardar cambios";
     
     -   "Enviar ticket".
   

Relacionado
-----------

[La área de trabajo del service desk](/es-es/4biz-helium/processes/tickets/use/desktop-of-service-desk.html)

[Crear ticket](/es-es/4biz-helium/processes/tickets/use/create-ticket.html)

[Registrar grupo](/es-es/4biz-helium/initial-settings/access-settings/user/register-groups.html)

[Configurar permiso de acceso de la gestión de solicitudes/incidentes](/es-es/4biz-helium/processes/tickets/configuration/access-ticket-management.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROfIFL9F-3s-gomHNzudBEy)'

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
