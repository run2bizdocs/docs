title: Register Nagios manager
Description: Register and maintain the managers that will be responsible for monitor the configuration items and event occurrences captured from Nagios.
# Register Nagios manager

Nagios is a network monitoring tool. It can monitor both hosts and services,
warning when happening the problems and also when the problems are solved. The
Hosts are equipment and Services are resources offered by the equipment.

The objective of this functionality is to register and maintain the managers that
will be responsible for monitor the configuration items and event occurrences
captured from Nagios. It allows the user to inform when the Manager will be
processed, which configuration items will manage and the actions to be taken
automatically.

This feature provides a variety of actions, such as including, changing, and
deleting a Nagios manager.

Before getting started
--------------------------

- [x] It's necessary to previously register the 4biz Event Monitor connection, 
time, occurrence category, automatic action and the 4biz Inventory connection.

Procedure
-------------

1.  Access the functionality through the main menu Processes \> Event Management
    \> Nagios \> Nagios Manager;

2.  Complete the fields for Basic Data, Scheduler Data, Configuration Item Parent and Configuration Item Child;

3.  In the parent configuration item area, it's possible to register the CI in
    4biz with the data of the Host selected. Click on "Create CI". Remember
    that this registration can only be made if there is no CI with the same Host
    identification:

    - Enter the data of the child configuration item;

    - Conduct a relationship between the Host service and the child configuration
    item. Each host service must be related to its respective child
    configuration item.

1.  Click on "Save".

Related
-------

[Register occurrence category](/en-us/4biz-helium/processes/event/configuration/register-occurence-category.html)

[Register Event Monitor Connection](/en-us/4biz-helium/processes/event/configuration/register-event-monitor-connection.html)

[Register Nagios/Zabbix connection](/en-us/4biz-helium/processes/event/configuration/register-nagios-zabbix-connection.html)

[Register time](/en-us/4biz-helium/processes/event/configuration/register-time.html)

[Register automatic action](/en-us/4biz-helium/additional-features/automation-of-operation/configuration/register-automatic-action.html)
