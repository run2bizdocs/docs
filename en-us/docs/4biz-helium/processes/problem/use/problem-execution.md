title: Execute problem
Description: It allows to execute problem.

# Executing problem

This functionality allows to execute the necessary tasks to solve a problem. In this step, the classification of the problem and the designation of the appropriate area to handle the problem according to the IT Service Catalog are done. It is necessary to link the problem to existing incidents and register the problem to facilitate prioritization of problem solving, evaluate the impact on business, and determine the urgency of the solution. This evaluation determines the classification of the problem.


## Before getting started

It is necessary to have problems registered to execute them.

**Procedure**

1.	Access the main menu Processes > Problem Management > Problem;

2.	Find the problem you want to execute, click on "Open" and confirm the assignment of the task to your user;

3.	In the "Diagnosis" area, for a better understanding and investigation of the problem, you can perform the following activities:

   
- Create a Kanban or link an existing one. To create a new Kanban, you need to click on "+ Workspace" and complete the available fields, such as title, select the users responsible for the execution of the problem, and others. To link a Kanban already created, just click on the other icon, related to the Workspace.

    
    !!! Abstract "ATTENTION"
    
        When linking an existing Kanban, if the user does not have permission to access a particular Workspace, the system will display a message informing you. The user must then request permission in Workspace and Sprint or create a new Kanban framework.

- Register any known error to enable the evaluation by the responsible team, and the diffusion of the solution for the ones interested. In the "Known Error" tab, click on "Add Workaround” and describe any relevant information;


    !!! Abstract "NOTE"
    
        If the known error option is selected, the system will present a field to define to which environment this knowledge should be linked (Production or Development).
    
    !!! Abstract "NOTE"
    
        It is possible to register more of than one solution to the "Workaround".
        
    !!! Abstract "NOTE"
        
        The workaround registered can be viewed in the "Ticket" screen when linking the problem to the ticket.

    - In the "Attachments" tab, it's possible to upload any related files;
    - The "Notes" tab allows to register any complementary information.


4\.	In the "Solution" area, fields will be available to describe the process and a solution of the problem. They are:

- Create a Kanban, with the information mentioned above;

- It's possible to create a new change related to the problem’s solution by clicking on "Register Change" (available in the tab "Change”) and completing the necessary fields, or to link an already existing change by clicking on the search field and selecting the change you want;

- It's also possible to attach files and register notes in this phase of the problem execution. 

5\.	In the "Review and closure" area, the executing team will specify the details of the problem solution and the lessons learned with it. The following actions are available:

- In the "Review" tab, select the option about the successful closure of the problem;

- In "Serious Problem Review”, users can complete the fields with the actions taken to correct the problem and the improvements to be deployed to avoid its subsequent occurrence, among others;

- In the “Tasker” tab, it is possible to create a Kanban;

- In "Lessons learned", when clicking in "Add", it'll be possible to select and link a knowledge to describe any useful instructions and facilitate the solution of future problems.

- It is also possible to attach files and register notes in this phase of the problem execution.

- In the "Closure" tab, it is possible to choose the status where the problem is (Registered, Solved or Canceled). If you choose any of the last two options, you will need to choose the cause and category of the solution, as well as to describe the information needed to close the problem.


6\.	Click on "Operations" and then on "Save and keep current task" to register the execution and not advance the activity flow or select "Save and advance flow” to close the task and direct it to the next phase of the flow.

    
Related
------------
 
[Register problem](/en-us/4biz-helium/processes/problem/use/register-problem.html)

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
