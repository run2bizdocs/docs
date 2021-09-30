title: Creating knowledge
Description: It's possible to create, edit and search knowledge about several subjects, ranging from clarifying a functionality to more technical guidelines.

# Creating knowledge

Creating knowledge is the act of saving information inside 4biz using the Knowledge Management functionality. Note that to perform any action it's necessary to have appropriate permissions, therefore, your view is limited to the type of profile being used.

## Before getting started

- [X] It's necessary to create folders and define access permissions. With this you can organize the knowledge and simplify the search of a knowledge article. (see [Creating access profile][2])  
- [X] To use the notification features, it's necessary to configure the parameters: **82** and **83** (Knowledge Creation/Change), **84** (Deleting knowledge) and **78** and **456** (Expiration of knowledge).  (see [Configuring email template][3], see [Configuring parametrization - knowledge][4]).


!!! note "NOTE"
    
    Parameters 82 and 83 have the same function, so it's not necessary to configure these two parameters, choose one of them. This is because now it has been gathered in a key email template that contemplates all activities that go from creating to archiving knowledge. And what does it mean? In this new scenario you'll use an email template that will contain several keys.
This template is already available in a clean installation, or if you already have an environment and are going to update it, you can use the email keys in your already used templates so that they stay in the new standard . (see [Key fields of knowledge base emails][5], see [Examples of email templates][6]).

## Procedure

1.	Access the functionality through the menu Processes > Knowledge Management > Knowledge Management;

### Search and Filters

When accessing the Knowledge Management, you'll see the main knowledge management interface. In it you'll find all the knowledge base registries, being able to perform several actions (depending on your permissions in the system), creating new knowledge or editing an existing one.

To locate a knowledge base, you have the following filters:

|Field|Description|
|-|-|
|Content|Enter a brief part of the knowledge, you can enter a word or a short sentence.|
|Document type|Select the type of information registered. By default, we have several options to select: *Document, FAQ, Known Error, Test Evidence, Recovery measure, Emergency Response Plan, Damage Evaluation Plan, Rescue Plan, Vitar Records Plan, Crisis Management and Public Relationships Plan, Accommodation and Services Plan, Communication Plan, Finances and Administration Plan, Service Quality Plan, Availability Plan, News.*|
|Situation|Select a criterion that matches the knowledge status. By default, we have the options: *All, In drawing, In revision, Reviewed, In Publication, Published, Archived*|
|Title|Enter a term that refers to the name of the knowledge.|
|View by|Select a criterion that references the actions you’re allowed to execute. By default, we have the options: *All, Can Review, Can Approve, Can Publish*|


!!! TIP "TIP"

    **For the Selection fields** - Other Items can be created as needed.
    
### Creating Knowledge

The main activity of the knowledge base management is the registration of information in 4biz to later enable its management. Let's access the registration interface and know its functions.

1.	Click on "Options", located in the bottom right side of the screen, then click on "Add new knowledge";

The knowledge base registration/management interface has the following functionalities:


- **Tabs when creating a Knowledge**

| Order (tabs) |  Tab | Description |
|-------|--------|-----------|
| 1 | Register | Form containing the fields for registration of knowledge bases |
| 2 | Related Document | It allows to link an existing knowledge to the document being created |
| 3 | Event Category Occurrence | It allows to link an event category (Event Management) |
| 4 | Interested Parties | Enables parties (users or groups) to be notified when a knowledge is updated |
| 5 | Notifications | Alternative to send notifications to interested parties |

- **Tabs when editing a Knowledge (add to the previous ones)**

| Order (tabs) |  Tab | Description |
|-------|--------|-----------|
| 1 | Register | `Previously described` |
| 2 | Comments | Any important information to the knowledge management (not visible to end users) |
| 3 | History | Knowledge change lifecycle, having details of what was changed and who made the change |
| 4 | Related document | `Previously described` |
| 5 | Configuration item | Relationship of knowledge with CMDB's configuration items (e.g.: user manual, tutorials, others) |
| 6 | Event category occurrence | `Previously described` |
| 7 | Interested parties | `Previously described` |
| 8 | Notifications | `Previously described` |
| 9 | Versions (only with active versioning) | It presents all versions of the document |

    
!!! note "NOTE"
    
    Note that the "Comments", "History", "Configuration Item" and "Versions" tabs only appear after the information is registered, as they are related to the knowledge management process. All actions taken from creation to closure are recorded in the history, serving as Audit.
  

#### Knowledge Fields

In the "Registration" tab, a form will be presented containing the fields for identification, treatment and control of the knowledge.

|Title (*)|Name of the knowledge|
|-|-|
|Action(*)|Knowledge management flow activity (e.g.: if the knowledge status is *"In drawing"* the possible action is *"Send for review"*). We also have the options, once the document is published: *Send for review, Send for approval, Send for publication, Publish, Archive.*|
|Attachment|Files related to the Knowledge|
|Author|Creator of the Knowledge|
|Availability Management|If the knowledge contributes to the Availability Management process|
|Content(*)|Content of the knowledge that will be made available on the Portal. Must include all the information and media related to the document|
|Copyright|Indication if the knowledge has copyright|
|Creation Date (automatic)|Day when the Knowledge was created|
|Document type(*)|Category that defines the type of document - there may be more (or less) options in this list (check Active Domains). By default, we have several options to select: *Document, FAQ, Known Error, Test Evidence, Recovery measure, Emergency Response Plan, Damage Evaluation Plan, Rescue Plan, Vitar Records Plan, Crisis Management and Public Relationships Plan, Accommodation and Services Plan, Communication Plan, Finances and Administration Plan, Service Quality Plan, Availability Plan, News*|
|Expiration Date(*)|Date when the knowledge becomes obsolete|
|Folder(*)|Place where the knowledge will be saved. By default, we have the options: *Service Desk, FAQ, For Approval, Partner Portal*|
|Legislation|Indication if knowledge is (or makes) part of some legislation|
|Observation|A description of the knowledge|
|Origin(*)|Trigger for the creation of a Knowledge. By default, we have the following options: *Knowledge, Event, Change, Incident, Service, Problem, Quality, CMDB & ITAM, Events, Availability and Release*|
|Privacy|Information sensitivity: **Confidential** (only the author of the knowledge and the folder administrator will have access to the knowledge), *Internal* (only people who have permission in the folder will have access to knowledge) and *Public* (internal/external) (everyone will have access to knowledge, even those who do not have permission in the folder)|
|Publication Date (automatic)|Day when the Knowledge was published|
|Publisher|The responsible for publishing the Knowledge|
|Source/Reference|Inform the source/reference of the knowledge. By default, we have the following options: *Development, Build, Systems integration testing, User acceptance testing, Production*|
|Status (automatic)|Knowledge lifecycle status|
|Tags|Words (or set of words) used to help the search engine|
|----------|All knowledge that changes will be submitted to an approval flow (controlled by the change or service request)|

(\*) Indicate mandatory field

!!! note "NOTE"
    
    If the option for known error is selected in the document type field, the system will present a field to define which environment this knowledge should be linked to (Production or development)
    
!!! note "NOTE"

    If the option for known error is selected in the document type field, the system will present a field to define which environment this knowledge should be linked to (Production or development)

#### Knowledge Content

A WYSIWYG editor is available to work with the HTML content of a document. In it, the Manager can insert and edit the text, images, videos, hyperlinks and others.

    • To add a link (hyperlink) to the knowledge content, in order to access an external link, select a word or phrase and click on the “Insert/Edit link” button (the chain icon), complete the fields and click on “OK”;

    • To add an image to the knowledge content, click on the “Image” button (the landscape icon) or copy and paste the image saved to a file on your computer;

    • To add a video, click on the “Insert a video” button:

    • In the Server video tab: it allows to insert a video that is located on the video server or on the computer;
    
    • In the Embedded tab: it allows to insert YouTube videos. When accessing the video, right-click and select “Copy embed code”.


### Saving

When creating a knowledge, 4biz will always establish version "1.0" and, when changing a document, the operator can indicate whether the change should be Versioned or not and also if previous versions must be archived.

!!! abstract "NOTE"

    The tool will inform in a pop-up, if there's an article with the same name you're creating in the Knowledge Base.

### Tips

!!! warning "ATTENTION"
    
    Pay attention when using “Public” privacy, as there is a risk of making documents available prior to their proper evaluation and approval. This scenario disregards the access profile configuration and releases document access for all users.

!!! note "Approval Tracker"
    
    The end user can propose new Documents/Knowledge by using the floating button of the Knowledge Portal. The Document will be saved in the folder indicated by Parameter 313 of the system. The knowledge Manager searches for unpublished documents or in the indicated folder and, as the approval progresses, the document will move to other statuses.

### Related

[Creating folder](/en-us/4biz-helium/processes/knowledge/configuration/create-folder.html)

[Configuring external access to Knowledge Portal](/en-us/4biz-helium/processes/knowledge/configuration/configure-external-access-knowledge-portal.html)


!!! tip "About"

    <b>Product/Version:</b> 4biz | 8.05 &nbsp;&nbsp;
    <b>Updated:</b>30/03/2021 – Andre Fernandes
    
[1]:https://en.wikipedia.org/wiki/WYSIWYG
[2]:/en-us/4biz-helium/initial-settings/access-settings/profile/create-profile-access.html
[3]:/en-us/4biz-helium/platform-administration/email-settings/email-templates-configure-email-template.html
[4]:/en-us/4biz-helium/platform-administration/parameters-list/configure-parametrization-knowledge.html
[5]:/en-us/4biz-helium/platform-administration/email-settings/key-field/knowledge-base-email.html
[6]:/en-us/4biz-helium/platform-administration/email-settings/key-field/knowledge-base-email.html#exemplos-de-utilizacao
