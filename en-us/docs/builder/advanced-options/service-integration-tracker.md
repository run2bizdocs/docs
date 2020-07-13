Title: Service Integration Flow  
Description:Service integration flows, as the name implies, involve workflows that are executed based on system services, such as integrations and conversions, for example.  

# Service Integration Flow   

Service integration flows allow you to integrate Builder applications with external systems, whether from the 4Biz environment or from third parties. It is a great option for integration with legacy systems.

## How to access  

1.	To access the Service Integration Flow configuration page, go to menu Builder > Management > Integration Flow or to menu Tracker > Integration Flow.

## Prerequisites  

1. Not applicable  

## Register a new integration flow

To register a new integration flow, click on the "New” button.

## Flow data

Through this tab, all basic information about the flow to be design is defined.

1.	On the **Flow data** tab, fill in integration flow **Name** and **Description**, and inform the Builder Application to which it will be associated. Select the **Show as a component** checkbox whether the integration flow should be made available as a component in 4Biz Tracker workflows.

## Variables

In this tab, you can configure the variables that will be used in the integration flow. Variables are objects capable of retaining and representing a value or expression during integration flow execution.

1.	To add a new variable, click on the "Add" button. The following screen will be displayed:

2.	Fill in the fields:
    •	Variable name
    •	Description
    •	Store in the database: whether the variable should be stored internally, in the Builder data model.
    •	Return variable: whether the variable should be included in the output JSON object returned at the end of the flow's execution.
    •	Values list: Whether the variable contains a values list
    •	Mandatory entry variable in execution: this option must be selected if the execution of the flow depends on the existence of the variable before the execution starts.
    •	Variable type
    •	Variable Initial value, which can be a constant value or a value returned by script execution.

3.	Click on the “Include” button to finish creating the variable.

!!! Abstract "ATTENTION"

    To permanently save the changes, it is necessary to click on the “Save” button on the top bar.


## Actions

Actions are code written in Rhino that implement rules and business logic in the integration flow.

1.	add a new variable, click on the "Add" button. The following screen will be displayed:

2.	Fill in the fields:
    •	Identifier: it is how the action will be associated to the flow diagram.
    •	Name: this is the name by which the action will be referenced in the flow diagram.
    •	Rhino Script to be executed when the action is triggered.

3.	Click on the “Include” button to finish creating the action.

!!! Abstract "ATTENTION"

    To permanently save the changes, it is necessary to click on the “Save” button on the top bar.

## Diagram
The diagram is the modeling of the integration process being implemented by the integration flow.

1.	To edit the diagram, click on the corresponding tab. The following screen will be displayed:

2.	Elements that can be added to the flow are found in the palette in the left corner of the screen. To add an element in the flow, select it and drag it to the drawing page. A pop-up window with the element's properties will be displayed on the screen. Fill in the information according to the chosen element.

3.	At finishing editing the diagram, click on the “Save” button on the top bar.





















!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020 
