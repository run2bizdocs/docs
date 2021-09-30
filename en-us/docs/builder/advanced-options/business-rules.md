    title: Business rules  
Description: Business rules define how your business works, and can cover a variety of issues such as your policies, interests, objectives, ethical and social commitments, contractual obligations, strategic decisions, laws and regulations, among others  

# Business rules

As regras de negócio criadas são bloqueadas por padrão. Isso significa que a regra não poderá ser utilizada a menos que seja desbloqueada. Para desbloquear selecione a regra desejada e clique na opção Desbloquear.     

## How to access 

1. To access the  Business Rule configuration page go to menu Builder > Management > Business Rule.    

## Prerequisites

1.	No applicable.  

## Register a new business rule

1.	To register a new database, click on the "New” button;

2.	Business Rules are built by designing flow or coding a Rhino script.

## Create Flow type business rule

1.	On the Basic data tab, fill in the business rule Name and Description, inform the Builder Application to which it will be associated, and choose Flow Type.

2.	On the Variables tab click on the "Add" button. The following screen will be displayed:

3.	Fill in the fields in the Variable section:
    •	Variable name
    •	Description
    •	Store in the database: whether the variable should be stored internally, in the Builder data model.
    •	Return variable: whether the variable should be included in the output JSON object returned at the end of the business rule flow's execution.
    •	Values list: Whether the variable contains a values list
    •	Mandatory entry variable in execution: this option must be selected if the execution of the flow depends on the existence of the variable before the execution starts.
    •	Variable type
    •	Variable Initial value, which can be a constant value, or a value returned by script execution.

4.	Click on the “Include” button to finish creating the variable;

5.	On the Actions tab click on the "Add" button. The following screen will be displayed:

6.	Fill in the fields in the Action section;

    1.	Identifier: it is how the action will be associated to the flow diagram.
    2.	Name: this is the name by which the action will be referenced in the flow diagram.
    3.	Rhino Script to be executed when the action is triggered.

7.	Click on the “Include” button to finish creating the action;

8.	To edit the diagram, click on the corresponding tab. The following screen will be presented:

## Create Script type business rule

1.	On the Basic data tab, fill in the business rule Name and Description, inform the Builder Application to which it will be associated, and choose Flow Script:

2.	Code the Rhino script that implements the business rule and, if necessary, add variables as explained in the section Variables of type Flow;

3.	When finishing editing the script, click on the “Save” button on the top bar.

!!! info "ATTENTION"
    
    New business rules are blocked by default. This means that the rule cannot be used unless it is unblocked. To unblock select the desired rule and click on the Unblock option


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021







