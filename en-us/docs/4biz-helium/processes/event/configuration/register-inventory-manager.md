title: Register Inventory manager
Description: Register and maintain the managers who will be responsible for the occurrences of events captured from 4biz Inventory.

Register Inventory manager
==========================

The purpose of this functionality is to register and maintain the managers who
will be responsible for the occurrences of events captured from 4biz Inventory.

It allows the user to indicate how much time the Manager will be processed, what
configuration items it will manage, the checks that will be applied and the
actions to be automatically taken.

This feature provides a variety of actions, such as including, changing, and
deleting Inventory manager.

!!! faq "Do you know?"

    The automatic actions are workflows related to process to facilitate the resolution of events.  
    The configurations of automatic actions are described further in this document and should be used according to each type of classification of event/configuration item.

Before getting started
----------------------

- [x]  To register the Inventory manager, it's necessary to previously register the
    4biz Event Monitor connection, time, occurrence category, automatic action
    and the 4biz Inventory connection.

Procedure
---------

1.  Access the functionality through the main menu Processes \> Event Management
    \> Inventory Monitor \> Inventory Manager;

2.  Click on the desired Tab (Search / Register) and function;

| Function   | Description               |
|------------|---------------------------|
| **Add**    | Add Managers to the grids |
| **Save**   | Save the Managers         |
| **Delete** | Delete the Manager Edited |
| **Clear**  | Clear all fields from the Form |

Search
------

**Select the filter to search for:**

| **Filter** | **Description**         |
|------------|-------------------------|
| Name       | Name to search          |
| Grid       | Grid with search result |

Register
--------

### BASIC DATA

1.  Complete the Basic Data:

| **Data Fields**      |
|----------------------|
| name (\*): Name of the connection |
| Connection Inventory: Source of monitoring data coming from external or internal tools |

### SCHEDULER DATA

| **Data Fields**            |
|----------------------------|
| Enable/Disable AutoCorrect |
| Time for event closure     |

!!! NOTE

    The autocorrect function is used to archieve events and automaticaly close incidents related to them.  
    The autocorrection depends on the value of the "Time for event closure" field, which means the interval of time to check for new evetns.

### CONFIGURATION TYPE FOR CONFIGURATION ITEMS

| **Data Fields**                                                 |
|-----------------------------------------------------------------|
| Configuration Type(Specific Configuration, General Settings) |

### CONFIGURATION ITEM PARENT

| **Data Fields**                          |
|------------------------------------------|
| Configuration item parent                |
| Category of occurrence group             |
| Category of occurrence                   |
| Generate occurrences of Up? (Yes / No )  |
| Action for up (Only register event)      |
| Urgency (Low/ Medium / High)             |
| Impact (Low/ Medium / High)              |
| Generate Down occurrences? ( Yes /  No ) |
| Action for down (Only register event)    |
| Urgency (Low/ Medium / High)             |
| Impact                                   |

### CONFIGURATION ITEM CHILD  OR  TYPE OF CONFIGURATION ITEM

| **Data Fields**                                                               |
|-------------------------------------------------------------------------------|
| Configuration Type ( Configuration item child/Type of Configuration Item)     |
| Configuration item child                                                      |
| Check                                                                         |
| Category of occurrence group                                                  |
| Category of occurrence                                                        |
| Generate occurrences of Information? Yes No                                   |
| Condition for Information                                                     |
| Action for information                                                        |
| Urgency  (Low/ Medium / High)                                                 |
| Impact (Low/ Medium / High)                                                   |
| Generate Warning occurrences? ( Yes /  No )                                   |
| Condition for Warning                                                         |
| Action for warning                                                            |
| Urgency (Low/ Medium / High)                                                  |
| Impact (Low/ Medium / High)                                                   |
| Generate Exception occurrences?  ( Yes /  No )                                |
| Condition for Exception                                                       |
| Action for exception                                                          |
| Urgency (Low/ Medium / High)                                                  |
| Impact (Low/ Medium / High)                                                   |
| Configuration Type: Configuration item child or Type of Configuration Item    |
| Configuration item child                                                      |
| Check                                                                         |
| Category of occurrence group                                                  |
| Category of occurrence                                                        |
| Generate occurrences of Information( Yes /  No )                              |
| Condition for Information                                                     |
| Value                                                                         |
| Action for information                                                        |
| Urgency (Low/ Medium / High)                                                  |
| Impact (Low/ Medium / High)                                                   |
| Generate Warning occurrences? ( Yes /  No )                                   |
| Condition for Warning                                                         |
| Value                                                                         |
| Action for warning                                                            |
| Urgency (Low/ Medium / High)                                                  |
| Impact (Low/ Medium / High)                                                   |
| Generate Exception occurrences?  ( Yes /  No )                                |
| Condition for Exception                                                       |
| Value                                                                         |
| Action for exception                                                          |
| Urgency (Low/ Medium / High)                                                  |
| Impact (Low/ Medium / High)                                                   |

(\*) Indicate mandatory field

!!! faq "Do you know?"

    For each block of information (Configuration Item Parent, Configuration Item Child or Type of Configuration Item), the follow configuration has the same meaning and values:   
    Action (Create incident, problem, change or send notification, Impact and Urgency to define the priority/criticity).  
    While there is a logged or in execution event, for a service or CI and new incidents occur, the tool will not duplicate the main event. The additional incidents will be linked to the main one. If the main event is arhived, a new one will be created.

1.  Complete the fields available in each area;

2.  The completion fields will be changed as the *type of configuration* chosen:

    - **Specific Configuration:** it allows to create specific rules to a single
    configuration item. Those rules will be applied when the configuration item
    is being inventoried;

    - **General Settings:** it allows to create rules to all configuration items.
    Those rules will be applied when the configuration item is being
    inventoried.

3.  Ente the data necessary and click on "Add";

4.  Click on "Save".

Related
-------

[Register occurence category](/en-us/4biz-helium/processes/event/configuration/register-occurence-category.html)

[Register Event Monitor Connection](/en-us/4biz-helium/processes/event/configuration/register-event-monitor-connection.html)

[Register time](/en-us/4biz-helium/processes/event/configuration/register-time.html)

[Set Inventory connection](/en-us/4biz-helium/processes/event/configuration/set-inventory-connection.html)
