Title: Settings

# Settings

## Parameters

## What is accuracy?

We can understand it as the level of understanding of what the user is saying to the assistant, if the text typed by the user needs to be exactly the same as the one built or if after a certain point of understanding of the text, the assistant can already follow the conversation flow planned.

The assistant will only continue the dialogue if the accuracy of understanding of the phrase entered by the user is greater than the value registered on this page. Otherwise, the virtual assistant will start the registered fallback flow.

**Example:** Let's suppose that in the dialogue it was created the greeting “Good morning!” and its accuracy is set to 100%. If the user writes "good morning?" your assistant will not understand what was said and will display a fallback message. The conversation flow will only be continued if the user types “Good morning!”, exactly as it was created.

The better your examples of dialogues and records of intentions, the better your assistant will be. So it's important to define what scenario the assistant will act on before defining the level of accuracy. See the reason below:

## Levels of accuracy:

|Level of accuracy|Risks|
|-|-|
| Between 0% and 30%   | In general we consider it low, and therefore, there is little certainty that the dialogues will correspond to what was planned. When it comes to identity and login validations the risk is high for your organization. |
| Between 30% and 70%  | They are considered medium, presents moderate risk. Depending on the level of information they will validate, it may be worthwhile.|
| Between 70% and 100% | Represents low risk and greater chances of accuracy of the information.|

## Notifications

Area for managing which system administrators need to receive notifications about the assistant updateArea for managing which system administrators need to receive notifications about the assistant update.

Three types of notifications are sent:

|Type|Description|
|-|-|
|Scheduling started| Email sent to notify that the scheduled training has started.|
|Training completed | Sent when training has completed successfully and the assistant is available with the new learnings.|
|Failure in the process| Notifies the platform administrator that the update could not be performed, the reason and the solution. Example: Training not performed. You need to register three more phrases in the intent, as the minimum of phrases to update is four phrases.|

**Procedure**

1.  In the “Type to add an email” field, type the email that will receive notifications;

2.  Click on Add;

3.  Once added, it's possible to delete the email.

## Migrations

This area allows you to use the case or scenario built in IBM Watson on Helper, without the need to reconstruct the conversation flows on this platform.

**Procedure**

1.  Click on the IBM Watson option;

2.  On the Settings tab, complete the fields API Key, URL, User, Password and Version with this data provided on the IBM Watson platform;

3.  The Workspaces available for importing from the IBM Watson platform will be displayed on the Imports tab;

4.  Select the Workspace you want to import;

5.  Click on Save;

6.  The Import History tab will show the name of the imported workspace, the date of import and status of the import.

!!! warning  "Attention"

    It may happen that the type of phrase or option is not compatible with the Helper and for this reason the importation of this item only will not occur. In this case it'll be necessary to check and manually create the non-imported section.

## Importat/Export

In this area it's possible to import dialogs by intent and export the existing dialogs in your assistant as well.

It's still necessary to schedule a training after importing the dialogs so that Helper learns these imported dialogs too.

### Procedure to export

1.  Click on export;

2.  The system will start the file download process, which will be delivered in .xlsx format.

### Procedure to import

1.  In an .xlsx spreadsheet, create three columns in this order: Intent, User Says, Text Response;

|Column|What to complete|
|-|-|
|Intent| Name of the intention registered in the Helper. Example: 1.0 Greetings to the Logged User|
| User says | What the person being assisted by the assistant can say. Each hypothesis being on a different line. Example: Hello, good night|
| Text Response | What the assistant must respond to this speech. Example: Hello, I'm Helper, your new virtual assistant. I'm here to simplify your service process and help you with your needs. Just write what you need and I'll help you!|

**Example:**

1.  Save the spreadsheet;

2.  Back to the Import/Export page, click on Import;

3.  Click on choose file;

4.  Find the spreadsheet saved;

5.  Click on Import.

!!! info "Observation"

    -   Only responses in text format can be imported. The other options (button, image and carousel) are not yet available in this functionality;
    -   If you want to refine existing dialogs, export, adjust, and import again. The import replaces the content, so if you remove any existing sentence in the spreadsheet that was exported, when it's imported the system will delete the phrase (s) removed from the spreadsheet.


!!! success "Tip"

    Use the service procedure (FAQ) that your organization already has (if you have one) in question and answer format to assemble this spreadsheet. Take advantage of the knowledge that already exists in your environment to enhance your virtual assistant.
