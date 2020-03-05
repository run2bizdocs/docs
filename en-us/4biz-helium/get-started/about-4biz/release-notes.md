Title: Release Notes
Description: Release notes, policies information, bug fixes and improvements in the CITSmart.

# Release Notes

## Version 8.0.5.3 (2020/02/27)
Welcome to Citsmart Version 8.0.5.3. This version has the following improvements:

|Fix|Fix/Improvement/New|Functionality|Description|
|--------|---------|---------|---------|
|Ticket 3666|Fix|Ticket Management|Fix made when clicking on the Chat icon through the My Tickets widget, in the Experience Center.|
|Ticket 3581|Improvement|WebService|Updated to create an instance via WebService in a Ticket.|
|Ticket 3604|Fix|Event Management|Fix performed in the Generic Manager Zabixx/Nagios to enable the automatic correction option.|

## Version 8.0.5.2 (2020/02/18)
Welcome to Citsmart Version 8.0.5.2. This release has the following improvements:

|Improvement|Fix/Improvement/New|Functionality|Description|
|--------|---------|---------|---------|
|Ticket 3505|Fix|Tickets|Correction of flow elements|
|Ticket 3350|Improvement|Tickets|Performance optimization in the screens of ticket, user and user group.|
|Ticket 3505|Fix|Neuro|Correction of Neuro components|

*Other released products:*

Neuro: 1.3.3.3

## Version 8.0.5.1 (2020/02/10)
Welcome to Citsmart Version 8.0.5.1. This release has the following improvements:

|Improvement|Functionality|Description|
|--------|---------|---------|
|3256|Smart Portal|Correction of Parameter 293 to validate group permissions on the Smart Portal search.|
|3310|SLA|Adjustment of system behavior when changing SLA on suspension and reactivation of Tickets.|
|3347|Ticket Management| Adjustment made in the table facto_solicitacaoservico when a ticket is closed via Webservice.|
|6739|WorksPlace| Adjust in the Worksplace Widget to display information correctly.|
|6247|Ticket Management | Adjustments made in the ticket approvals.|

Version 8.0.5.0 (2020/01/27)
---------------------------

Welcome to CITSmart Version 8.0.5.0. This release has the following
improvements:

| Improvement | Functionality        | Description                                                                                                                                 |
|-------------|----------------------|---------------------------------------------------------------------------------------------------------------------------------------------|
| 5485        | Change Management    | [ITSM 1504] Sending a change approval email to everyone in the approval group                                                               |
| 6242        | Knowledge Management | Improvement that allows adding new permissions on the knowledge folders to be used to define the action of the document in 'Knowledge base' |
| 6243        | Knowledge Management | Improvement to add actions (state) to contemplate the phases of the knowledge process                                                       |
| 6244        | Knowledge Management | Add knowledge article comments                                                                                                              |
| 6245        | Knowledge Management | Add history to knowledge document                                                                                                           |
| 6246        | Knowledge Management | Improvement that allows configuring notifications to be received regarding knowledge                                                        |
| 6287        | Knowledge Management | The Knowledge Folder is allowing you to link interested parties with the Notification options and / or Notify the Author option             |
| 6387        | Knowledge Management | Adjusted e-mail sending behavior for all Group users informed to interested parties                                                         |
| 6075        | Experience Centers   | A global report and dashboard filter widget has been created                                                                                |
| 6396        | CMDB                 | Improvement to create a Relationship Type screen                                                                                            |
| 6397        | CMDB                 | Improvement to create a Relationship link screen in CMDB                                                                                    |
| 6399        | CMDB                 | Creation of the CMDB Map to allow graphical visualization of the entire managed environment.                                                |
| 6386        | Knowledge Management | Improvement to add new action of 'Delete' in the knowledge folder                                                                           |

Version 8.0.5.0. has the following fixes

| Fix  | Functionality                                                                                   | Description                                                                                                                                               |
|------|-------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1920 | CMDB                                                                                            | Corrective performed when informing start date greater than end date in the "Financial" tab of the CMDB.                                                  |
| 6391 | [General](https://dictionary.cambridge.org/pt/dicionario/ingles-portugues/general) registration | Correction of the popup label "Service Level Agreement Registration (General)", when the system language is in English                                    |
| 6416 | Problem / Release / Change Ticket Management                                                    | Correction of failure when creating a problem / release / change / ticket, when the customer used parameter 104                                           |
| 6419 | Omnichannel                                                                                     | Fixed message presented with error to the user when the user was registering Omnichannel - Facebook-Messenger interaction                                 |
| 6433 | Change management                                                                               | Adjustment of the Change type label to the correct term                                                                                                   |
| 6515 | Omnichannel                                                                                     | Fixed error when registering an Omnichannel Facebook-Messenger Interaction Channel in Oracle DB                                                           |
| 6517 | Knowledge Management                                                                            | Fixed "Error" showing "Edit" a "Knowledge" when it was created with a situation other than published                                                      |
| 6536 | Omnichannel                                                                                     | Error that was occurring via chat conversation between requester and attendant of a ticket created via Omnichannel Facebook-Messenger                     |
| 6221 | System General                                                                                  | [ITSM 2544] A correction was made in the treatment of the logs, where a request was constantly being submitted to the bank where it was shown in the log. |
| 6247 | Ticket Management                                                                               | A correction was made to the problem that occurred when approving a ticket                                                                                |
| 6312 | E-mail Models                                                                                   | E-mail templates with PostgreSQL knowledge actions were implemented (these e-mails are only loaded on installation)                                       |
| 6355 | Knowledge base                                                                                  | Within a Knowledge folder in the "Access Profiles" the Action of Archiving has changed the label to Archive / Unarchive                                   |
| 6358 | Knowledge Management                                                                            | Correction in the language of the status of situations in the knowledge history.                                                                          |
| 6381 | Ticket Management                                                                               | A correction was made to block the change of service portfolio at the time of execution of a ticket (It will only be allowed when reclassifying)          |
| 6392 | Knowledge Management                                                                            | Corrective layout of the page that broke when clicking on new knowledge was performed                                                                     |
| 6407 | Release Management                                                                              | A correction was made to limit the number of characters in the "description" field of a release portfolio                                                 |
| 6371 | Knowledge Management                                                                            | Adjustment in the display of Messages from interested parties                                                                                             |
| 6410 | Change Management                                                                               | Error presented to the user when the user clicked the Next button in a Change Portfolio                                                                   |
| 6411 | Ticket Management                                                                               | Corrective performed in the mandatory fields when creating a ticket, they were not considering the page settings                                          |
| 6412 | Ticket Management                                                                               | Fixed ticket screen so that the situation is in accordance with parameters 182 and 192                                                                    |
| 6417 | Knowledge Management                                                                            | Fixed when the user has permission in the knowledge folder by access profile to perform the action of Publish and Restore a knowledge                     |

!!! info "NOTE" 
    Knowledge Base improvements have not been implemented in an Oracle database.


## Version 8.0.4.5 (2020/01/14)

Welcome to Citsmart Version 8.0.4.5. This release has the following fixes:

|Fix	| Functionality	| Description |
|--------|---------|---------|
|3074 | Web Service | Adjustments in the automatic closure of tickets via WebService.|

## Version 8.0.4.4 (2019/12/19)

Welcome to Citsmart Version 8.0.4.4. This release has the following fixes:

|Fix	| Functionality	| Description |
|--------|---------|---------|
|ITSM 2652 | Knowledge Base Maintenance Report | Fix in the knowledge base maintenance report where information was duplicated.|

## Version 8.0.4.3 (2019/12/18)

Welcome to Citsmart Version 8.0.4.3. This release has the following fixes:

|Fix	| Functionality	| Description |
|--------|---------|---------|
| [ITSM 2854] | Registering Quiz | Fix when registering a quiz, where the system was creating quizzes at the time it changed.|
| [ITSM-2995] | WEBSERVICES |Fix when closing a ticket via webservice. The ticket was leaving the Solution/Response field blank, and with no responsible.
| [ITSM-2960] | Ticket Management | A corrective fix was implemented  where when executing a ticket, the service and activity corresponding to it was not being presented. What was being presented was the portfolio selection stage.|

## Version 8.0.4.2 (2019/12/12)

Welcome to Citsmart Version 8.0.4.2. This release has the following fixes:

|Fix	| Functionality	| Description |
|--------|---------|---------|
|6058|Ticket Management|RIt was performed some spelling fixes. The name in the popup header that is currently displaying "Request". Change this name to "Ticket".|
|6277|Ticket Management|Fix when sending an attached text document to open the ticket via email, it was placing this attachment description in the ticket description.|
|6334|Ticket Management|Fix in the application when parameter 446 was enabled, and when closing the ticket and it had an attachment, the closure email is not sent with that attachment.|

## Version 8.0.4.0 (2019/11/30)

Welcome to Citsmart Version 8.0.4.0. This release has the following fixes and improvements:

|Improvement	| Functionality	| Description |
|--------|---------|---------|
|5959  | Anuva | Implemented message sending functionality to Anuva |
|3902  | CITSmart Installation |	Fix in the internationalization of loads on a zero basis, the initial loads of the screen 'Cause' and 'Solution' should be with the language selected in the installation. |

|Fix	| Functionality	| Description |
|--------|---------|---------|
| 6241 | SmartChat	| It was made corrections when trying to open a ticket via chat. | 
| 6258 | SmartChat | Performed corrective as it was not displaying the attendant name in the conversation window even when the attendant captured the ticket |
| 6213 | Portfolio and Catalog Management | Fixed loading support service on service map | 
| 5947 | Email Template | Adjusting in the languages of the email templates, the initial screen loads should appear with the language selected at installation. If it is in English, then no matter which language is selected in the application the screen data will be in English | 
| 5970 | Neuro | Fixed in Neuro form session on ticket screen. | 
| 6069 | Neuro/Flow | Fixed the function Edit field in a Flow and Neuro | 
| 5939| Notifications | Fixed the number of Notifications seen | 
| 6261 | Approval Service via Token | Fixed bugs in the Approval via Token | 
| 6141 | SLA | Made adjustments to the Time of attendance of SLA of services | 
| 5969 | Ticket | Adjusted Ticket Search with values in single quotes | 
| 6262 | Ticket | Fixed Bugs in Sub-Ticket Creation | 
| 6068 | Web Service Operation	 | Fixed Web Service updateStatus to call the finish method () when the status is CLOSED. | 

!!! info "NOTE"
    OBS: 5947 Initially only for Postgres bank.

!!! bug "KNOWN ERRORS"
    6272 - Failure when attempting to execute a ticket with canceled status.
    6273 - Search field of the Change screen incorrectly displays the name of the responsible for current task.
    6274 - Tickets with a status of "Canceled" in the floating menu show incorrect actions by the status of the ticket.
    6275 - #5544 - Facebook-Messenger error when closing or canceling a ticket created via Facebook Messenger. It still shows the chat icon in the list of "Tickets in progress" and does not open another ticket for this same Messenger requester.

## Version 8.0.3.0 (2019/11/01)

Welcome to CITSmart Version 8.0.3.0. This release has the following fixes and improvements:

|Item|Description|
|--------|---------|
|4776|"Category" field now has just one line in the xls report|
|4815|The Problem Registration allows to complete all fields (without autocomplete).|
|4841|Error on the change screen message displaying generic message while criticizing required field|
|5095|Error in the Release search|
|5304|Creation of Change from a Problem| 
|5305|The tool should allow automatic association or definition of the appropriate SLA based on predefined methods.|
|5309|Should allow management of multiple chained changes|
|5326|Removal of Change Template functionality|
|5373|Create native webservices in CITSMART WORKFLOW|
|5544|Facebook Messenger Integration with Smartchat|
|5557|Implementing knowledge portfolio|
|5592|Adding the title, description, non-implementation effect, advisory committee and 'planning' and 'reversal plan' tabs in the Change Model|
|5678|Limit field to 200 characters|
|5769|Flow execution correction.|
|5861|Access denied fix.|
|5863|Implementation of adding employee-repository.js|
|5882|[Tickets] Error trying to view a closed ticket in some situations|
|5890|[4785] Notifying requested attendant when messaging between attendants|
|5910|Correction in internationalized key|
|5919|When new message arrives all minimized chats are being notified|
|5920|Doesn't load correct Neuro form when portfolio configuration changes. Correction in the monitoring template|
|5925|Error in the correction on Request for Change screen|
|5926|Entering alert message by clicking on create change option|
|5958|Fixed error in SLA not being able to link to a Service in the portfolio - "Error running the location...."|
|5959|Create possibility to send messages to anuva|
|5962|Twitter integration fixes|
|5969|Error trying to create ticket when falback message contains quotation marks "".|
|5981|Allowing to register service requests without locale.|
|5982|[2466] - Error Inactivating a linked quiz with link to the ref. to the popup presentation|
|5983|Remove access to new omnichannel configuration functionality from the system main menu|
|6042|Remove access to new Knowledge Portfolio functionality from system main menu [Simple 5557]|
|6049|Required group field in release delegation|
|6051|Automatic Change Actions registration screen error|
|6053|Failed to start a chat conversation, it is not being able to perform message exchange, that is, messages are not being delivered!|
|6054|Adding the "Import discontinued template data" option|
|6071|Changing impact and urgency columns to accept 2 characters as per bank structure for priority matrix|

## Version 8.0.2.0 (2019/10/07)

Welcome to CITSmart Version 8.0.2.0. This release has the following fixes and improvements:

|Item|Description|
|--------|---------|
|4785|Improvement in the communication Attendant x Attendant in Smart Chat.|
|4609|[MY-452] Add filter and Unit column in the Tickets panel.|
|4610|[MY-201] When registering new User, send Login and Password by email.|
|4608|Allows to filter the attendance queue by Ticket Status.|
|4621|[My 259] - Allows the linkage of child Configuration Item Group in Remote Access.|
|4602|Create dynamic flow components.|
|4616|Unify Widgets from "My Approvals and My Requests" in "My Tickets".|
|5408|Integration of "Widget of Service" with "Knowledge" in the Experience Center.|
|5409|End user ticket screen in the Experience Center.|
|5492|Configuration area of the "My Tickets Widget".|
|5569|[ITSM 1652] – Failure in the Simple of Problem, Change and Release. When creating a Workspace, the Sprints overwrite themselves.|
|5487|[Ticket] -  Ticket is being duplicated when reopening request in closed ticket filter view.|
|5362|[Ticket] - Ticket history presenting unconfigured comment.|
|5493|[Change] - Text translation corrections in the Change process.|
|5469|[Ticket] - Error clicking print on a closed ticket using the new closed filter.|
|5495|[Ticket] - Failed to remove attachment when creating ticket from the Experiment Center screen.|
|5494|[Email] - Investigação sobre chaves internacionalizadas de modelo de e-mail.
|2613|[Trend Analysis] - Adjust the screen of Problem creation.|
|2612|[System]  - Adjust the Impact and Urgency fields according to parameter 104.|
|5272|[System] - Create API/Backend security rules for the database command execution screen.|
|1273|[CMDB] - Allows to remove default groups.|
|4309|[Ticket] - Ticket with Neuro form exceeds the default screen size when viewing flow Variables.|
|3423|[Problem] - System is allowing to save known error without reporting any folders in problem portfolio.|
|2125|[Ticket] - Prevent service Request from being closed and dated null.|
|4847|[Ticket] - Error in the search behavior of subrequest.|
|4848|[Ticket] - Check subrequest closed without closing group.|
|5221|[Email] - Incorrect behavior when viewing available email template options when a system update occurs.|
|4980|[Ticket] - Remove search and blank from comments section of ticket attendant screen when no information is displayed.|
|4559|[Ticket] - Problem regarding to the Requestor CI and Related CI in a Ticket.|
|4933|[CMDB - Inventory Status] - Reset link options in IP and 'Inventory Now'.|
|2850|[Change] - Verify that the Roles and Responsibilities option for Change is displaying duplicate information for this option.|
|4354|[Ticket] - Field of Date (Post Hours) from Comment accepts alphanumeric characters.|
|1654|[Group] - Correct Group screen - duplicated flow.|
|5511|[Experience Center] - Verify that in the experience center, when we create 'My Approvals' widget, the tickets are not listing.|
|5522|[Ticket] - When the description has an image, the image exceeds the margin in the description field in the satisfaction survey mode in the Ticket Widget in EC.|
|4845|[Ticket] - Parameter 448 doesn't reflect the subrequest creation text editor.|
|1528|[Knowledge] - Comment moderation, if comment is rejected, remove comment from comment count.|
|5223|[Ticket] - Verify tha the system doesn't return Activity and Type in history after reclassifying a ticket.|
|2580|[Image Gallery] - The Knowledge Base Image Gallery no longer has URL when clicking on an image.|
|4764|[Knowledge] - The Knowledge Portal view exceeds page layout.|
|4874|[Ticket] – [Show reason to approve and reject on the occurrence] Change how the reason for approval or rejection on the occurrence is displayed.|
|5878|[ITSM 2002] - Error in EC links doesn't record settings from within another EC.|
|5763|[ITSM 1829] - Error in Neuro.|
|5781|[ITSM1846] - Verify that when delegating a ticket the occurrence of the advanced search history is coming unconfigured.|
|5568|[ITSM 1313] - Edge Browser doesn't save to the "Description" field in a Ticket.|
|5883|[ITSM 1971] - Check null pointer on ticket screen when parameter 231 is active.|


!!! info ""
    In version 8.0.2.0, the parameter 299 - Ticket - Enable message exchange has been retired because the messaging functionality has been replaced by the Chat. The histories are kept in the occurrence histories.

!!! info ""
    In version 8.0.2.0 in the ticket list we insert the possibility of appearing the field "Description". In order to view this field, the user must follow the procedures:

    1.	Clean cookies;

    2.	Delete records from serviceRequestColumnsProfile table
    
    3.	Restart the system after developing step 2.

    Chat communication in this version is most effective when done in the same browser, if a requester and an attendant are in different browsers, there may be a long delay in message exchange.

    For a better experience of the CITSmart version 8.0.2.0, we advise that the “my requests” and “my approvals” widgets to be replaced by the “my tickets” widget in the customers Experience Centers.

## Version 8.0.1.7 (2019/09/13)

Welcome to CITSmart Version 8.0.1.7. This release has the following fixes:

|Item|Description|
|--------|---------|
|5569|[ITSM 1652] – Failure in the Simple of Problem, Change and Release when creating a Workspace, the sprints overwrite themselves.|

## Version 8.0.1.6 (2019/09/11)

Welcome to CITSmart Version 8.0.1.6. This release has the following fixes:

|Item|Description|
|--------|---------|
|5288|Safety – Do not make system users password visible|
|5272|Safety – Do not allow access to the Script screen without logging in to the application|

## Version 8.0.1.5 (2019/09/02)

Welcome to CITSmart Version 8.0.1.5. This release has the following fixes:

|Item|Description|
|--------|---------|
|5407|Simple – Functionality did not allow downloading attachments from Simple cards|

## Version 8.0.1.4 (2019/08/20)

Welcome to CITSmart Version 8.0.1.4. This release has the following fixes:

|Item|Description|
|--------|---------|
|5067|Knowledge Base - [My 1009] - Check attachment exchange in knowledge draft.|
|4418|Ticket Management - The Ticket List search filter Status field is not searching as requested.|
|5066|Knowledge Base - Nullpointer when versioning new knowledge containing attachment.|
|5000|Okta Integration - Create/Update user data during SAML authentication.|
|5146|Ticket Management - Check Null Pointer error when wending email of occurrence.|
|5078|Smart Portal - [My 1279] - System does not validate mandatory questionnaire field|
|5068|Smart Portal - [My 1190] - Check error while viewing reclassified ticket history |
|3904|Problem Management - Verify that no PDF could be generated from the problem form accessed|
|5042|Chat - When you open the Chat and then minimize it, the scroll bar no longer works.|
|5108|Problem Management - Error registering problem|
|5076|CMDB - Inappropriate behavior in changing the characteristics of a CI.|
|4866|Reports- Internationalization for date presented in ACC report.|
|4178|Ticket Management - Kanban per attendant does not open the interface.|
|4839|Chat - Fix integration of the SmartChat with the Knowledge Base and Portfolio.|
|5061|Snow - Verify that integration with Snow does not return inventory data.|
|5044|Chat – Chat error when you try to talk to with an attendant.|
|4385|Ticket Management - [My 389] - Security failure in attached files.|
|5073|Knowledge Base - Error downloading attachment from public and external knowledge.|
|1504|Knowledge Base Report - Knowledge Base Maintenance Report showing layout errors in both .XLS and .PDF.|
|4787|Ticket Management - Check email template keys that return no information.|
|3881|Knowledge Base - Unhandled error when trying to insert Knowledge Base containing content longer than 20.000 characters.|
|4514|Ticket Management - Verify that the application is not validating the requirement of time of attendance overdue.|
|4978|Experience Center - Failure in the widget “My Request”.|
|4786|Ticket Management - Error sending occurrences, the system sends copy to the outbox.|
|4740|Ticket Management - [My 810] - Translation failure in the satisfaction survey options when it opens in private browser.|
|4599|Installation - Script errors when uploading CITSmart on zero basis.|
|5001|Problem Management - [My 1168] - Verify that attachments cannot be viewed on the problem preview screen.|
|3192|Continuity Management - Access permission error when user has permission.|
|4825|Neuro - Unable to change parameters in Oracle database.|
|3612|Ticket Management - Remove 'Deadline' information when SLA is 'TO COMBINE' at the time of execution.|
|4966|Smart Decision - [My 1120] - Check for inappropriate behavior when linking 2 Smart Decision specific widgets.|
|4934|Problem Management - Failed to return proactive problem conclusion registration|
|4542|Experience Center - [My 560] - My Request widget breaking description layout|
|5002|Ticket Management - [My 1166] - Verify that CITSmart is not displaying attachments on the ticket screen.|
|4482|Ticket Management - Ticket Description "Breaking" modal when presented via "View" option triggered from floating menu.|
|2107|Problem Management - Verify that when the root cause response and workaround is large, and the application brings the whole misconfigured popup on the TICKET screen in the 'Workaround' option|
|5289|[ITSM 1384] - System flow does not return link of events.|
|5290|Failure when creating a ticket through the portal for a non-approval service and when parameter 65 is not entered.|

**Note:**

In version 8.0.1.4 the “Description” field of the service request attendance screen will be blocked after the creation of a ticket.


## Version 8.0.1.3 (2019/07/31)

Welcome to Citsmart Version 8.0.1.3. This release has the following fixes and improvements:

|Item|Description|
|--------|---------|
|4763 |Correction in the language displayed in the Knowledge Portal.|
|3720 |Correction in the webservice of updateStatus.|
|4541 |Correction in the SSO Integration ITSM.|
|4522 |Creation of the option to remain in attendance screen after registering the ticket.|
|3869 |Check if it is possible to link "change" duplicated.|
|4598 |Correction in the comment search for SQLServer in the ticket screen.|
|1355 |Correction in the use of "anchors" in the knowledge base.|
|4754 |Correction when saving images in the Knowledge Base. |
|4748 |Correction in the internationalization of reports.|
|4742 |Correction in the installation of flow designs.|
|3637 |[ITSM 9752] - System does not load graphics in Availability Management.|
|4729 |[MY-804] - Failed to access Simple on Mobile CITSmart Experience application.|
|4836 |Error in expressions when importing flow.|
|4674 |Check Simple checklist that does not count the complete one.|
|4585|[Access Profile - Oracle] [Clean Base]: Error clicking save button in the Access Profile registration.|
|4523|Parametrize the redirect page after saving a Ticket in the Experience Center.|
|4756|Correction in redirect behavior of the knowledge creation screen.|
|4035|Internationalization Error - Ticket screen is being translated into French.|
|4422|[ITSM 461] - When opening a tab containing an attachment in a ticket registration, the system attaches the file to another ticket.|
|4136|Unhandled error when trying to create ticket.|
|2358|Error saving in Original version a flow that we have renamed.|
|3696|[Smart Portal] - Verify that the application is changing the language when switching service display.|
|3672|The "Clear" button is not working in the Report of USTs Use in the Contract Management functionality.|
|4287|[ITSM 347] - Translation error in English reports.|
|4526|[My 481] - Check HTTPS connection failure on port 443.|
|4728|Label change from format “Nº” to “NO”.|
|4540|[My 577] - Translation error in group registration screen.|
|4600|Error inserting an attachment and then removing it from the Change Management screen (attachment field disappears).|
|2845|Notifications that appear in duplicate.|
|4771|The attendance is failing when accessing the ticket screen via Smart Chat and advancing the flow competed.|
|4317|[Chat] - Verify that messages cannot be exchanged between attendants.|
|4543|[Chat - Ticket] - Check the possibility to open the Ticket execution screen via chatbox.|
|4315|Check the possibility of removing the information "How can I help you" from chat when the service has already started.|
|4572|When moving an item from one Sprint to another in Simple, it is moved to an archived list.|
|4533|[Chat] - Problems interacting with Anuva.|
|4535|[Chat] - Change the label "Request" to "Ticket" that appears inside the chat.|
|4532|Change phrases displayed in chat popup.|
|4587|Error in Simple when registering a new Sprint - with users.|
|3868|Check layout break with "problem" with long title.|
|4595|[Portfolio]: Error trying to save a new service registration.|
|4529|[Time of Attendance]: "Customer" time not showing correct SLA value.|
|852|Do not display on the parameter screen items that are already displayed on configuration screens.|
|4536|“Anuva” widget change in the Experience Center configuration.|
|3660|In the user registration, when searching the contributor by the Brazilian ID CPF - with the correct masks containing points and hyphen - no result is displayed.|
|4570|Error accessing ticket screen on an installation basis.|
|4546|[Chat]: Replace message icon hint inside ticket screen.|
|4117|Adjust the label "SmartDecisions" in Access and Permission to "Smart Decisions".|
|3178|Verify that the "Drive" popup within the "Time of Attendance" screen is opening with incorrect pattern.|

**Note:**

In version 8.0.1.3 the parameter “452 - Continue in the Ticket screen after saving?” was created. This parameter, when enabled, checks the user's permission to execute a ticket and allows the screen to remain..

In version 8.0.1.3 the parameter “451 - Redirect page after saving the ticket in the Experience Center” was created, which allows informing the page that the user wants to return when an action in the Experience Center occurs.


## Version 8.0.1.2 (2019/07/20)

Welcome to the Citsmart Version 8.0.1.2. This version presents the following fixes.

|Problem|Description|
|-------|-----------|
|4730|Error creating a ticket through Smart Portal when it has no Neuro or Questionnaire|
|4537|Error in the LDAP synchronization|
|4733|Slowness in Smart Portal when there is knowledge related|

From version 8.0.1.2 it was inserted the parameter “454 - Display the smart portal knowledge tab only when there is content” this parameter controls the display of the Knowledge Tab in Smart Portal only when there is knowledge linked to the Activity, if it does not exist, the system does not display the tab.

## Version 8.0.1.1 (2019/07/15)

Welcome to the Citsmart Version 8.0.1.1. This release contains the following fixes.

|Problem|Description|
|-------|-----------|
|4425|[My 218] - Error saving request with questionnaire that has validator in the flow.|
|4426|[My 222] - When validating the registration of a questionnaire, the fields of the type radio or combo are not saving the options.|
|4604|[My 710] - Error in external knowledge requesting login and password.|
|4552|[My 589] - When you access the user registration screen and select a user and click on save and refresh the page, you get automatically logged with the user you have selected.|
|4650|[My 686] - When you make approvals of tickets via token by e-mail, you are directed to a CITSmart page in the EDGE/MOZILA/CHROME browser, where the information is appearing in English even with the parametrization in Portuguese.|
|4168|[My 001] - Error while viewing a ticket by advanced search.|
|4596|[My 705] - Verifying error in deadline calculation for tickets.|

## Version 8.0.1.0 (2019/06/28)

Welcome to Citsmart Version 8.0.1.0. The Version 8.0.1.0 of Citsmart presents the following improvements:

|Improvement|Description|
|--------|---------|
|3717|Optimization in Chat, ANUVA and Message Exchange – The entire messaging system has been integrated into Chat, so channels such as Messaging from this version, promote a more iterative dialogue between the requester and the attendant.|
|3467|Improvement in ticket attendance interface - 1. From this version, the users can dimension the service interface visually in a way that best meets them. 2. The interface became larger giving visibility to the ticket information, and the menus are in a tab that becomes visible only when the attendant needs other resources. 3. The comments have gained their own session where Content Search, Editing, Deletion and Response between attendant and requester and between attendants is allowed. Therefore, the function of public and private conversations was maintained.|
|3127|Experience Center - Widget of Simple. The resources of this important management tool from this version will be available in the Experience Center, facilitating the work of the teams that treat their activities through it.|
|1516|We included the possibility to filter by Estimation period of a Workspace and Sprint.|
|2126|User Profile Improvement: We have included the possibility for the user to edit the following information: Unit, extension, email and telephone.|
|3491|In the notifications of a ticket, we include the possibility of having an audible alarm that alerts the attendant of the arrival of a new ticket to the service queue.|
|3875|The option to reclassify is now parameterized through group registration, so the functionality contained in the ticket may or may not be available according to group permission.|
|4211|On the ticket screen, the email field received an auto complete to make it easier to search for user emails.|
|2584|Simple - The sprint administrator can assign a specific user the manager accesses of a Sprint.|
|2134|Simple - Restriction to edit the Administrator access profile.|
|837|Simple –  Presentation of the quantity of tasks by list in the Sprint|
|1265|Parameter to enable/disable sending attachments in email notifications|
|3718|Ticket – Filtering option increment by Date of last Update in the search items.|
|2588|Simple – Search by part of workspaces, sprints and tasks titles.|
|2711|Presentation of unread notifications in the foreground.|
|474|Contract Registration - Allow multiple selection of Units.|
|2585|Simple - Option to order Workspace and Sprint.|
|3462|Integration of CITSmart with OKTA|
|1498|Simple - Presentation of the task number in editing an activity.|
|3070|Simple – Filter by name of employees and name of TAG.|
|3911|Smart Portal - After ticket registration, direct the user to "My Requests".|
|2615|Simple – Search for unselected items.|

## Version 8.0.0.10 (2019/06/07)

Welcome to CITSmart Version 8.0.0.10. This release features some emergency fixes.

| Problem	| Description|
|-----------|------------|
|3097	| Error attempting to link an attachment in Sub-request |
|3607	| Correction in notification view |
|3900	| Correction in ticket delegation |
|3914	| System allows to register same login for different users |
|4028	| Correction in the presentation of the responsible person in the registration of an occurrence |
|4148	| Improvement in the queries of the ticket listing |

## Version 8.0.0.9 (2019/05/31)

Welcome to the Citsmart Version 8.0.0.9
Version 8.0.0.9 of CITSmart presents some emergency corrections.

|Problem |Description|
|--------|-----------|
|3670|Validation of the email field on the User Profile screen|
|3702|Correction in Neuro Scripts|
|3793|SQL optimization in the request list to reduce response time|
|3879|Kanbam correction per attendant to view the task information|
|3895|Problems running CMDB cron|
|3897|System forwarding password reset to inactive user|
|3915|Optimizing SQL list of requests|
|4038|Correction of image upload in portfolio presentation|

## Version 8.0.0.7 (2019/05/17)

With performance optimizations, usability improvements, adjustments and bug fixes.

| **Code**   | **Ticket Description**                                                                                                                                                                                                                                          | **type**     |
|------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| 3005       | Analyze and improve system menu class                                                                                                                                                                                                                 | Improvement  |
| 3004       | Analysis and improvement in I18N class                                                                                                                                                                                                                            | Improvement  |
| 2869       | Analysis and correction of open streams                                                                                                                                                                                                                           | Corrective   |
| 3466       | Internationalization problems                                                                                                                                                                                                                                | Corrective   |
| 3701       | [ITSM 9819] - In Release Mgmt., system loading another user as responsible                                                                                                                                                                               | Corrective   |
| 3155       | Change Labels Names and Set Neuro Menus                                                                                                                                                                                                                   | Improvement  |
| 2389       | GRP architecture settings                                                                                                                                                                                                                                      | Corrective   |
| 3884       | [ITSM 9845] - Failure to load attachments in unstable and slow environment                                                                                                                                                                                             | Corrective   |
| 3707       | Datepicker is not functional when you try to select the date in the Problem report. The same allows to fill, however, does not allow to select specific date.                                                                                                        | Corrective   |
| 3264       | [ITSM-9480] - Verify that the system does not respond to the email component drawn in the flow                                                                                                                                                                   | Corrective   |
| 3790       | [ITSM 9816] - Changing the dynamic context of the missing CITSmart screens \# 3698                                                                                                                                                                            | Corrective   |
| 3870       | Check error message when clicking on "questionnaire"                                                                                                                                                                                                          | Corrective   |
| 3698       | [ITSM 9816] - Some CITSmart URL are not respecting the jboss-web.xml configuration. That is, when the context is changed from "citsmart" to "anac", or something like that. Screens such as Neuro form and flow maintenance crash. \# 3790 | Corrective   |
| 3877       | Check system behavior when trying to access the application with consultant on a zeroed basis                                                                                                                                                               | Corrective   |
| 3214       | [ITSM-9609] - Error appending a file with a numeral character                                                                                                                                                                                                   | Corrective   |
| 3471       | Only display tabs if there is content                                                                                                                                                                                                                          | Improvement  |
| 3791       | [ITSM 9793] - Verify that when we try to change form data for a request, clicking "Save" will not save this information.                                                                                                    | Corrective   |
| 3664       | [ITSM 9793] - Verify that when trying to reclassify a request by exchanging activity, the application is not loading the Neuro form of that activity.                                                                                                   | Corrective   |
| 2870       | [Neuro] Internationalization load optimization                                                                                                                                                                                                              | Corrective   |
| 3616       | Check problem of slowness to REGISTER A CHANGE with a large number of attachments (extensive attachments).                                                                                                                                                  | Corrective   |
| 3649       | Some flow components are not displayed in Chrome browser                                                                                                                                                                                                  | Corrective   |
| 3610       | When accessing a particular screen via the link, the menu list is not loaded                                                                                                                                                                                           | Corrective   |
| 3661       | Improved SQL Client Structured Queries.                                                                                                                                                                                                               | Corrective   |
| 3678       | Create form of greater control of requests of webservices                                                                                                                                                                                                     | Improvement  |
| 3499       | Quick access items are not following Access Profile                                                                                                                                                                                                      | Corrective   |
| 3590       | [ITSM 9708] - Knowledge base with profile per group does not appear for link in Portfolio                                                                                                                                                                   | Corrective   |
| 3500       | Standardize icons and add hints                                                                                                                                                                                                                             | Improvement  |
| 1557       | Verify that it is not possible to select a change template in the template screen                                                                                                                                                                       | Corrective   |
| 3689       | Verify that it is not being able to access the Simple                                                                                                                                                                                                          | Corrective   |
| 3517       | Internationalization settings in CITSmart Workflow                                                                                                                                                                                                             | Corrective   |
| 3611       | After installation of the system, it is not possible to access the toolbarHeader                                                                                                                                                                                      | Corrective   |
| 3668       | The Quick Access applications are not being displayed on the old screens                                                                                                                                                                                       | Corrective   |
| 3624       | [ITSM 9623] - When reclassifying a ticket, it presents the following message: Key must not be null or empty.                                                                                                                                          | Corrective   |
| 3623       | Removing attachments when forwarding flow after a request is created.                                                                                                                                                                                              | Corrective   |
| 3496       | Check pattern to register related CI in CMDB                                                                                                                                                                                                          | Corrective   |
| 3494       | Verify that when the user clicks on 'View Relationship Map', the application displays error message.                                                                                                                                           | Corrective   |
| 3187       | Critical message (in pop-up) and "Start Date" field mandatory in the Contract Evaluation Period, presented with a misspelling.                                                                                                            | Corrective   |
| 3241       | Verify that the 'Outbox E-mail' field information is multiplying each time you save a contract.                                                                                                                                               | Corrective   |
| 3621       | Unable to remove attachments from the Release                                                                                                                                                                                                          | Corrective   |
| 3669       | It is not being able to create a ticket through the portal when the activity is configured to not display the description field                                                                                                                                       | Corrective   |
| 3607       | [ITSM-9097] - Handle saving of Neuro form data in Reclassification                                                                                                                                                                                | Corrective   |
| 3512       | Slow loading a Change/Release/Problem with attachments                                                                                                                                                                                                  | Corrective   |
| 3506       | Neuro does not automatically install in the migration from ITSM version 7 to 8                                                                                                                                                                                         | Corrective   |
| 3605       | [ITSM 9722] - Translation Error in Report                                                                                                                                                                                                                     | Corrective   |
| 3602       | [ITSM 9773, 9824] Verify that it is not possible to publish or version a knowledge                                                                                                                                                                | Corrective   |
| 1602       | Add counter in attachment icon, message and exchange the place of icons                                                                                                                                                                                    | Corrective   |
| 3501       | Display float button                                                                                                                                                                                                                                     | Corrective   |
| 3609       | It is not possible to remove attachments from the Change planning tab                                                                                                                                                                                     | Corrective   |
| 3589       | Error saving attachments. System did not save some attachments due to competition problem                                                                                                                                                                   | Corrective   |
| 3479       | Error logging into system                                                                                                                                                                                                                                        | Corrective   |
| 3596       | System is not displaying iframe. Spring boot: X-Frame-Options set to deny                                                                                                                                                                                     | Corrective   |
| 3463       | Change the "Start" label in breadcrumb to "Portal"                                                                                                                                                                                                             | Improvement  |
| 3559       | Corrective in the latest version of Simple                                                                                                                                                                                                                           | Corrective   |
| 3378       | The initialize function is not returning.                                                                                                                                                                                                                        | Corrective   |
| 3447       | No advanced session message is displayed on the advanced search screen                                                                                                                                                                                              | Corrective   |
| 3473       | Add autocomplete in the "Contact email" field                                                                                                                                                                                                              | Corrective   |
| 3066       | Field value (numeric) in the Form Registration, allows you to enter alphanumeric values, although the application does not save the registration, correct so that the field only fills the defined type                                                                   | Corrective   |
| 3281       | [ITSM-9629] - Modal for CI view opened by Event Mgmt. is too small and needs adjustments                                                                                                                                                   | Corrective   |
| 3368       | The word "Solicitación" must be replaced by "Solicitud".                                                                                                                                                                                               | Corrective   |
| 3186       | Critical message (in pop-up) as mandatory field "Contract" in the Contract Evaluation presented with misspelling                                                                                                                            |              |
| 3424       | Validate Neuro parameters before saving                                                                                                                                                                                                                   | Corrective   |
| 3166       | [ITSM-9562] - Check ticket registration with empty space                                                                                                                                                                                                     | Corrective   |
| 3201       | Correction of names in Impact and Urgency in the time of service screen                                                                                                                                                                                          | Corrective   |
| 3093       | Check system behavior when user clicks on 'About CITSmart'                                                                                                                                                                           | Corrective   |
| 1910       | Message is not internationalized (Depends on simple \# 2878)                                                                                                                                                                                                 | Corrective   |
| 2919       | It is not closing the modal by approving the request                                                                                                                                                                                                              | Corrective   |
| 3086       | Correct the term: "I didnt'l like it" to "i didn't like it".                                                                                                                                                                                                  | Corrective   |
| 2780       | Change operation status on the audit screen I=INSERT to C=CREATION.                                                                                                                                                                                         | Corrective   |
| 3282       | [ITSM 9628] - Failed to Edit a Zabbix Manager                                                                                                                                                                                                          | Corrective   |
| 3172       | When perform a token approval and there is no session in operation.                                                                                                                                                                                         | Corrective   |
| 3179       | Verify that updating the version is giving error in the update scripts. (Related to tasks 3154 and 2838)                                                                                                                                            | Corrective   |
| 3278       | Does not load labels after correcting database scripts                                                                                                                                                                                              | Corrective   |
| 3286       | Enable parsing of objects in the Rest component                                                                                                                                                                                                               | Corrective   |
| 1665       | Generating search report in .PDF without filling in required fields                                                                                                                                                                               | Corrective   |
| 3106       | In the Problem registration, when linking Ticket/Incident, the number component is showing negative numbers. Addendum: In the same field (Number) is accepting alphanumeric values (different from its type)                                   | Corrective   |
| 3072       | Verify that when we report on the working day the final time equal to 00:00, the application does not calculate the SLA correctly.                                                                                                                                    | Corrective   |
| 1596       | Verify that the user changed the last time of the DAY, but when creating request this change was not reflected                                                                                                                                        | Corrective   |
| 3067       | Improvements to the processing of the inventory queue (Threads)                                                                                                                                                                                                      | Improvement  |

**Other released products**

Neuro: 1.2.4.10

Audit: 0.4.0

## Version 8.0.0.5 (2019/04/25)

| Problem  | Description                                                                                                                                              |
|----------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| 3360     | Problem Mgmt. - Error retrieving the definitive Solution                                                                                                |
| 3361     | Problem Mgmt. - Error retrieving the closure field                                                                                             |
| 3362     | Problem Mgmt. - Errer retrieving known error                                                                                                    |
| 3363     | Configuration Mgmt. – Error retrieving Completed Changes related to the Configuration Item                                                        |
| 3364     | Release Mgmt. – Error linking Change closed in Release                                                                                       |
| 3365     | Problem Mgmt. – Interface suitability to display the fields "Associated error message" and "Diagnostics"                                          |
| 3366     | Change Mgmt. – Error retrieving Simplified Risk                                                                                                     |
| 3393     | Relese Mgmt. – Return of Business Rule when linking a change that has CI linked to a Release, automatically linking the CI to the Release |
| 3282     | Event Mgmt. – Failure when Edit a Zabbix Generic Manager                                                                                                 |
| 3115     | Event Mgmt. – Better rendering of the Ticket Mgmt. screen                                                                                             |
| 3394     | Release Mgmt. – System doubles attachments when forward flow                                                                                               |
| 3388     | Problem Mgmt. – Saving the known error does not set the archiving field and the system cannot recover the knowledge                              |
| 3419     | Change Mgmt. – System does not retrieve attachment placed in Revision and closure field                                                                    |

*Known error and solution*

Note the following scenario:

-   Preconditions:

    1.  The client will be upgrading from version 7 to version 8.0.0.5;

    2.  The consultant did not parametrize in the Problem Portfolio the folder
        to save the Known Error knowledge base;

-   What happens:

    1.  The user accesses the Problem Management screen;

    2.  The user informs the Root Cause field and attempts to save the knowledge base;

    3.  When open the Knowledge Base screen for saving, the system presents the message
        that the user does not have the permission;

-   Why does it happen?

    1.  The message appears because the consultant did not informed the folder to save
        the known error in the Problem Portfolio;

    2.  Once you try to save the known error, the system does not identify the folder
        and sends the message;

    3.  In these cases, contact the Citsmart Support to make the correctness of this
        register;

    4.  Make the configuration of the known error saving folder on the Problem Portfolio
        screen;

    5.  In the next registration the message will not be repeated.


**Other released products**

Neuro: 1.2.4.8

Inventory: 2.0.0.3

EVM: 2.0.0.3

Audit: 0.2.0


## Version 8.0.0.4 (2019/04/12)

| Problem  | Description                                                                                |
|----------|--------------------------------------------------------------------------------------------|
| 3275     | Failure when restoring the Executor Group, Impact and Urgency in the Release Management    |


## Version 8.0.0.3 (2019/04/04)

| Problem | Description                                                                                                                                                                                                          |
|----------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 2573     | Known error in version 8.0.0.0 when answering to a satisfaction survey by Experience Center Widget. Version 8.0.0.3 provides a definitive solution to the error while registring a satisfaction survey.     |
| 2122     | Webservice failed to create service request. Version 8.0.0.3 provides definitive solution to the failure presented when attempting to register a service request via webservice.                      |
| 2917     | Failed to upload attachments by the service request functionality. Version 8.0.0.3 provides a solution for uploading attachments through the service request functionality.                  |
| 2777     | Intermittent failure in the method that returns timezone to register the date and hour. In the Neuro component. Version 8.0.0.3 provides definitive solution in the Neuro component to register date and time. |


## Version 8.0.0.2 (2019/03/20)

| Problem | Description                                                                                                                                                                                                                                                                 |
|----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 2309     | Intermittent failure and of greater incidence in clustered environments in the method that returns timezone to register date and time. Version 8.0.0.2 provides definitive solution to the error that occurs in classes that use timezone for registration. |
| 2124     | Incorrect validation failure while accessing an external knowledge base. Version 8.0.0.2 provides definitive solution to the session expiration message displayed improperly when the user attempted to access an external knowledge base.                    |
| 2400     | Failure in the advanced search component that didn't return words with "ç" and "ã". Version 8.0.0.2 provides definitive solution for advanced search with accented words.                                                                                          |

## Version 8.0.0.1 (2019/03/08)

| Problem | Description                                                                                                                                                                                      |
|----------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 2576     | Known error in the portfolio that is not displayed when there is an end date in the contract service. Version 8.0.0.1 provides a definitive solution to the error caused by the service portfolio. |

## Version 8.0.0.0 (2019/03/01)

|Type|Functionality|Description|
|----|-------|-----------|
|Fixe|Ticket Management|The Sub-Request and Related Request functionalities were restructured to provide greater compliance to their assignments. The focus of this fix was to bring the functionalities closer to their proposal. For further information, see [Relate Ticket][1] and [Register Sub-Request][2]|
|Fixe|Webservices|The synchronization for creating new Activities has changed in the business rule, that's because it's not possible to create an activity that doesn't have a link with the Business Service and Portfolio. Therefore, the webservice designated for creation will open a ticket with the parameters in the initial configuration of the service. The functionality of create a new user, when the data synchronization is enabled, remains consistent.|
|Fixe|Flow|Adjustments to avoid editing native expressions and expressions of same name.|
|Improvements|Quick Access|The quick access allows the user to find main processes through icons that help in the efficiency of fixing and viewing. **The users only sees the icons of the processes that they have access, with the exception of Simple, Knowledge Portal, Experience Center and User Guide.**|
|Improvements|Ticket Management|We created the possibility of configuring the functionality of email notification in the ticket delegation. For further information, see [Notification via E-mail of Ticket Delegated][3]|
|Improvements|Ticket Management|We created the possibility of configuring the functionality notification via email reclassification. For further information, see [Notification via email of reclassified ticket][4]|
|Improvements|Change Management|Version 8.0.0.0 of CITSmart has improvements in the change management process, bringing the agile world to manage the activities that should occur during the scope of the change. **Note:** This functionality replaces the default flow parameters for usage of the change process, moreover, the change is necessary for this configuration. For further information, see [Change Management][5]|
|Improvements|Problem Management|In version 8.0.0.0 of CITSmar,t the problem management process allows adding activities to assist in the management of teams during the root cause diagnosis. **Note:** This functionality replaces the default flow parameters for usage of the problem process, moreover, the change is necessary for this configuration. For further information, see [Problem Management][6]|
|Improvements|Release Management|The release process is more powerful in planning, testing and approving, allowing the designation of activities and management at sight. **Note:** This functionality replaces the default flow parameters for usage of release process, moreover, the change is necessary for this configuration. For further information, see [Release Management][7]|
|Improvements|Knowledge Management|In version 8.0.0.0 CITSmart allows the evaluation and publication of written comments about a knowledge. For further information, see [Comments Review][8]|
|Improvements|Knowledge Management|We innovate the way of access to the knowledge base for users who don't have login to the CITSmart tool. In version 8.0.0.0 knowledge with permission of visualization can be accessed by the community in general, just have the link of access. For further information, see Configure external access to the [Knowledge Portal][9]|
|Improvements|Configuration Management|We enhance the user experience by highlighting a dashboard that displays the number of configuration items by group, type, and agglutinated in the Incident, Change, and Release processes, leaving in sight possible CI's that will be changed or involved in some incident. For further information, see [Configuration Item Management][10]|
|Improvements|Ticket Management|We simplified the use of ticket escalation rules, with a few steps, it'll be possible to implement the rule that previously had numerous configurations. **Note:** This functionality replaces the use of several escalation parameters, moreover, it's necessary to change for the effective use of the escalation rules. For further information, see [Create escalation rule][11]|
|Improvements|Ticket Management|In version 8.0.0.0 of CITSmart, we included ticket approval through a new direct icon in the attendance list, it's not necessary to open the ticket to perform the attendance, we present the available information and the options configured to accept or refuse the call. This functionality is available on Mobile SM and on the Service Portal. For further information, see [Approve ticket][12]|
|Improvements|Ticket Management|We allow the automatic ticket list updating function to be enabled to refresh the list automatically from time to time. For further information, see [Automatic Update of Ticket List][13]|
|Improvements|Ticket Management|The improvement of the occurrence registration allows the requester or technician to be notified via email. In addition to the permission to include activity execution time and keep the information confidential registered, so that only authorized technicians can see it. For further information, see [Register ticket occurrence][14]|
|Improvements|Integrated Management|Simple was created with the purpose of bringing the concept of agile management to the tool. Independently or clustered in one of the Problem, Change and Release solutions, Simple allows you to reuse Sprints, share resources, send activities to other Sprints and manage at sight. For further information, see [Simple][15]|
|New|Experience Center|We provide a specific area to improve the user experience. In this area will be allowed the presentation of services, information and reports that come closest to the day-to-day use of the customer. For further information, see [Experience Center][16]|
|New|Smart analytics|From the version 8.0.0.0, we have provided some quantitative reports of the main processes contained in CITSmart through our new BI platform. For further information, see [Business Intelligence][17]|
|New|Audit|We have reformed the system audit to increase the agility and reliability of the audit research feature. For further information, see [System Audit][18]|
|New|Platform administration|We have improved information security, implementing forms of password security for internal users. For further information, see [Password Security Policy][19]|
|New|Mobile|We delivered a new application that, in a robust way, allow the field service of technicians who are momentarily without internet connection. The mobility experience goes beyond signature features and notes. For further information, see [Mobile Field Service][20]. Still in the context of mobility, and no less robust, we improved the Mobile SM application, which has among other uses, the ability to sign, approve and notes. For further information, see [Mobile CITSmart Experience application manual][21]|
|New|Neuro|From the version 1.2.3.0 of Neuro, it's possible to automatically create a CITSmart questionnaire from the Neuro business object register. The idea behind this innovation is to facilitate the extraction of responses from CITSmart questionnaires and to create reports in a simple way, with the help of the Smart Report.|
|New|Flow|The package of flows delivered to the processes of Problem, Change and Release have been simplified, the products have been remodeled to adhere to the possibilities that the flow offers. __If the customer doesn't want to use the new flows, the latest version 7.1.0 will continue to work perfectly.__ |





[1]:/en-us/citsmart-platform-8/processes/tickets/use/register-ticket-related.html
[2]:/en-us/citsmart-platform-8/processes/tickets/use/create-and-view-sub-request.html
[3]:/en-us/citsmart-platform-8/processes/tickets/configuration/notification-delegated-email-ticket.html
[4]:/en-us/citsmart-platform-8/processes/portfolio-and-catalog/configuration/send-email-reclassified-ticket.html
[5]:/en-us/citsmart-platform-8/processes/change/overview.html
[6]:/en-us/citsmart-platform-8/processes/problem/overview.html
[7]:/en-us/citsmart-platform-8/processes/release/overview.html
[8]:/en-us/citsmart-platform-8/processes/knowledge/use/review-reviews.html
[9]:/en-us/citsmart-platform-8/processes/knowledge/configuration/configure-external-access-knowledge-portal.html
[10]:/en-us/citsmart-platform-8/processes/configuration/overview.html
[11]:/en-us/citsmart-platform-8/processes/tickets/use/create-escalation-rule.html
[12]:/en-us/citsmart-platform-8/processes/tickets/use/approve-a-ticket.html
[13]:/en-us/citsmart-platform-8/processes/tickets/use/desktop-of-service-desk.html
[14]:/en-us/citsmart-platform-8/processes/tickets/use/register-ticket-occurrences.html
[15]:/en-us/citsmart-platform-8/additional-features/project-management/simple-agile-management/simple-agile-management.html
[16]:/en-us/citsmart-platform-8/processes/knowledge/use/create-experience-center.html
[17]:/en-us/citsmart-platform-8/additional-features/smart-analytics/use-bi-solution.html
[18]:/en-us/citsmart-platform-8/platform-administration/logs-and-auditing/system-audit.html
[19]:/en-us/citsmart-platform-8/platform-administration/security/implement-password-security-rules.html
[20]:/en-us/citsmart-platform-8/additional-features/mobile-and-field-service/apps/citsmart-field-service-manual.html
[21]:/en-us/citsmart-platform-8/additional-features/mobile-and-field-service/apps/citsmart-app.html
