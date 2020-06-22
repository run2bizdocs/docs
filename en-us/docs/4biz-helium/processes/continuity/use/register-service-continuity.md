title: Register service continuity
Description: Allows to register the continuity of a certain service.

# Register service continuity

The Continuity Management focuses on the recovery of IT services and its components in face of an event of disaster.
This functionality allows to register the continuity of a certain service.

## Before getting started

- [x] The existence of a defined service in a Portfolio and Catalog Management process.

- [x] It's necessary to previously register the threat and threat category, both
linked to each other, in addition to previously register the risk and risk
category.

- [x] It's equally necessary to have registered the automatic actions of Incident,
Request and Procedures about the Event Management.

## Procedure

1.  Access the functionality through the main menu Processes \> Continuity
    Management \> Continuity;

2.  Click on "Continuity Registration" and complete the fields:

|Field|Description|
|-----|-----------|
|**Name(\*)**|The name for the continuity|
|**Client(\*)**|Set the client for this continuity|

(\*)Indicate mandatory fields.

Once created the continuity, in the list provided, find the one you want and click on Advance to complete all the information about the continuity.

### Initiation

In the initiation phase, set the fields for the tabs Policy, Scope and Project.

**Policy**

|Field|Description|
|-----|-----------|
|**Title(\*)**|The title for the policy|
|**Version(\*)**|The version of the policy|
|**Expiration date(\*)**|The date that expires the policy|
|**Description**|The details about the policy|
|**Assignment(\*)**|Assign the people for the policy|
|**Attach**|To add files for the policy|

(\*)Indicate mandatory fields.

**Scope**

|Field|Description|
|-----|-----------|
|**Executive summary(\*)**|Detail the executive summary|
|**Description(\*)**|Describe the informations about the scope|
|**Expiry date(\*)**|The date that'll expire the scope|
|**Attach**|To add files for the scope|

(\*)Indicate mandatory fields.

**Project**

|Function|Description|
|--------|-----------|
|**Link Project**|To link a project already existed|
|**Create New Project**|To create a new project to the continuity, complete the fields: Name, abbreviation, contract, emergency, severity, name of manager, change, release, status, value for project execution, detail/supplementary instructions. It's necessary to add other information, they are: Resources, Subscriptions and Approvals, Work Order and Baseline|

### Requirements and Strategy

In the requirements and strategy phase, set the fields for the tabs Vital Functions, Business Impact Analysis, Risk Assessment and IT Service Continuity. 

Choose the service on the list of service by criticality, than, choose the viatal function.

**Vital Functions**

|Funtion|Description|
|-------|-----------|
|**Add vital function**|To select a process to link to the continuity|
|**Attach**|To add a file|
|**Delete**|To delete the vital function linked|

**Business Impact Analysis**

Once selected the Vital Function, click on the icon "+" and complete the fields.

|Field|Description|
|-----|-----------|
|**Possible impacts**|Select the possible impacts for that|
|**Gravity**|Set the degree of severity for this vital function|
|**Recovery point purpose**|Set the recovery point|
|**Purpose of recovery time**|Set the time of recovery|
|**Cost by hour of inactivity**|Set the cost for inactivity|
|**Maximum tolerable of inactivity**|Set the time tolerable for inactivity|
|**Cost of impact**|Set the cost of its impact|
|**Strategy 1,2 and 3**|Describe the strategies for each one of them|

**Risk Assessment**

On the Risk assessment phase, it'll be made the evaluation of the risk. Here you can add possible scenerios for the risks. We have the following functions:

|Function|Description|
|--------|-----------|
|**Add scenary**| To add a possible scenary of risk. Complete the mandatory fields: Name and vital function|
|**Add service**|To add a service available for your profile to the risk. You can delete it too|
|**Add risk**|Select the risk you want to link. Once linked the risk, it's possible to **Select threat** or **Add Threat**. When adding a threat, complete the mandatory fields: Threat Name and Threat Category. Next the Treats tab, there's the **Treatment Plans** to add a treatment plan for the risk|

**IT Service Continuity**

|Field|Description|
|-----|-----------|
|**Select Vital Function**|Select the vital function, it'll have the following actions: Services - to see the services of the vital function; Scenarios - To view the scenarios of vital function; Delete - To delete the vital function|
|**Recovery measures**|Stablish the recovery measures|
|**Risk response measures**|Stablish the risk response measures|

*Critical Service*

The tool will present a list of critical services associated with vital business functions. This information is also available in the [BI report](https://documentation.run2biz.com/en-us/4biz-helium/additional-features/smart-analytics/use-bi-solution.html).

### Implementation

In the implementation phase, set the fields availble in the tabs: Continuity Plan, Organizational Planning and Test Strategy.

**Continuity Plan**

|Fields|Description|
|------|-----------|
|**Title(\*)**|The title for the continuity plan|
|**Version**|The version for the continuity plan|
|**Status(\*)**|Set the status of the plan|
|**Description**|Describe the plan|
|**Continuity Procedure(\*)**|Add the continuity procedure|
|**Assignment(\*)**|Assign the people for this plan|
|**Validity(\*)**|The date for the expiration of the plan|
|**Authorization(\*)**|Set if is authorized or not|
|**Related Change**|Relate a change for the plan|

(\*)Indicate mandatory fields.

|Action|Description|
|------|-----------|
|**Relate Knowledge**|To link a document to the plan|
|**Relate Recovery Measures**|To link recovery measures|
|**Attachments**|To add files|

**Organizational Planning**

After describe the executive summary, which is mandatory, we have the following levels:

|Level|Description|
|--------|-----------|
|**Executive Committee**|To add the group and responsibility. Both are mandatory|
|**Coordination**|To add the group of coordination. The fields group and responsibility are mandatory|
|**Recovery Teams**|To add the group of recovery. The fields group and responsibility are mandatory|

**Test Strategy**

|Field|Description|
|-----|-----------|
|**Name(\*)**|Identify the test with a name|
|**Executive summary(\*)**|Describe the executive summary|
|**Attachments**|To add files to the test|
|**Select recovery measures**|To search for and select a recovery measures for the plan|

(\*)Indicate mandatory fields.

### Continuous Operation

In the continuous operation phase, set the fields availble in the tabs: Awareness, Review and Audit, Tests and Invocation.

**Awareness**

After describe the Executive summary, which is mandatory, it's possible to complete the Training Registries. Click on Add Register and complete the fields:

|Field|Description|
|-----|-----------|
|**Critical Analysis of Action(\*)**|Make a critical analysis of the action|
|**Type of Activity(\*)**|Select the type of activity|
|**Status(\*)**|Select the status of the activity|

(\*)Indicate mandatory fields.

**Review and Audit**

On the Registered Audits tab, you can search for an audit already created by Period and Category. It'll appear the audits in the list.

To register an audit, complete the fields:

|Field|Description|
|-----|-----------|
|**Category(\*)**|Select the category of the audit|
|**Description(\*)**|Describe the audit|

**Tests**

Select one day in the calendar and complete the fields for the tabs:

|Tab|Description|
|---|-----------|
|**Main informations**|Describe the test information, completing the fields: Event Name, Start Date/Time, End Date/Time and Details|
|**Group**|Add a group|
|**Employee**|Add an employee|
|**Test evidence**| Select or create a test evidence|
|**Test plans**|Add a test plan|

!!! abstract "NOTE"

    Those informations and tests are used to predict the services and generate predictive reports.


After complete all the information for each phase of the continuity registration, click on "Save".

Related
-----------

[Register threat](/en-us/4biz-helium/processes/continuity/configuration/register-threat.html)

[Register threat category](/en-us/4biz-helium/processes/continuity/configuration/threat-category.html)

[Register risk category](/en-us/4biz-helium/processes/continuity/configuration/risk-category.html)

[Register service continuity scope](/en-us/4biz-helium/processes/continuity/use/service-continuity-scope.html)

[Register continuity risk](/en-us/4biz-helium/processes/continuity/configuration/register-continuity-risk.html)

[Define service continuity policy](/en-us/4biz-helium/processes/continuity/use/continuity-policy.html)

[Define service continuity project](/en-us/4biz-helium/processes/continuity/use/service-continuity-project.html)

[Register automatic actions of incident/request/procedure](/en-us/4biz-helium/additional-features/automation-of-operation/configuration/register-automatic-actions-incident-request-procedure.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RPwpIsGu97d5LVHeTNzpTMC)'

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020


