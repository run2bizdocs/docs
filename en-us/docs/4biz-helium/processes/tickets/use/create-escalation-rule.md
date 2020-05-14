title: Create escalation rule

Description: Allows to create escalation rules in order provide a perspective of impact to the company by managing the attendance of tickets (and its requests and incidents) within a pre-established adequate time
# Create escalation rule
This functionality allows to create escalation rules in order provide a perspective of impact to the company by managing the attendance of tickets (and its requests and incidents) within a pre-established adequate time. When creating rules for the notification of the responsible when the ticket is at critical level of rupture of its SLA, is possible to avoid this through preventive actions and escalate this service to other executor groups and thus respect their time of attendance.
This feature provides a variety of actions, such as including, changing, and deleting the escalation rule.

Before getting started
--------------------------

To create escalation rules, it's necessary to set the parameter **190** with
value **Y**, and previously register the contracts, employees, groups, services
portfolios and the automatic action of escalation type.

In the file **4biz.cfg**, it's necessary configure the
properties **START\_MONITORA\_INCIDENTES** informing the parameter TRUE
(only the operating system administrator of the application server makes this
adjustment).

Procedure
-------------

1.  Access the functionality Escalation Rules through the main menu Processes \>
    Request and Incident Management \> Escalation rules;

2.  Click on "New";

3.  Enter the general data of the Escalation Rule (Title, Status, Requester, the
    attendance Executor Group, Portfolio and Contract to be linked to rule, and
    impact and urgency of ticket attendance);

4.  Enter the specific data about the Escalation Rule:  

| **Field** |                                                **Objective**                                               |
|:---------:|:----------------------------------------------------------------------------------------------------------:|
|    Time   |                      Enter the deadline for the escalation/notification of the ticket                      |
|   Format  |    Enter if the rule is regarding to minutes (time of the rule) or percentage (regarding the time o SLA)   |
| Condition | Select the mark of escalation/notification (if it will happen before or after the rupture of the deadline) |
|    Date   |   Select the date of reference rule (the date of its creation, date of last occurrence or its limit date)  |
|   Action  |                              Link the type of automatic action to the new rule                             |

Related
-----------

[Register a contract](/en-us/4biz-helium/additional-features/contract-management/use/register-contract.html)

[Create the portfolio](/en-us/4biz-helium/processes/portfolio-and-catalog/use/create-the-portfolio.html)

[Register group](/en-us/4biz-helium/initial-settings/access-settings/user/register-groups.html)

[Register employee](/en-us/4biz-helium/initial-settings/access-settings/user/register-employee.html)

[Register escalation automatic action](/en-us/4biz-helium/additional-features/automation-of-operation/configuration/register-escation-automatic-action.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RNrJnhiXj3dbmgsm9-quhfz)'

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020

