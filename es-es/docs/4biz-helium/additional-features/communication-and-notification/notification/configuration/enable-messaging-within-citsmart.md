title: Configurar la mensajería dentro del 4biz
Description: Ofrece un canal de comunicación entre el solicitante (Smart Portal) y el técnico (área de solicitud de servicio/ticket) vía mensaje (correo electrónico).
# Configurar mensajería dentro del 4biz

4biz ofrece un canal de comunicación entre el solicitante (Smart Portal) y
el técnico (área de solicitud de servicio/ticket) vía mensaje (correo
electrónico). Esta comunicación tiene por objeto facilitar la resolución de un
ticket. Este conocimiento reúne información pertinente a la configuración del
servicio de mensajería.


Antes de empezar
--------------

Es necesario configurar la cuenta de correo electrónico (SMTP) de antemano (ver elemento relacionado).

Procedimiento
-----------------

1.  Para que el servicio de mensajería esté disponible dentro del 4biz, es
    necesario establecer el parámetro 417 con el número del ID de la plantilla de
    correo electrónico que contenga algunas variables para poder ser enviado a
    mensajería;

2.  A continuación se enumeran las claves para el envío de correo electrónico:

    -  \${IDSOLICITUDSERVICIO} - Número del ticket (clave pública);

    -  \${COMMENTTEXT} - Descripción del Comentario hecho en la mensajería;

    -  \${DATETIMECREATED} - Fecha en que se registró el comentario;

    -  \${USERNAME} - Nombre de usuario que ha introducido el comentario;

    -  \${REQUESTERNAME} - Nombre del solicitante;

    -  \${REQUESTRESPONSIBLENAME} - Nombre del técnico responsable por el servicio
         del ticket.


Relacionado
-------

[Configurar cuenta de correo electrónico](/es-es/4biz-helium/platform-administration/email-settings/configuration.html)

[La área de trabajo del service desk](/es-es/4biz-helium/processes/tickets/use/desktop-of-service-desk.html)

[Configurar parametrización - ticket](/es-es/4biz-helium/platform-administration/parameters-list/configure-parametrization-ticket.html)

[Configurar modelo de email](/es-es/4biz-helium/platform-administration/email-settings/email-templates-configure-email-template.html)

[Gestionar mis solicitudes por el Smart Portal](/es-es/4biz-helium/processes/portfolio-and-catalog/use/request-through-Smart-Portal.html)


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
