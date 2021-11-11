Title: Ticket status on Racer 4biz  
Description: We will see the possible actions that can be done in ticket attendance.

# Ticket Status on Racer 4biz  

This document will show the possible actions to be taken in ticket attendance when using Racer 4Biz app.  

## Before getting started

- [x] Install the app Racer 4biz for Android or IOS  
- [x] Have valid access credentials to the system

It is also necessary to configure the parameters:

- [x] 254 - API Key for use of Google services; 
- [x] 331 - Enable Google Maps API; 
- [x] 436 - Project number (Sender ID) in Google Cloud Platform used to generate API keys (Mobile SM only).   

Besides, it is also necessary to configure the 4biz Webservice, Unit and Tickets platforms.

**Webservice**

Access the function through Main Navigation Menu > System > Webservice > Webservice Operation.  

On the Operation Search tab, search for each one of the webservices below. Next, click on the button "Add to group" on each one of them and include the groups the agents are linked to:

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
    - notification_checkin
    - notification_attendRequest
    - notification_checkout
    - service_deviceDisassociate
    - notification_locationTrack 
    
The webservice request_updateStatus must be configured with the following information:
    
    - Default ID for justification of the alteration of the request;
    - Add groups with permission to change ticket status;

Click the "Save" button after the configuration is done.

**Unit**

Access the functionality through Main Navigation Menu > General Registration Acessar a funcionalidade através do menu principal Cadastros Gerais > Personnel Management > Unit.  
Search for the unit using the Unit Search tab and select the proper one.  
Go to the Unit Registration tab of the chosen unit and click "Get Coordinates"  
Click "Save".

**Tickets**

It is necessary to have permission to view, capture and perform actions on the tickets.  
To reclassify a ticket, the user must be a part of an executor group, on the group screen the flow must be linked to the option "Change SLA", and must also have permission to "Create" in the flow of the target activity. This is necessary if the reclassification needs to include a different flow.  
The group must have permission to suspend the ticket.  
The administrator can enable the email sending parameter:

    - 290 - Email template ID sent when suspending a service request

The administrator can enable the requirement of the complement for suspention fieldO administrador poderá habilitar a obrigatoriedade do campo para complemento da suspensão:

    - 372 - Enable mandatory fulfillment when suspending request

The administrator must have registered the Solicitation Justification to suspend the ticket.
The administrator mus enable the parameter that limits the period to reopen a ticket after it's closed:

    - 171 - Days limit for reopening of services Tickets.;

The administrator can enable the parameter to send specific emails:

    - 291 - Email template ID sent when reactivating a service request;

The administrator must enable the following parameters to receive Push notifications:

    - 350 - Enable sending notifications to mobile devices;
    - 352 - Enables sending notifications to mobile devices when creating requests;
    - 353 - Enables sending mobile notifications while updating requests reporting close calls;  
    - 460 - Enables sending mobile notifications while updating requests.

## Procedure

Open the app Racer4biz. Login and access the tickets.

### Ticket Details

By accessing a ticket, you will have access to all the details, actions and information of the selected ticket. We have:

1. A symbol informing the type of ticket;	
2. The ticket status;
3. The ticket priority;
4. The current task;
5. The current group;
6. The SLA;
7. The time limit to finish the attendance;
8. The solicitor, shown with their avatar, name and phone number. By selecting the solicitor you will see a screen with the following information:

       - The solicitor's avatar;
       - Their name;
       - The Call symbol, which will redirect the user to the calling screen of the smartphone when selected;
       - The Message symbol, which will redirect the user to the message screen of the smartphone when selected;
       - The Email symbol, which will redirect the user to the email screen of the smartphone when selected;
       - The solicitor's phone number;
       - Their email;
       - Their address.

9. The assigned agent, shown with their avatar, name and phone number. By selecting the responsável???? you will see a screen with the following information:

       - O avatar do responsável;
       - O nome do responsável;
       - O Símbolo e o nome chamada, que ao ser selecionado redireciona o celular para realizar uma chamada para o número cadastrado;
       - O Símbolo e o nome Mensagem, que ao ser selecionado redireciona o celular para enviar uma mensagem para o número cadastrado;
       - O Símbolo e o nome E-mail, que ao ser selecionado redireciona o celular para enviar um E-mail para o e-mail cadastrado;
       - O Telefone do responsável;
       - O e-mail do responsável;
       - O endereço do responsável.

10. The ticket description;
11. Destination????: Shows the name of the location as well as a map with the location of the unit;
12. Monitoring survey: By selecting it, a screen is shown with the title of the survey and the number of the ticket. The existance of the survey is defined by the administrator when configuring the portfolio or the workflow. Should there be a survey, the questions will be defined by the administrator of the contract and answered during the attendance;

        - Answers of the creation survey: This function can have the answers of the creation survey.

13. Attachment. By selecting this, a screen named Attachments is shown.

    !!! note "NOTE"
    
        If the ticket has no attachments:  
        
            - A message will appear: No attachments added;
            - A button to add attachments will appear. Clicking it will allow the option to choose a file from the smartphone. After selecting the file a message will appear: New attachment added successfully!
            
        If the ticket has attachments:
        
            - The app will show the amount of attachments;
            - By selecting the attachment tab the name of the attachments will be shown;
            - The ... button, when selected, will give you the option to delete attachments. when selecting it, a message will appear: Are you sure you want to delete the attached file? along with the Cancel and Confirm buttons.
            
            
14. Knowledge articles. By selecting this, a screen named Knowledge will be shown, with a magnifier icon. By selecting the icon, a search field will appear, allowing the search of terms from the knowledge database.

        - The search is made by the title of the attachment or part of the content;
        - In order for the app to properly list the knowledge articles, make sure that the database is correctly indexed on the app;
        - If the ticket has no linked knowledge, a message will appear: The selected ticket doesn't have any linked knowledge????? and the OK button
        - A list with articles named Knowledge Database will appear. Each item on the list will have: The author; the title; the description; a button to link knowledge, if it is not linked to the ticket; a link symbol; the Unlink button, if it is linked to the ticket.

15. Services and contract portfolio. by selecting this, a screen named Portfolio/Contract will appear, containing the following information:

        - A box named Portfolio and the name of the portfolio;
        - A box named Service and the name of the service;
        - A box named Activity and the name of the activity;
        - A box named Contract and the description of the contract;

16. Comments. By selecting this, a screen named Comments will be shown containing the following information:

    1. If there are no comments, a message will appear: "There are no comments", with the OK button;
    
       The screen will have a message saying there are no comments and a button to Add Comment. Clicking the button will show a new screen named Add Comment and the following information:
       
           - Chave??? to select if it's Public; this will allow the solicitor to view comments.
           - Chave to select if the comment should be emailed; This option requires the correct parameters to be configured.
           - Box to type in your comment.
           - Título: Lançar horas (opcional);????
           - Field to select the date, which will open a calendar.
           - Field to select the time.
           - Send button.
            If the Comment field is not filled, a message will appear: Você deve informar uma descrição para o comentário. ????????? and the Ok button.
            If everything is correct the comment is added and a message will appear: Comment added succesfully! with the OK button.

    2. If there are any comments, a list of comments wil be shown, containing:  
    
           - The author's name;
           - The comment;
           - Time and date of the comment;
           - Reply button, which will open the Add Comment screen;
           - The ... button will have a few options: Edit (which will show the Add Comment screen, but with filled information) and Delete (which will show a confirmation message); 
           - The + button, which will open the Add Comment screen;
           
17. Ticket History. By selecting this, a screen named Ticket History will be shown, containing the following information:

        - Date of the change;
        - Name of the author of the change;
        - Time of the change;
        - Ip of the machine that perfomed the change;
        - The action of the change;
        - Details of the change;

18. Action. By selecting this, a screen named Action will be shown, containing the following information:

    1. Field to select the action, that can be Approve Ticket or Refuse Ticket?????;
    
           - The actions shown will be related to the flow design of the activity.
           
19. Direct to Group, followed by a field named Select Group, which will show a list with all the registered groups;
20. Button: Save and Exit. By selecting this a box will pop up asking "Do you wish to save and exit" All the changes will be saved and you will return to the list screen" and buttons Back and Save and Exit;
21. Button Save and Submit. By selecting this a message will apear saying "Success. Advanced to next step" and the OK button.


## Ticket attendance

To access the possible actions inside a ticket, we need to select one of the tickets from the list. For the following actions, we will use a ticket **In progress**.

### Capture ticket

!!! warning "WARNING"

    To capture a ticket, it must be open and checked. The user can check-in to more than one ticket. This document will instruct you on how to check in.
    
1. When you click a ticket from the list, a screen will appear with the request details. On top of the screen, there's a button with 3 dots where the options will be presented.  
2. Select "Capture ticket".  
3. By selecting this option, a pop-up message will appear with the message: Capture ticket number #0000. You can cancel the capture and go back to the ticket screen, or you can confirm and save the information. The ticket will be assigned to you then.  

!!! note "NOTE"

        The user can capture more than one ticket at a time.

### Suspend ticket

!!!note "NOTE"

        To apply the suspension of a ticket, the user must have permission to do this, and also have a proper justification.

1. When clicking a ticket from the list, a screen will appear showing details of the request. On top of the screen, there's a button with 3 dots where the options will be presented.  
2. Select "Suspend Ticket".  
3. When selecting suspend ticket, a new screen with the following options will appear:

- Field to select justification;  
- Field to insert a comment.

4. After filling in the fields, click Save.

!!! warning "Warning"

        - If the justification field is not filled, a pop-up message will appear reading: "You must select a justification for ticket suspension." It is not allowed to save before the action is performed.  
        - If the comment field is not filled, a pop-up message will appear reading: "You must inform a comment for ticket suspension." It is not allowed to save before the action is performed.   
        - If everything is correct, a message will appear saying that the action was performed successfully Id: 0000000. The Ok button will return to ticket screen.
        
### Conclude ticket  

1. When clicking a ticket from the list, a screen will appear showing details of the request. On top of the screen, there's a button with 3 dots where the options will be presented.  
2. Select "Close Ticket".  
3. When selecting close ticket, a new screen with the following options will appear:

- Field to select cause;  
- Field to select solution. This list is only loaded after selecting the cause;
- Optional field to insert a comment.

4. After filling in the required fields, click Save.

!!! warning "Warning"

        - If the cause field is not filled, a pop-up message will appear reading: "You must select a cause to close the ticket." It is not allowed to save before the action is performed.  
        - If the solution field is not filled, a pop-up message will appear reading: "You must inform a solution to close the ticket." It is not allowed to save before the action is performed.   
        - If everything is correct, a message will appear saying that the action was performed successfully Id: 0000000. The Ok button will return to ticket screen.
        
### Cancel ticket        

1. When clicking a ticket from the list, a screen will appear showing details of the request. On top of the screen, there's a button with 3 dots where the options will be presented.  
2. Select "Cancel Ticket".  
3. When selecting cancel ticket, a new screen with the following options will appear:

- Field to select cause;  
- Field to select solution. This list is only loaded after selecting the cause;
- Optional field to insert a comment.

4. After filling in the required fields, click Save.

!!! warning "Warning"

        - If the cause field is not filled, a pop-up message will appear reading: "You must select a cause to cancel the ticket." It is not allowed to save before the action is performed.  
        - If the solution field is not filled, a pop-up message will appear reading: "You must inform a solution to cancel the ticket." It is not allowed to save before the action is performed.   
        - If everything is correct, a message will appear saying that the action was performed successfully Id: 0000000. The Ok button will return to ticket screen.
        
### Perform check-in        

Check-in is a way to identify the path taken when dealing with the attendance of a request/incident ticket. To use this, the user must enable this option for attendance.

!!! note "NOTE"

       Checking-in is not mandatory for ticket attendance 

By selecting the option to check-in, a pop-up message will appear reading "Are you sure you want to check-in this ticket?" If you wish to proceed, click "Save". If you wish to cancel the check-in, click "Cancel".

### Perform checkout

Check-out is a way to identify the end of the path taken when dealing with the attendance of a request/incident ticket. To use this, the user must have permission to execute it.

!!! note "NOTE"

        The checkout is not mandatory for ticket attendance         
!!! note "NOTE"

        If it is necessary, an agent with access to the web application can perform the attendance checkout
        
 By selecting the option to checkout, a pop-up message will appear reading "Are you sure you want to checkout this ticket?" If you wish to proceed, click "Save". If you wish to cancel the checkout, click "Cancel".
 
### Assign ticket

1. When clicking a ticket from the list, a screen will appear showing details of the request. On top of the screen, there's a button with 3 dots where the options will be presented.  
2. Select "Assign Ticket".  
3. When selecting assign ticket, a new screen with the following options will appear:

- Field to select user;  
- Field to select the group;
- Field to insert a justification.

4. After filling in the required fields, click Save.

!!! warning "Warning"

        - If the group field is not filled, a pop-up message will appear reading: "You must select a group to assign the ticket." It is not allowed to save before the action is performed.  
        - If the justification field is not filled, a pop-up message will appear reading: "You must inform a justification to assign the ticket." It is not allowed to save before the action is performed.   
        - If everything is correct, a message will appear saying that the action was performed successfully Id: 0000000. The Ok button will return to ticket screen.

### Reclassify ticket

1. When clicking a ticket from the list, a screen will appear showing details of the request. On top of the screen, there's a button with 3 dots where the options will be presented.  
2. Select "Reclassify Ticket".  
3. When selecting reclassify ticket, a new screen with the following options will appear:

- Field to select portfolio;  
- Field to select the service. This list is only loaded after selecting the portfolio;
- Field to select the activity. This list is only loaded after selecting the service;
- Field to select the contract. This list is only loaded after selecting the service;
- Field to insert a justification.

4. After filling in the required fields, click Save.

!!! note "NOTA"

        - If one of the fields is not filled, a pop-up message will appear reading: "Warning! The activity and contract must be selected!" It is not allowed to save before the action is performed.  
        - If the justification field is not filled, a pop-up message will appear reading: "You must inform a justification to reclassify the ticket." It is not allowed to save before the action is performed.
        - If everything is correct, a message will appear reading: "Do you want to assign the ticket to you?" With the Yes and No buttons. If the No button is clicked, the app will remain on the same screen.  
        - If the Yes button is selected, a message will appear reading: "Ticket reclassified successfully" The Ok button will return to ticket screen.
        
!!! warning "Warning"

        - The user group must have permission to reclassify on the activity flow;  
        - The ticket status must be Open or In Progress.
        
### Reopen ticket

If the ticket is closed, you have the option to reopen it on the 3 dots button and clicking "Reopen ticket".

!!! note "NOTE"

    - The app will not show the reopen option in 2 cases: when the user does not have permission to reopen and when the time limit for reopening is expired.  
    - The ticket must be closed.  
    - It is not allowed to reopen a Canceled ticket.
    
When selecting Reopen Ticket, a new screen with the following options will appear:  

- Field to insert justification for reopening;  
- Reopen button.

!!! note "NOTE"

    - If the field is not filled, a pop-up message will appear reading: "You must inform a justification to reopen the ticket!" It is not allowed to save before the action is performed.
    - If everything is correct, a message will appear saying that the action was performed successfully Id: 0000000. The Ok button will return to ticket screen.
    
### Evaluate attendance    

If the ticket is closed, you can evaluate the attendance of the requested service.

!!! note "NOTE"

    - The ticket must be closed;  
    - The ticket must not be canceled.
    
There are two types of attendance evaluation:  
1. Default – Configuration on service x contract the field Finalization E-mail = Request answered (ID2 of the email model).  
   - The default option allows that the ticket is reopened by the satisfaction survey, by configuring the parameter 295 - Reopen Request by Satisfaction Survey (Possible values: Y or N, Default: N);  
   - Configuring the parameter 139 - Deadline in days to respond to a satisfaction survey regarding service requests (Eg. 7) with the amount of days to answer the satisfaction survey after the service is finished.  
   
2. Through survey register - Registering a survey of the Activity/Satisfaction type and linking the survey to an activity. The register of the survey has a limit date, so the parameter 139 is not considered.    

By selecting the option to evaluate the attendance, a new screen will appear with:  
-  4 faces corresponding to a scale of very satisfied to very unsatisfied. The faces are buttons that can be selected and, by clicking them, they will show a name;  
- Field to insert comment.  
    
If everything is correct, click "Finish survey". The survey will be sent and you will return to the ticket screen.  

### Reactivate ticket

If a ticket is suspended, you can reactivate it and perform the regular actions of the flow.  
To do this, click the 3 dots button and select "Reactivate ticket".  
When selecting this option, a pop-up message will appear reading: Reactivate ticket #00000". You can confirm or cancel the reactivation.  
Once reactivated, you have the same regular options to deal with the request.


## Related

[Filter – all tickets](/en-us/4biz-helium/additional-features/racer-4biz-app/all-tickets-filter.html)

[Filter - my tickets](/en-us/4biz-helium/additional-features/racer-4biz-app/my-tickets-filters.html)

[Racer 4biz – Homescreen](/en-us/4biz-helium/additional-features/racer-4biz-app/racer-homescreen.html)

[Create ticket on Racer 4Biz app](/en-us/4biz-helium/additional-features/racer-4biz-app/create-ticket-racer.html)

[Configure instance to use Racer 4Biz and Mobile GO](/en-us/4biz-helium/additional-features/mobile-and-field-service/configuration/configure-field-service-application.html)

[Get signature on Racer4biz app](/en-us/4biz-helium/additional-features/mobile-and-field-service/use/get-signature-in-attendance.html)
