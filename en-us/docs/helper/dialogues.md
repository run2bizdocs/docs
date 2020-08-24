Title: Dialogs

# Dialogs

Helper learns from the **dialogs** added to its knowledge base. These dialogs are structured by **interests or intentions** (possible phrases used in the user's interaction) and **skills** (possible responses of the virtual assistant to the user's interactions).

As Helper works reactively to user interactions, to form dialogs we need to group interests and skills in pairs. Contexts will be used only when, during the dialog, it's necessary to store some information cited by the user to be used in another point of the conversation. 

It is up to the administrator of the virtual assistant to supply this data to the system, structuring the possible dialogs and training. The training must be scheduled through the Helper interface, and at the end of the training, your assistant will be updated automatically. 

## Adding Dialog

**Procedure**

1.  After accessing the platform, go to the menu "Dialogs”;

2.  First, it'll be presented the following options:

|Field|Description|
|-|-|
|New|To create a Dialog|
|Search|To search for a Dialog already registered|

3\.  To view or edit a “Dialog” already registered, search for a specific one or find it in the list presented;

4\.  To create a new dialog, click on “New” and complete the information as needed:

|Field|Description|
|--------------------------------|-------------------------------|
| Name| To identify the general tenor of the user's subject. It'll be the name for the dialog that the administrator can use for a given context.|
| Theme| Depending on the type of the attendance and services that the chatbot will perform, the themes will classify the type of conversation.|
| Add Dialog| The option to add dialog is used to add a new dialog to the theme.|
| Link Intent| The option to link Intent is used to add an intent to the dialog, thus being able to specify it and link it to a specific context.|
| Link main dialog | If there is already a previously created dialog and you want to reuse its behavior for the dialog being created, just click on “Link main dialog”. |

5\.  To save a new dialog click on "Save", or if you want to return to the initial dialog screen, click on "Back".

## Link maind dialog

If there is already a previously created dialog and you want to reuse its behavior for the dialog being created, just click on “Link main dialog”.

It'll be presented the following options:

|Field|Description|
|-|-|
| Dialog | To search for the dialog already created in the tool to be linked. |
| Add | To add the selected dialog.|
| Close| To return to the previous page.|

When linking this dialog, the chatbot will take into account the flow of information you were already registering, in addition to the behavior of this new dialog that was linked.

Once the link is made, you can edit or delete this dialog in the list presented in the option “Dialogs”.
