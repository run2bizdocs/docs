Title: Setting service attribute
Description: At 4biz, service attributes are configured from the Service Portfolio.

# Setting service attribute

Every service has a set of attributes that characterize it and differentiate it
from others. The individual characteristics are varied and can be related to the
provision of the service, its relationship with different management processes,
its relationship with other services and with the parties involved in its
delivery or operation.

At 4biz, service attributes are configured from the Service Portfolio.

## Before getting started

- [x]   It's necessary to have previously configured the Service Pipeline.

## Procedure

To access the configuration screen for the attributes of a service, follow the
procedure below.

1.  Access the main menu Processes \> Portfolio and Catalog Management \>
    Portfolio.

2.  Find the Service Portfolio that has the service to be detailed and click on
    the "Advance".

3.  Find the service in the Service Portfolio list and click on the "Advance";

4.  On the left side of the screen are presented the different themes where the
    attributes that can be configured are grouped.

5.  Click on the theme of the attribute to be defined to access its
    configuration page.

>   Next, there are the service attribute themes available in 4biz.

## Service Attributes

**Details**

Theme related to the basic attributes of the service, such as Name, Status,
Criticality, Category, and others.

The tabs, form fields and actions available on this topic are described in the
document [Registering/Editing a service](https://docs.run2biz.com/en-us/4biz-helium/processes/portfolio-and-catalog/use/register-a-service.html).

### Service Level Requirements

This theme groups the attributes related to the service level management
process, such as the utility and guarantee of the service. The utility of the
service is its purpose for which it was created, and which customer needs it
intends to meet. The service guarantee is the conditions that determine that the
service is suitable for usage.

Clearly, service level requirements are related to the service level management
process. However, they can also be associated with other processes, such as
incident, problem and change management.

*Tab of Service Level Requirements*

| Field              | Description                                         |
|--------------------|-----------------------------------------------------|
| Creation date (\*) | Date the service was created.                       |
| Service start date | Date the service was or will be released for usage. |
| Service owner      | Indication of service owner.                        |

(\*) Mandatory field

-   SERVICE USEFULNESS

| Field                     | Description                                                                                                                                           |
|---------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| Specification (\*\*)      | Describe the purpose of the service, that is, why the service exists and what it must do to meet the needs of its customers.                          |
| Context (\*\*)            | Describe the context of use of the service, that is, by whom, when, where and how the service will be used.                                           |
| Essential Features (\*\*) | List the essential features of the service. These are the items that the service depends on to work and whose failure would cause its unavailability. |

(\*\*) Fields that accept attaching files

-   SERVICE WARRANTY

| Field                        | Description                                                                                                                                                                                                                                                                                                                                  |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Safety (\*\*)                | Describe the information security requirements and what are the mechanisms that the service must perform to ensure the security of the data, such as: Secure storage and data disposal, access and permission profiles, information classification, and others.                                                                              |
| Availability (\*\*)          | Describe the availability requirements and what are the mechanisms that the service must perform to ensure its availability of access, such as: deployment and maintenance of equipment, high-availability technologies such as clusters and others.                                                                                         |
| Capacity (\*\*)              | Describe the capacity requirements and what are the mechanisms that the service must perform to ensure the delivery of adequate capacity, such as: Dynamic allocation of processing, monitoring of service usage, metrics for measuring capacity and demand, and others.                                                                     |
| Business Continuity (\*\*)   | Describe the service continuity requirements and what mechanisms the service should have in place to ensure that the service can operate within minimum acceptable levels, even in a crisis situation, such as: redundant data center availability, disaster response plans, service recovery tests, and others.                             |
| Performance (\*\*)           | Describe the performance requirements and what are the mechanisms that the service must have to ensure that its performance will meet customer expectations, such as: expected and acceptable times to complete each stage of the service, and others.                                                                                       |
| Planned interruptions (\*\*) | Describe the requirements for planned service interruptions and how service management needs to ensure that agreed rules are followed, such as: Maximum time for a planned service interruption, the frequency at which the service can be interrupted, mechanisms for requesting, approving and managing planned interruptions, and others. |

(\*\*) Fields that accept attaching files

-   SERVICE SUPPORT

| Field               | Description                                                                                                                                                                                                                                                     |
|---------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Incident Management | Describe the requirements for the incident management process. Items such as: Classification of incidents, their severity and priority, acceptable times to identify an incident, its registration, investigation, and restoration of normal service operation. |
| Problem Management  | Describe the requirements for the problem management process. Items such as: Expected times for identifying, recording, and investigating a problem.                                                                                                            |
| Change Management   | Describe the requirements for the change management process. Items such as: Types of changes, procedures for recording, analyzing, approving, and reviewing changes. Also, preferred windows for maintenance and periods to stop change.                        |

-   CONFORMITY

| Field           | Description                                                                                                                                                                                                                                                                                                      |
|-----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Internal (\*\*) | Describe the internal governance and risk requirements that must be observed and met during the service lifecycle and its operation. They are usually related to management policies determined by the organization's board of directors to preserve investments and the organization from a bad administration. |
| External (\*\*) | Describe the external governance and risk requirements that must be observed and met during the service lifecycle and its operation. It usually involves complying with regulations, ordinances, laws and regulatory frameworks to which the organization is subject.                                            |

(\*\*) Fields that accept attaching files

*Tab of Attached Documents*

| Component                    | Description                                            |
|------------------------------|--------------------------------------------------------|
| Select subject of attachment | Select the subject to which the attachment is related. |
| Table of files               | List of attached files.                                |

The following functions are available:

| Functions | Description                                                      |
|-----------|------------------------------------------------------------------|
| Add File  | Enter the indicated file as an attachment to the indicated topic |
| Save      | Save the attribute                                               |
| Clear     | Clean the fields                                                 |
| Delete    | Delete the file                                                  |

### Financial Attributes

These are the attributes that describe the relationship between the financial
management process and the service.

The financial attributes indicate the service's relationship with the Result
Centers, Departments and with the financial values of CAPEX, OPEX, Direct Value
and others.

This information can be used to present the current financial situation of a
service, as well as the entire history of cost and price variation.

The registration or changes in the financial information are performed within
the Financial Management process.

**Tip**

4biz differentiates between service cost and service price.

**Note**

4biz, using the hierarchical cost model, lists the registered financial items
and calculates the values corresponding to each service. This allows identifying
the cost distribution among the different registered services.

In addition, the values will be automatically linked to the corresponding
configuration item with the following information:

| Field          | Description                                                      |
|----------------|------------------------------------------------------------------|
| Category       | The financial registration category.                             |
| Type           | Indication of the type of registration, that is, cost or revenue |
| Classification | The cost classification                                          |
| Value          | The value of service                                             |
| Cycle          | The financial cycle                                              |

### Business Cases

This section contains the strategic information related to the business cases
prepared for the project and development of the service.

*Business Cases Guide*

| Campo                      | Descrição                                                                       |
|----------------------------|---------------------------------------------------------------------------------|
| Business Case (\*)         | Name of business case                                                           |
| Executive summary (\*\*)   | Present the executive summary of the business case                              |
| Stakeholder/Entity         | Indicate stakeholders for the business case                                     |
| Scenarios (\*\*)           | Describe the business scenarios considered in the development of business cases |
| Problem/Opportunity (\*\*) | Describe the problem to be solved or the opportunity to be taken advantage of   |
| Proposed solution (\*\*)   | Specify the proposed solutions                                                  |
| Financial analysis (\*\*)  | Report on the performed financial analysis                                      |
| Risk analysis (\*\*)       | Describe the risks considered in the analysis of the case                       |
| Technical viability (\*\*) | Indicate technical considerations about the case                                |
| Conclusion (\*\*)          | Specify the conclusion reached by the case analysis                             |

(\*) Mandatory fields

(\*\*) Fields that accept attaching files

*Attached Documents Guide*

| Component                    | Description                                           |
|------------------------------|-------------------------------------------------------|
| Select subject of attachment | Select the subject to which the attachment is related |
| Table of files               | Lista of attached files                               |

The following functions are available:

| Functions | Description                                                      |
|-----------|------------------------------------------------------------------|
| Add file  | Enter the indicated file as an attachment to the indicated topic |
| Save      | Save the attribute                                               |
| Clear     | Clean the fields                                                 |

### Configuration Items

This section of attributes presents the relationship map of the configuration
items that make part of the service.

Changes in the relationship between configuration items are made within the
Configuration Management process & ITAM.

### Business Processes

Services are always linked to business processes, whether to operationalize,
support or enable their execution. It's important to understand this
relationship to properly evaluate the risks and impacts of unavailability, as
well as investment and business opportunities.

In this section of attributes, register and link the organization's business
processes with the services provided.

The following functions are available:

| Function                   | Description                                           |
|----------------------------|-------------------------------------------------------|
| Linking business process   | Associates a business process record with the service |
| New business process       | Records a new business process                        |
| Search here                | Search between the linked processes                   |
| List of business processes | It allows to view details and unlink                  |

### Support Services

Services can be primary, intensifying, or supportive.

Primary services are those that are created and supported to deliver the
expected results. They are perceived directly by their customers through
interaction and obtaining value.

Intensifying services are not essential for delivering value to the customer.
However, they encourage customers to use the contracted services more and
differentiate the service provider from its competitors.

Support services that provide support for the primary service. They are not used
directly by customers and users, however they are critical to delivering value.
Most common examples are data backup and equipment monitoring.

The following functions are available:

| Function     | Description                         |
|--------------|-------------------------------------|
| Link service | Link a support service.             |
| Search here  | Search between the linked services. |
|              |                                     |
|              |                                     |

### Business Owner

The business owner is the person or group that is responsible for defining the
business vision and roadmap that should be supported by the service.

This information is important to speed up the negotiation of changes, escalation
of incidents, reporting of service levels and other management actions involving
business areas.

The following functions are available:

| Function    | Description                                  |
|-------------|----------------------------------------------|
| Link users  | Link someone as business owner               |
| Link groups | Link a group as business owner               |
| Search here | Search between linked individuals and groups |
| Unlink      | Unlink the listed business owner             |

### Business User

Business users are the people who use the service during their work.

This information is relevant to actions, such as: communicating about the
service's operation, identifying opportunities for improvement, understanding
the demand and other management actions that involve the use of the service.

The following functions are available:

| Function    | Description                                |
|-------------|--------------------------------------------|
| Link users  | Link an individual as user                 |
| Link groups | Link a group as user                       |
| Search here | Search between the linked users and groups |
| Unlink      | Unlink the listed user or group            |

### Requests

In this attributes section, all requests activities that make up the service are
linked. These activities are the main point of contact of users with the service
since their orders are formalized through their records.

Availability for registering a request depends on its link to the service and
the permission set.

The following functions are available:

| Function             | Description                                                    |
|----------------------|----------------------------------------------------------------|
| New service request  | Register an activity of request                                |
| Link service request | Allows to search and link a registered activity to the service |
| Search here          | Search between the linked requests                             |
| Unlink               | Unlink the listed activity                                     |

### Applications

Services are supported or operated using applications or information systems. In
this section, all applications related to the service are associated and
presented.

The following functions are available:

| Function         | Description                                             |
|------------------|---------------------------------------------------------|
| Link application | Allows to search and link an application to the service |
| New application  | Create a record for an application                      |
| Search here      | Search between the linked applications                  |
| Unlink           | Unlink the listed application                           |

### Service design package

This section contains all technical documentation of the service, such as
software requirements, contract templates, service level agreements, operational
level agreements, service transition plans, data schema, data network topology,
and others.

It's required to note the technical details of the service and files can be
attached. Since the content of the service design package can vary widely
between different organizations, each attached file can receive its own
description.

| Field        | Description                                  |
|--------------|----------------------------------------------|
| Details (\*) | Notes of the service design package details. |

(\*) Mandatory field

*Attached Documents*

The following functions are available for attaching documents:

| Functionality          | Description                     |
|------------------------|---------------------------------|
| Attachment description | Subject of the attached file.   |
| Add file               | Select the file to be attached. |
| List of attached files | Open and delete attached files. |

### Incidents

In this section of attributes, all incident activities that make part of the
service are linked. The registration of these activities allows the quick
targeting of the incident attendance, as well as its evaluation, diagnosis, and
resolution.

The following functions are available:

| Function               | Description                                                    |
|------------------------|----------------------------------------------------------------|
| New incident activity  | Register an activity of incident.                              |
| Link incident activity | Allows to search and link a registered activity to the service |
| Search here            | Search between the linked incidents                            |
| Unlink                 | Unlink the listed activity                                     |
|                        |                                                                |

### Continuity procedures

Continuity procedures are used to respond to an exceptional situation that
severely impacts the service, such as a crisis or disaster. In these cases, an
action plan to continue the service delivery must be triggered and followed for
a quick response. This plan consists of a set of procedures.

In this section of attributes, all the necessary procedures for the restoration
of normal service operation are listed.

The following functions are available:

| Function       | Description                                          |
|----------------|------------------------------------------------------|
| New procedure  | Register a new procedure                             |
| Link procedure | Allows to search and link a procedure to the service |
| Search here    | Search between the linked procedures                 |
| Unlink         | Unlink the listed procedure                          |

### Contracts

The relationship between services and contracts is one of 4biz's most important
configurations. The flexibility to organize this relationship allows you to
manage multiple contracts and offer different levels of quality for the same
service, such as Gold, Silver and Bronze.

The following functions are available:

| Function      | Description                                         |
|---------------|-----------------------------------------------------|
| New contract  | Register a new contract                             |
| Link contract | Allows to search and link a contract to the service |
| Search here   | Search between the linked contracts                 |
| Unlink        | Unlink the listed contract                          |

### Service owner

Service owner presents the service to the organization. Has great knowledge
about the service and participates in strategic decisions. The owner also acts
as a point of contact within the escalation process for incidents and requests.

In this section of attributes, there are listed the users and groups that are
indicated as owners of the service.

The following functions are available:

| Function    | Description                                |
|-------------|--------------------------------------------|
| Link users  | Link someone as service owner              |
| Link groups | Link a group as service owner              |
| Search here | Search between the linked users and groups |
| Unlink      | Unlink the listed user or group            |

### Knowledge base

Knowledge is a fundamental tool for the design, development, delivery and use of
a service. The more people are knowledgeable about the service, the greater the
chances of getting value from its usage.

This section lists all knowledge records related to the service.

The following functions are available:

| Function       | Description                                                 |
|----------------|-------------------------------------------------------------|
| Link knowledge | Allows to search and link a knowledge record to the service |
| Search here    | Search between the linked knowledge records                 |
| Unlink         | Unlink the listed knowledge record                          |

### Skill/Resource

To put knowledge into practice, the people involved in the service need skills
and resources to perform the actions. Indicate the requirements for using the
service facilitates the process of hiring people, organizing teams and training
and qualification.

This section lists the skills and resources needed to use and maintain the
service.

The following functions are available:

| Function        | Description                                           |
|-----------------|-------------------------------------------------------|
| Link capability | Allows to search and link a capability to the service |
| New capability  | Register a new capability                             |
| Search here     | Search between the linked capabilities                |
| Unlink          | Unlink the listed capability record                   |

### Planned Capacity

When designing a service, the manager must plan how to meet current and future
capacity needs. This long-term vision for the service will allow to make the
appropriate investments and in time to ensure the availability of capacity.

This section of attributes lists the service's capacity or performance
indicators.

The following functions are available:

| Function                             | Description                                                                  |
|--------------------------------------|------------------------------------------------------------------------------|
| Link capacity/performance indicators | Allows to search and link a capacity or performance indicator to the service |
| Unlink                               | Unlink the listed capacity or performance indicator                          |

### Attribute of Demand

The lack of capacity of a service causes unavailability and the excess is a
waste of investments. For this reason, the demand for a service needs to be
understood to adequately plan the capacity to attend it.

In this section, the demand attributes are related to the service.

The following functions are available:

| Function               | Description                                          |
|------------------------|------------------------------------------------------|
| Link demand attributes | Allows to search and link a service demand attribute |
| Unlink                 | Unlink the listed demand attribute                   |

### Service Evaluations

This section lists all service delivery evaluations. To facilitate the viewing,
it's possible to filter the records using dates to limit the period of listing.

The following functions are available:

| Filter                  | Description                              |
|-------------------------|------------------------------------------|
| Register period – Start | The start date to filter the evaluations |
| Register period – End   | The final date to filter the evaluations |

The following functions are available:

| Function | Description                                         |
|----------|-----------------------------------------------------|
| Search   | List the evaluations considering the defined filter |
| Clear    | Clean the dates defined in the filter               |

### Service Audit

This section presents the occurrences of actions related to the service. These
can be changing attributes or details, registering incidents and requests,
configuring relationship with contracts, and others.

The following functions are available:

| Field          | Description                                 |
|----------------|---------------------------------------------|
| Opening period | Sets the start and end date for the listing |
| Category       | Filters the listing by the chosen category  |
| Search         | Searches with defined filters               |
| Clear          | Clean the filters                           |
| Expand         | Presents more details                       |

*Tab of register occurrences*

| Object           | Description                           |
|------------------|---------------------------------------|
| Category (\*)    | Defines the category to be registered |
| Description (\*) | Specifies the registration details    |
| Save             | Saves the completed data              |
| Clear            | Clean the completed fields            |

(\*) Mandatory field
