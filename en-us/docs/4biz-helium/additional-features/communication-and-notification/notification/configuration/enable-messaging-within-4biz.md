title: Configuring messaging within 4biz
Description: It provides a communication channel between the requester (Smart Portal) and the technician (service/ticket request area) through message (email).
# Configuring messaging within 4biz

4biz provides a communication channel between the requester (Smart Portal)
and the technician (service/ticket request area) through message (email). This
communication aims to facilitate the resolution of a ticket. This knowledge
gathers information pertinent to the configuration of the messaging service.


Before getting started
--------------

It is necessary to configure the email account (SMTP) beforehand (check related item).

Procedure
-------------

1.  In order for the messaging service to be available within 4biz, it is
    necessary to set the parameter 417 with the ID number of the email template
    that has some variables to be sent to the messaging;

2.  Below are the keys for sending email:

    - \${IDSERVICEREQUEST} - Number of the ticket (public key);

    - \${COMMENTTEXT} - Description of the comment made on the messaging;

    - \${DATETIMECREATED} - Date the comment was registered;

    - \${USERNAME} - Name of user that made the comment;

    - \${REQUESTERNAME} - Name of the requester;

    - \${REQUESTRESPONSIBLENAME} - Name of the technician responsible for the
      ticket attendance.

Related
-------

[Configure email account](/en-us/4biz-helium/platform-administration/email-settings/configuration.html)

[The desktop of Service Desk](/en-us/4biz-helium/processes/tickets/use/desktop-of-service-desk.html)

[Configure parametrization – ticket](/en-us/4biz-helium/platform-administration/parameters-list/configure-parametrization-ticket.html)

[Configure email template](/en-us/4biz-helium/platform-administration/email-settings/email-templates-configure-email-template.html)

[Manage my requests through Smart Portal](/en-us/4biz-helium/processes/portfolio-and-catalog/use/request-through-Smart-Portal.html)


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021
