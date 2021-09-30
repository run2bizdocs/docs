Title: Report setup  
Description:Report setup is where you can configure execution settings, if needed, for the reports added to the system through the Report File option. 

# Report setup  

**Report** **setup** is where you can configure execution settings, if needed, for the reports added to the system through the **Report File** option.

## How to access 

To access the Report setup configuration page, go to menu Builder > Management > Report.

## Prerequisites 

The report to be set up must have been registered through the menu Builder > Resources > Report upload.

## Filling in the registration fields

Choose an item from the list of reports and click the "Edit" button.

## Report

1.	The values for Application, Name, Description and Folder are filled in based on the report registration data and can be changed on the Report screen.

## Data source

1.	Configure the Data source from where the report will get its data. Enter the type of the data source, which can be:
    •	None: if the report does not get data from a database;
    •	Data connection if the information source is in a database. In this case, also enter the respective Database Connection (created in the menu Builder > Configuration > Database Connection);
    •	Data object: if the information source is a database object configured in the Builder application;
    •	ESI flow: if the source of information is an integration flow configured in the Builder application. In this case, also enter the name of the Flow (created in the menu Builder > Management> Integration Flow);
    •	Script: if the data source is a script, enter the Rhino script code to be used.

## Parameters

1.	User this tab to register parameters necessary for the report execution 
    •	Click on the "Add" button to add a new parameter;
    •	Enter the parameter Name, Type  and  any type related data;
    •	Click the "Save" button to add the parameter to the list;
    •	To edit a parameter in the list, click on the "Edit" button;
    •	To remove a parameter from the list, click on the "Remove" button.

## Form

In this tab if the form configuration for the report.
1.	Fill in the Form Title and check whether tabs should be displayed;
2.	Optionally adjust HTML e JavaScript codes used in the form.



!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021 


