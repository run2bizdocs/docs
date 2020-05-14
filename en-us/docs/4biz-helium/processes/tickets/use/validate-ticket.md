title: Validate and close the ticket
Description: After attend the ticket, its execution should be validated and the ticket closed.

# Validate and close the ticket
After attend the ticket, its execution should be validated and the ticket closed.

Before getting started
--------------------------

It's necessary to previously register the ticket and have permission to validate
it.

Procedure
-------------

1.  Access the functionality Ticket Management through the main menu Processes
    \> Ticket Management \> Ticket;

2.  Click on the ticket you want and then in the icon “Open”;

3.  Certify the ticket attendance was done according to what was requested;

4.  In the "Status" area, choose the option "Solved", complete the data to close
    the ticket;

    - If the type of request is "Incident":
    
         * Solution Category: select the category of the incident solution;
         
         * Cause Detail: describe the details of the incident cause;
         
         * Answer Solution: describe the details of the solution made to the 
           incident attendance;
         
         * Save Solution/Answer in the Knowledge Base: in order to the checkbox "Save Solution/Answer 
           in the Knowledge Base" is visible, check the parametrization of the Knowledge Management process;

        !!! abstract "NOTE"
        
            To reduce the options for the "Cause" and "Solution Category" fields, presented when closing the ticket,  
            the tool provides the Cause and Solution Category link to specific services.
            For this, it's necessary to create a "Cause", where is possible to link to other related causes. It's 
            also necessary to create the "Solution Category", where is possible to link a cause and depending on it, 
            it will bring all the causes related to the main one
            Then, in Service Portfolio you want, you will link the Causes and Solution Category in the service you 
            find most appropriate.
            When executing the ticket, completing the closing fields, the options for "Cause" and "Solution Category" 
            will be in accordance with what was linked to the service within the Portfolio, reducing so the options 
            available, focusing only on the necessary
         
        !!! Abstract "ATTENTION"
           
             In order for the "Save Solution / Knowledge Base Answer" option to be available by 
             checking the "Resolved" option of the ticket, it is necessary to configure parameters 
             182 and 192.
             
           
         * Justification of SLA expired: the visibility of this field is conditioned to the SLA 
           status expired for the attendance question;
           
         * Temporary Solution: indicate if the activity performed to attend the incident was a temporary solution.
         
    - If the type of request is "Request", complete the field ""Answer Solution"", describe what 
      was made to attend the service request. 
      
    !!! Abstract "ATTENTION"
    
        The steps to solve the Ticket steps can be the suggestion of a new knowledge, being evaluated 
        beforehand to be effective. It is also possible to suggest a name for this new knowledge in the 
        field "Knowledge Base Title".

5.  Click on the "Option" button and definy the next step:

    -  "Save changes";
    
    -  "Send ticket".

Related
-----------

[Register group](/en-us/4biz-helium/initial-settings/access-settings/user/register-groups.html)

[The desktop of Service Desk](/en-us/4biz-helium/processes/tickets/use/desktop-of-service-desk.html)

[Create ticket](/en-us/4biz-helium/processes/tickets/use/create-ticket.html)

[Configure access permission of request/incident management](/en-us/4biz-helium/processes/tickets/configuration/access-ticket-management.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RNrJnhiXj3dbmgsm9-quhfz)'

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
