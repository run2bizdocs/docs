title: Verifying Availability Process

Description: This functionality is intended to verify the availability of CI.

# Verifying Availability Process

This functionality is intended to verify the availability of CI.   

The Availability process captures incidents, releases, changes and events information to make the projection of services and events availability.  

The Creation of the availability process indicators report refers to the relationship with CMDB and Events as an information base through the association with configuration item, CI groups, Availability groups and Services. The reports facilitate the ability to calculate the reliability of components and services in terms of agreed availability targets.

The data stored in the tool can be accessible for analysis, trending and reporting using the graphical illustration of the analysis results of CI failures over a 12-month rolling window.

The reports created in the availability process are:  
- Availability by period; (This report will return: Name of CI, Group or Service,% of Measured Availability, Agreed Availability; Difference between measured and agreed availability, downtime, hourly downtime cost and total downtime cost.  
- Total availability time, total downtime and scheduled changes  
- Unavailability Occurrences
- 12-month rolling window

***All reports can be exported to Excel***.

In addition to the reported reports, there are also management reports that are made available by the BI of 4biz.

-   Mean time to repair (downtime)  
-   Mean time between failures (uptime)  
-   Mean time between Incidents  
-   Number of Service degradations  
-   Incident handling/resolution times

[See Use BI Documentation](/en-us/4biz-helium/additional-features/smart-analytics/use-bi-solution.html)

## Before getting started

- [x] Previous registration of the availability group. 
- [x] It's also necessary to link the calendar, the service level agreement of type "availability" and the cost per hour of unavailability to the: configuration item, the configuration item group and the service contract.

## Procedure

1.  Access the functionality through the main menu Processes \> Availability
    Management \> Availability;

2.  Click on the Configuration Item tab;

3.  Click on “+” symbol located on the Filters area, to search for the CI
    you want;

4.  It can be added several items, the amount you want, to the verification;

5.  Once you add the CI, you can update the charts presented after this field by clicking on "Update Charts".

6.  Verify the information in **Availability per period**. You can set the period you want and click on "Update" to view it. 

7.  Verify the information in **Total Availability**. You can set the period you want and click on "Update" to view it. You can also download it by clickin on "Save table". You can click on the slices of the chart to see the details about the CI's time distribution: Available, Unavailable and Scheduled change. In the chart, at the end, there're the followin information:

|Information|Description|
|-----------|-----------|
|Name|The name of the CI|
|Availability|The total number of the CI availability|
|Availability Agreement|It presents the total of the available agreement|
|Availability difference|It presents the total difference for the availability|
|Unavailability time|The time of unavailability|
|Unavailability cost by hour|It presents the cost of unavailability|
|Total cost of unavailability|The total for the cost of unavailability|

8.  Verify the information in **Unavailability Occurrences**. You can set the period you want and click on "Update" to view it. It's also possible to download it by clicking on "Save table".

Related
-----------

[Register a contract](/en-us/4biz-helium/additional-features/contract-management/use/register-contract.html)

[Register configuration item](/en-us/4biz-helium/processes/configuration/use/register-CI.html) 

[Create calendar](/en-us/4biz-helium/platform-administration/time/create-calendar.html)

[Service level agreement](/en-us/4biz-helium/processes/service-level/use/service-level-agreement.html)

[Register configuration item group](/en-us/4biz-helium/processes/configuration/configuration/register-configuration-item-group.html)

[Register cost per hour of unavailability](/en-us/4biz-helium/processes/configuration/use/cost-per-hour-unavailability.html) 

[Register availability group](/en-us/4biz-helium/processes/availability/configuration/register-availability-group.html)
  
!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020

