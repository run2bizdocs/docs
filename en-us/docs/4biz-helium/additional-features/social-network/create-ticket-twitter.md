title: Creating ticket via Twitter
Description: 4biz, in order to expand the service modalities, allows users to register their tickets directly through the social network interface Twitter.

# Creating ticket via Twitter
4biz, in order to expand the service modalities, allows users to register their tickets directly through the social network interface Twitter.

Before getting started
----------------------

- [x] It is necessary to have the integration functionality with Twitter configured in the 4biz instance besides of having the machine learning functionality (Python environment). Moreover, it is necessary to define the service that will attend to this type of service, as well as contracts and permissions in workflows. 

Procedure 
-------------

1.  Follow 4biz on Twitter;

2.  Click on "Messages" on Twitter;

3.  Create the ticket with the request you want;

4.  After the ticket is created, the system will answer with a standard feedback including the request number;

    !!! Abstract "NOTE"
        
        Once created the ticket via Twitter, the executor will have access to the request through the 
        functionality "Tickets" in the system, following the regular procedure of tickets execution. 
        
5.  When closing the ticket attendance, the Solution-Response will be sent to the user's Twitter as a direct message.

!!! Abstract "IMPORTANT"

    The opening and attendance of tickets via Twitter is only possible if the system follows a Builder workflow 
    specifically created in order to meet this type of request. Besides, to execute this flow, it's necessary 
    a business process scheduled by Cron expression. 
