Title: Builder FAQ
Description: 4biz - FAQ

# Builder Frequently Asked Questions (FAQ)

!!! Question "What is the difference between creating a form using the Form menu and the Business Object menu?"

	Creating a form using the Form menu is 100% manual process. Doing it through the Business Object menu, a form is generated from the database model. The form can then be edited in the Form menu.


!!! Question "How do I create many-to-many relationships in the Business Object?"

	To create a many-to-many relationship between two business objects, it is necessary to create a third business object that will be responsible for the relationship.
	E.g.: Let's create a many-to-many relationship between two business objects A and B, through a business object C.
	Both business objects A and B will have a one-to-many relationship with the business object C.
	In the business object C there will be two many-to-one relationships, one to business object A and the other to business object B.
	That way, through business object C, it is possible to relate one record in busines object A to many records in business object B and vice-versa.

!!! Question "Is it possible to create customized components to be used in Builder forms?"

	Yes, it is possible to create your own components to be used in Builder forms. For a complete tutorial, please check the technical documentation.

!!! Question "Where should I start building an application using the Builder?"

	Please refer to the section Steps to Implement Builder Solution.

!!! Question "How can I inject my own dependencies in a Builder form? Which steps must be performed?"

	You must register your own dependencies before they can be used. Only CSS and JavaScript dependencies can be injected in Builder forms.
	Register you dependency through menu Builder > resources > CSS or Builder > resources > JavaScript.
	With the new dependency added to the system, select the Shared code tab or the tab for the type of page you want to inject the dependency, click on the "Dependencies" tab on the left side, and fill in the requested fields.
	For more information about form dependencies, please check the technical documentation.

!!! Question "How do I define the actions that should be available in each workflow task?"

	Actions are registered in the main register flow tabs. To associate an action to a specific task, go to the workflow design, open the element properties, select the desired actions, and save your changes.

!!! Question "How do I delete an element from the workflow?"

	To delete a workflow element, select the element you want to delete, and press Ctrl + Del.


!!! Question "What do I do when I get the error message "Business process not informed"?"

	This error occurs when a reference to the business process is missing in the controller of the form that starts the business process. To fix it, access the form that starts the business process and insert the following code on the Process page controller:
	$scope. businessProcessName = 'name_of_the_business_process';

!!! Question "When I register a sub-process, is the information in the main process inherited by the sub-process?"

	No, it’s not inherited. When you include a new sub-process, regardless being BPE or ESI, in the main workflow you must fill in the "Attributes" tab the exact name of the sub-process that must be created on the workflow registration.
	All information, such as actions and main workflow status should be replicated in the sub-process registration.
	In a nutshell, it is recommended to follow these steps:
		1.	Register the main workflow;
		2.	Register the sub-process;
		3.	Include the sub-process element, making a reference to the sub-process already created.

