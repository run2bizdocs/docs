title: Service level agreement
Description: Allows to register the service level agreement of type availability, time (by phases) and miscellaneous information captured from other sources
# Service level agreement
This functionality allows to register the service level agreement of type *availability*, *time* (by phases) and *miscellaneous information captured from other sources*.

After N minutes (informing the time of action) and in case there is no action performed in the linked service request to this SLA, the system will attribute the priority and will escalate the group to execute the service request.
This feature provides a variety of actions, such as including, changing, and deleting a service level agreement.

Before getting started
--------------------------

- [x] A previously registration of priority, group, unit, user is needed  alse the definition of e-mail templates and service
level requirements.

## Procedure

1.  Access the functionality Service Level Management through the main menu
    Processes \> Service Level Management \> Service Level Agreement;

1.  Click on the desired Tab (Search / Registration) and action;

| Function   | Description           |
|------------|-----------------------|
| **Save**   | Save the new SLA      |
| **Delete** | Delete the SLA Edited |
| **Clear**  | Clear all Form Fields |

!!! warning
    
    If the type of agreement entered is Time (by phases), set the SLA deadlines (service level agreement), takin into consideration the priority. The priority goes from 1 to 5, being 1 the highest level and 5 the lowest.

4.  Click on "Save".

## Search

**Select the SLA to search for:**

| **Filter**        | **Description**                                                                                                                                       |
|-------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| Title             | Title to search                                                                                                                                       |
| Status            | Active / Inactive                                                                                                                                     |
| Type of Agreement | “Time(By Phases)”, Availability, ”Miscelaneous Information”                                                                                           |
| Grid              | SLA searched with the criteria with A selection radio button, Title, Situation ( “A” Active or “I” Inactive) Start Date, End Date, Date of Evaluation |

## Register

### Basic data

1.  Complete the SLA Basic Data:

| **Basic Data Fields**   | **Description**                                                                                          |
|-------------------------|----------------------------------------------------------------------------------------------------------|
| Title (\*)              | Title of identification of the SLA                                                                       |
| Type of Agreement (\*)  | “Time (By Phases)”, Availability, ”Miscellaneous Information”                                            |
| Seasonality             | Describe if this SLA will be used from time to time                                                      |
| Impact                  | Define the SLA impact between "High", "Low" and "Medium"                                                 |
| Urgency                 | Define the urgency of the SLA between "High", "Low" and "Medium"                                         |
| Change impact / Urgency | Inform if the impact or urgency can be changed in a Incident or Service request registration (Yes or No) |
| Status                  | Active / Inactive                                                                                        |
| Description             | Relevant description for using the SLA                                                                   |
| Scope                   | Scope to the SLA                                                                                         |
| Start date (\*)         | Set the start date of SLA                                                                                |
| End date                | Set the end date of SLA ( mandatory if Seasonal is checked)                                              |
| Evaluates on            | Set the date to evaluate this SLA                                                                        |
| Contacts                | Contact for the SLA                                                                                      |

!!! Note "Scope - Change blackout periods"
   
    Change Management to provide access to Service Level Agreement details, implementation windows, change blackout periods, and availability requirements

### Targets

2. Complete the **targets for published time of this SLA**

| For each Priority | The Priority go goes from 1 to 5, being 1 the highest priority and 5 the lowest |
|-------------------|---------------------------------------------------------------------------------|
| Capture Hour      | Enter the SLA "capture" and "Resolution" time                                   |
| Capture Minute    | Enter SLA "capture" and "Resolution" minutes                                    |



### Automation

3.  Complete the Automation Fields ( if it´s needed):

| Automation Fields | Description                                                                |
|-------------------|----------------------------------------------------------------------------|
| Time of Action    | Time after a scenario is true for the execution of an automatic action     |
| Priority          | The new priority that the service that will be scheduled will receive;     |
| Group             | Group to whom the assistance will be directed after the scheduling action; |
| Email Template    | Email Template used to send Notifications                                  |

!!! warning

    Before complete the fields in **Automation**, it must be properly parameterized, so it is necessary to execute the steps in the knowledge Creation escalation rule, except for parameter 190 that must be equal to 'N' in this context;

### Unit Priorities

4.  Complete the Unit priorities:

| Fields                                      | Description                                                                                                                             |
|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Search Unit (\*)                            | Search                                                                                                                                  |
| Unit (only for "Client" or "Specific") (\*) | Unit and it´s permission for the SLA, (Select a unit and the system will make a Grid with the selected unit and the priority assigned ) |

(\*) Indicate mandatory field

### User Priorities

5.  Complete the **User priorities**:

| User (Only for "Client" or "Specific") (\*) | User and it´s permission for the SLA (select an User and the system will make a Grid with the selected employee and his priority assigned ) |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|

## Additional Information

### Service Level Agreement (Link) Requirements

Link a Service Level requirement to the SLA   
- Date of Link* - Date of the linking between the SLA and the Service Level requirement  
- SLA Requirement* - Name of the Service Level requirement  

(\*) Indicate mandatory field

!!! Note
   
    The information will be consolidated at the [SLA Evaluation Report] (/en-us/4biz-helium/processes/portfolio-and-catalog/use/SLA-evaluation.html)

### Client Contract

The system will show the contracts linked to the SLA in a Grid (with a treeview of services of the contract, number, Contract Date, Client, Provider, Status)

### Operational Level Agreement

The system will show the history of the SLA in a Grid (with a treeview of services of the Operational Level Agreement, number, Contract Date, Client, Provider, Status)

### Underpinning Contract (Third Party)

The system will show the contracts linked to the SLA in a Grid (with a treeview of services of the contract, number, Contract Date, Client, Provider, Status)

### Audit History

The system will show the contracts linked to the SLA in a Grid (with a treeview of Histories of the SLA, Title, Start Date, End Date, Evaluate On,	Status, Modified By, Modified On)

The treeview  will show description, Scope, Default, Type and Priority, Time and Log data)

### Review SLA

Inform Review Data for the SLA:   
- Review Date* - Date for the review  
- Review Details* - Detail to be reviewed
- Observation - - Observation to the review  
- Add Function  
- Grid with Reviews

### Service Quality Plan

Inform Service Quality Plan to be linked to the SLA:   
- Service Quality Plan*  
- Service Quality Plan  
- Add Function   
- Grid with Service Quality  


## Related

[Register priority](/en-us/4biz-helium/processes/portfolio-and-catalog/configuration/register-priority.html)

[Register group](/en-us/4biz-helium/initial-settings/access-settings/user/register-groups.html)

[Create template of incident, request and procedure](/en-us/4biz-helium/processes/tickets/configuration/create-template-of-ticket.html)

[Service level requirement](/en-us/4biz-helium/processes/service-level/use/service-level-requirement.html)

[Register user](/en-us/4biz-helium/initial-settings/access-settings/user/users.html)

[Register unit](/en-us/4biz-helium/platform-administration/region-and-language/register-unit.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RNz3E16sjg5mfdugX2Ia9jZ)'

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021

