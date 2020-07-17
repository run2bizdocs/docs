title: Register Global manager
Description: This functionality is intended to create rules to monitor several types of
events
# Register Global manager

This functionality is intended to create rules to monitor several types of
events.

Each global event manager contains an EPL for *Information*, *Warning*, and/or
*Exception*. EPL is an event correlation language used by Esper (Espertech). In
the start of 4biz Event Monitor, these EPL are imported into the
Esper engine so that a new correlated event will be created each time the
condition set in the EPL is satisfied. 

Events and alerts related to: 

- Business Processes, Service Level Requirements 

- Awareness of similar and multiple events per CI or Service, 

- Connection to Incident prioritisation codes and categorizations,

- Control action, 

- Access to information on supporting and dependent CI, the Change schedule and known error information from vendors

Example of an EPL that correlates between
4biz Inventory and Nagios events: \@Description ('For any Nagios event that
occurs after any Inventory event in the last 10 minutes) select \* from pattern
[every a = EventCheckInventory- \> b = EventServiceNagios where timer: within
(10minutes)].

This feature provides a variety of actions, such as including, changing, and
deleting a global manager.

Before getting started
--------------------------

To register the Global manager, it's necessary to previously register the
4biz Event Monitor connection, time, occurrence category, automatic action
and the 4biz Inventory connection.

Procedure
-------------

1.  Access the functionality through the main menu Processes \> Event Management
    \> Global Events Manager;

2.  Complete the fields available in each area:

       - Enter the data of **Action for Information**:

         - Select the action that will be triggered when there is an event of type
           *information*, the degree of urgency and impact. The rules for this action
           are defined using the Event Processing Language (EPL). Click
           the *Validate EPL Information* button to validate the informed EPL.

       - Enter the data of **Action for Warning**:

         - Select the action that will be triggered when there is an event of type
           *warning*, the degree of urgency and impact. The rules for this action are
           defined using the Event Processing Language (EPL). Click on
           the *Validate EPL from Warning* button to validate the informed EPL.

       - Enter the data of **Action for Exception**:

         - Select the action that will be triggered when there is an event
           occurrence of type *exception*, the degree of urgency and impact. The
           rules for this action are defined using the Event Processing Language
           (EPL). Click the *Validate EPL from Exception* button to validate the EPL
           entered.


3.  Click on "Save".

Related
-------

[Register occurrence category](/en-us/4biz-helium/processes/event/configuration/register-occurence-category.html)

[Register Event Monitor Connection](/en-us/4biz-helium/processes/event/configuration/register-event-monitor-connection.html)

[Register time](/en-us/4biz-helium/processes/event/configuration/register-time.html)

[Set Inventory connection](/en-us/4biz-helium/processes/event/configuration/set-inventory-connection.html)

[Register automatic action](/en-us/4biz-helium/additional-features/automation-of-operation/configuration/register-automatic-action.html)
