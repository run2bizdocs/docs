title: Registering user
Description: This feature provides a variety of actions, such as including, changing, and deleting an user. 
# Registering user

Some employees may need to access the system, in which case it is necessary to create a user account. This account will allow the employee access through a login, a password and an access profile that consolidates their rights and permissions in the system.

Note that the employee needs to be registered previously, which makes this procedure simplified.

The maintenance of the user's account involves the inclusion, alteration and exclusion. In particular, the system administrator can change an employee's login and password.


## Before you start

To register an user, it is necessary to:

- [X] Register the employee in advance;

- [X] Have at least one Access Profile registered in the system.

When creating or changing a user's data, the system checks whether sending an email with access data is set. The following parameters must be configured to activate this functionality:

- [X] Configure the parameter 33 and correctly indicating the URL to access the 4biz platform;

- [X] Configure the parameter 455 with the email template ID created to send the access data. The chosen model must contain the keys $ {LOGIN} and $ {NEWPASSWORD}.

!!! note "EXAMPLE"

    Email template: "Dear user, here's the access data. User: $ {LOGIN} and Password: $ {NEWPASSWORD}"

!!! warning "ATTENTION"

    It is not possible to send login and password information when registering a new user imported from Microsoft Active Directory® or LDAP.


## Procedure

1. Access the functionality through the Navigation Menu> General Registration> Personnel Management> User;

2. Indicate the employee through the search box presented by clicking on the “Employee” text box;

3. Fill in login and password, repeating the password in the password confirmation box;

4. Select an Access Profile for the user;

5. If necessary, add corresponding User Groups;

6. Click on "Save".


!!! info "INFORMATION"

    To complete an operation to create, change or delete a user record, the system checks whether a password policy is in place and whether the user has been imported from an LDAP directory.

    In this way, the completion of the operation can be prevented. Because it is not possible to change the password for a user imported from an LDAP directory. Likewise, the password must follow the defined complexity policy.


Active Directory is a registered trademark of Microsoft Corporation.



Related
-----------

[Register employee](/en-us/4biz-helium/initial-settings/access-settings/user/register-employee.html)

[Create profile access](/en-us/4biz-helium/initial-settings/access-settings/profile/create-profile-access.html)

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021

