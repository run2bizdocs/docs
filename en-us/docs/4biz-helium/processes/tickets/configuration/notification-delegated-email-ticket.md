title: Notification through delegated email ticket
Description: Implement the way of sending email from a delegated ticket, so the delegated tickets will have an email template to send to the technician. 

# Notification through delegated email ticket

This feature allows to define and select a template for the notification emails to technicians receiving a delegated ticket.

## Before getting started

An email template must have been previously registered and, the recommended keys to use in the body are the following:

```html
${IDSERVICEREQUEST}

${SERVICENAME}

${REQUESTERNAME}

${DESCRIPTION}
```

**Procedure**

1.	Access the functionality through the main menu Processes > Portfolio and Catalog Management > Portfolio;

2.	Choose a portfolio and click on "Advance";

3.	Choose a service and click on "Advance";

4.	Click on Contracts;

5.	Select the contract and click on "Advance";

6.	Click on the tab Requests and click on "Edit";

7.	Choose the activity;

8.	In the field Email Template Delegation choose by the previously registered e-mail template;

9.	Click on "Save";

10.	In the parametrization screen, enable the parameters 438 (inform email template for delegation) and 439 (option "YES");

11.	In the group registration screen, in the field "Employees", select the checkbox "Email" for the people that will receive the email of that group.

## What to do next

Access a ticket and delegate it.

Related
-------

[Delegate ticket](/en-us/4biz-helium/processes/tickets/use/delegate-ticket.html)

[Configure email template](/en-us/4biz-helium/platform-administration/email-settings/email-templates-configure-email-template.html)

[Register group](/en-us/4biz-helium/initial-settings/access-settings/user/register-groups.html)



!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
