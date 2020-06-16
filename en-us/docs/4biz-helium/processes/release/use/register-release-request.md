title: Registering release
Description: This functionality makes available several actions, like, include, change and delete a release. 
# Registering release
According to ITIL, release is "one or more changes to an IT service that are built, tested and deployed together. A single release may include changes to hardware, software, documentation, processes and other components".
This functionality makes available several actions, like, include, change and delete a release.

## Before getting started

- [x] Purchases/Provisioning must be initialized in a service request (in a specify service catalog )
The service request must be check in CMDB if it´s license, hardware, or specific item requested is available. 
Only after this procedure the release will be created;

- [x] It's necessary to have a registered RFC (request for change);

- [x] It's necessary to have previously registered the release portfolio, the employee,
contract, unit linked to the contract, executor group linked to the contract,
type of release and periodic activity group

## Procedure

1.  Access the functionality through the main menu Processes \> Release
    Management \> Release;

2.  Click on the options button “Options” and then on "Register";

3.  At the beginning of the page, we have the following information:

|Information|Description|
|-----------|-----------|
|**Number**|The number that'll identify the release|
|**Phase**|The release phase|
|**Priority**|The priority of the release when creted|
|**Current group**|The group responsible for the release when created|
|**Assignment**|The person who will be responsible for the release|
|**View flow**|These are the status of the workflow release, which will change according to the release maintenance. It'll appear when you edit or execute the release already created. The status of the flow are: Release, Run, Test, Homologation and Solved. There are checklists for workflow enforcement to link specific item for each phase/steps/status of the workflow|
|**Execution registration**|This information will appear after created the release, and will present history information about the release|

## Identification Fields

When creating a release, complete the fields for the identification.

|Field|Description|
|-----|-----------|
|**Name(\*)**| Identify name of the requester|
|**Contact(\*)**|Inform the contact for the requester|
|**E-mail(\*)**|The e-mail of the requester|
|**Phone**|The phone number of the requester|
|**Extension**|The extension number of the requester|
|**Unit(\*)**|The unit of the requester|
|**Physical Location**|The location of the requester|
|**Other information**|All other information you think is important about the requester|

(\*) Indicate mandatory field

### Release

|Field|Description|
|-----|-----------|
|**Search here**|To search for the portfolio you want|
|**Portfolio(\*)**|Select the portfolio of the release you're creating|
|**Model(\*)**|Select the model of the portfolio of the release|
|**Title(\*)**|The title for the release you're creating|
|**Contract(\*)**|The contract related to the portfolio selected|
|**Executor Group(\*)**|The group responsible to deal with the release|
|**Impact(\*)**|Set the degree of the impact|
|**Urgency(\*)**|Set the degree of the urgency|
|**Risk(\*)**|Set the degree of the risk|
|**Release Date**|Set the date for the release|
|**Version**|The version of this release|
|**Notifications**|The types of notification regarding the maintenance of the release|

(\*) Indicate mandatory field

!!! faq "Do you know?"

    According to the portfolio, the types of release can be **Minor, Major, Significant and Emergency**.
    
    **Minor release** is a release of a product that does not add new features or content, maintenance releases are typically intended to solve minor problems, typically "bugs" or security issues.
    
    **Major release** means a new version of Software that includes changes to the architecture and/or adds new features and functionality in addition to the original functional characteristics of the preceding software release.
    
    **Signifcant release** adds features and functionality improving overall product performance, efficiency and usability.
    
    **Emergency release** are exactly what they sound like. Some incident or scenario needs attention ASAP, so will be released a temporary fix.

### Changes

|Function|Description|
|--------|-----------|
|**Search Change**|To link a change already created, use this search box and select it|
|**Register Change**|To create a new change for this release, click here and it'll be redirected to the screen of change registration|

### Planning

|Tabs|Description|
|----|-----------|
|**Activities**|Create a new workspace or link an existing one|
|**Roles/Responsibilities**|Assign the roles and responsibilities according to the needs|
|**System notifications**|Set up a system notification to inform you about the release|
|**Documents**|To add documents for identification and control of all aspects of a release package such as software, hardware, documentation, training requirements. You can also add legal documents and general document to control|
|**More**|Two more options for the planning phase|
|**Other information**|Set the dates for the planing: start date, start time, end date and final time|
|**Notes**|Add relevant notes for the release planning|

!!! abstract "NOTE"

    The workspaces are based on Kanban methodology to the easy and agile management of activities. Go to **Creating Kanban to the Planning and Deployment phases** to see how to create a workspace.

### Deployment

|Tabs|Description|
|----|-----------|
|**Activities**|Create a new workspace or link an existing one|
|**Roles/Responsibilities**|Assign the roles and responsibilities according to the needs|
|**System notifications**|Set up a system notification to inform you about the release|
|**Documents**|To add documents for identification and control of all aspects of a release package such as software, hardware, documentation, training requirements. You can also add legal documents and general document to control|
|**More**|Two more options for the deployment phase|
|**Other information**|Set the dates for the deployment: start date, start time, end date and final time|
|**Notes**|Add relevant notes for the release deployment|

!!! abstract "NOTE"

    The workspaces are based on Kanban methodology to the easy and agile management of activities. Go to **Creating Kanban to the Planning and Deployment phases** to see how to create a workspace.

### Linking additional items

On the left side of the screen, you can link other items to the release being created.

|Function|Description|
|--------|-----------|
|**Related CI**|Search and link CI to the release|
|**Definitive Media**|Search or create a definitive media to link the release|
|**Problem**|Search or create a problem to link the release|
|**Knowledge Base**|Search or create a document to link the release|
|**Tickets**|Search for a ticket to link to link the release|

## Creating Kanban to the Planning and Deployment phases

In the tool, the Planning and Deployment phases use Workspaces based on Kanban methodology to the easy and agile management of activities, visually organizing in a framework with cards that indicate flow progress.

This space is to detail the rollout plan, rollback, service validation, test and activities. In the Workspace, activities are inserted and grouped by projects (Workspace), task pane (Sprint) and finally tasks, which can be in groups of cards.

Moreover, you can create a Workspace for the planning or deployment phase you want, for example, for a rollout plan, you can create a workspace called "Rollout Plan" and populate with the information necessary to acomplish that, including the phases, group responsible, notes and history.

For a better understanding of how to create a workspace, or using the planning and deployment phases, see the documents:

- [Tasker Agile Management](https://documentation.run2biz.com/en-us/4biz-helium/additional-features/project-management/tasker-agile-management/simple-agile-management.html). Tasker is the functionality of the tool that creates the kanbans.

- [Activities of the release planning phase](https://documentation.run2biz.com/en-us/4biz-helium/processes/release/use/release-planning-activities.html)

- [Activities of the deployment release phase](https://documentation.run2biz.com/en-us/4biz-helium/processes/release/use/deployment-release-activities.html)

## Saving

At the end of the page, you'll find a floating button with the functions of:

|Function|Description|
|--------|-----------|
|**Cancel**|To cancel the creation of the release|
|**Save**|To save the release and create the number for tracking and monitoring|

## Editing release

Once created a release, it's possible to edit all the information we found in its registration. In addition to that, it'll appear the "Closure" phase, at the end of the page, where you can change the status of the release.

In the Closure field, at the end of the page, there's the following situation:

|Situation|Description|
|------|-----------|
|**In Execution**|To edit and see the release without finishing it|
|**Solved**|To solve and finish the release|
|**Canceled**|To cancel the release|

To see how to finish the release, see the document [Executing Release](https://documentation.run2biz.com/en-us/4biz-helium/processes/release/use/execute-release.html)


Related
-----------

[Register a contract](/en-us/4biz-helium/additional-features/contract-management/use/register-contract.html)

[Register group](/en-us/4biz-helium/initial-settings/access-settings/user/register-groups.html)

[Register employee](/en-us/4biz-helium/initial-settings/access-settings/user/register-employee.html)

[Relate information to the release](/en-us/4biz-helium/processes/release/use/relate-information-to-release.html)

[Register periodic activity group](/en-us/4biz-helium/additional-features/automation-of-operation/configuration/periodic-activity-group.html)

[Register unit](/en-us/4biz-helium/platform-administration/region-and-language/register-unit.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RMA1W1Js4-lPEDUDUJJ_rUa)'

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020

