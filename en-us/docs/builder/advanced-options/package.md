Title: Package
Description: A package is a collection of Builder artifacts (applications, business objects, forms, flows) that can be copied between environments through export and import procedures.
# Package  

A package is a collection of Builder artifacts (applications, business objects, forms, flows) that can be copied between environments through export and import procedures.

## How to access

1.	To access Package configuration page go to menu Builder > Management > Package.

## Prerequisites

1. No applicable.  

## Managing packages 

1.	To register a new package, click on the "New" button;

![Screenshot](images/Package-Search.png)

Figure 1 - Package search screen  

2.	Fill in the package Name and Description. Then add elements that will be part of the package.;

3.	Click on the "Save" button to create the package and click on the "Search" to go back to the main screen;

4.	To export a package, select it and then click on the "Export" button. Packages are exported in JSON format;

5.	To import a package, click on the “Import” button, inform whether version of the package to be imported should override elements with same identifier, and whether the create/modify Business Objects DDL should be executes. Select a JSON import for a previously exported package and click on the “Import” button.

!!! info "Atenção"
    
    To ensure compatibility, it is recommended that the Builder version that is importing a package is the same version that has exported it.




!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020 
