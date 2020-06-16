title: Register EPL template
Description: Allows to create and maintain the EPL templates, to be used in the EPL creation.
# Register EPL template

This functionality allows to create and maintain the EPL templates, to be used
in the EPL creation.

It's necessary to have knowledge in the event processing language. For further
information go to: <http://www.espertech.com/esper/esper-documentation/>.

This feature provides a variety of actions, such as including, changing, and
deleting the EPL templates.

The correlation of events can be done through the configuration of parameters and scripts that support the integration of Event Management tools for component failure event correlation and potential Problem identification within the context of the EPL. It serves to identify two or more simultaneos events and create another event that contains both scenarios. This can be easily configurated through the following fields:

. Name: name of correlation  
. Source: the source of event  
. Type of connection: external correlation or file  
. Category: category of event created

Actions:
. For Information, which action, urgency, impact and business rules.

![Basic-data][1]
 
. For Warning, which action, urgency, impact and business rules.

![Warnning][2]

. For Exception, which action, urgency, impact and business rules.

![exception][3]

Procedure
-------------

1.  Access the functionality through the main menu Processes \> Event Management
    \> Business Monitor \> Model of EPL;

2.  Complete the fields available;

3.  Click on "Save".

[1]:images/basic-data.png
[2]:images/warnnig.png
[3]:images/exception.png
!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
