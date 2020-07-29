title: Configuring a mailbox
Description:Configure the sending and receiving of e-mail from different servers in order to meet different contracts, so that the same 4biz can serve different clients and each one will have its own mailbox.

# Configuring a mailbox

As an omnichannel platform, 4biz connects with multiple communication channels. The variety is presented both in types and formats of the channels, as well as in their quantity. In this way, 4biz enables the simultaneous and connected use of several communication channels, facilitating contact between service provider and consumer.

Among the communication options, email is one of the most active and popular ways. 4biz is capable of sending and receiving email from several different accounts, even if they are on separate email servers. Therefore, the information flow can be built to meet business needs.

For example: Configuring a different email account for each contract managed by 4biz, where each mailbox is hosted on the corresponding client's email server.

In this configuration, we have the following advantages:
- Communication with clients is facilitated by using an email address familiar to their organization.
- The impact of unavailability on communication is reduced once the loss of access to a server affects only the related contract.
- Messages are properly stored and grouped by contract.


## Procedure to register the mailbox

1.	Access the functionality through the navigation menu > Parametrization > Mailbox;
2.	Click on "New";
3.	Complete the field "Description" to identify the email connection;
4.	Choose the type of mailbox. Each one has a different purpose, which is:
    
    4.1\. The "Input" type means that emails that arrive in the specified mailbox will be read and processed. Use this option to indicate where the users' messages will arrive. 
    
    In this case, new registration fields will be opened, such as:

        - Server (host address or server IP);
        - Server port (Connection port);
        - User (Email address);
        - Password;
        - Provider (Connection protocol, which can be imaps, pops, imap or pop);
        - Inbox folder where emails will be stored (usually inbox).

    4.2\. The "Output" type indicates the connection that will be used by 4biz to send emails originating from system actions. For example: confirmation for the opening of a request, approval request or completion of a service. 
    
    In this case, new registration fields will be opened, such as: 
       
        - Server (host address or server IP);
        - Server port (Connection port - usually the value is 25);
        - Sender (Identification that will be presented to the recipient);
        - Indicate whether secure TLS/SSL authentication is required;
        - Indicate whether connection user authentication is required. If so, you will be required to complete the corresponding user and password fields.

5\.	Click on "Save" to perform the operation.

## Procedure to link a mailbox to a contract

If you want to link one of the previously registered mailboxes to a contract, follow the procedure:

1.	Access the navigation menu > Processes > Portfolio and Catalog Management > Contract Registration;
2.	Then link in the "E-mail Outbox" field the mailbox you want to. The mailbox must be previously registered;
3.	Click on  "Save" to perform the operation.

## Procedure to link a mailbox to a workflow

If you want to link a mailbox to a workflow, follow the procedure below:

1.	Access the navigation menu > Tracker > Flow Design;
2.	When creating or editing a flow, find the "Diagram" tab. Add or edit a "Send message - email" connector;
3.	In the "Message" tab, in the "Email Outbox Configuration" field there are 2 options:

    3.1. Choose the option "Contract" so that the component uses the mailbox indicated in the contract related to the flow.
   
    3.2. Choose the option "Specific" to indicate the mailbox you want to.

4\.	Complete the parametrization of the email sending indicating in the "Recipients" tab, the users or groups that will be the recipients of the messages;
5\.	Click on "Save" to perform the operation.


!!! note "Text"
    
    By default, every flow primarily uses the output system mailbox. Therefore, it's only necessary to indicate a specific mailbox, if it's necessary to satisfy a particular requirement of a workflow.



!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>03/11/2020
