Title: Builder Elements

# Builder Elements

A Builder application is built with a combination of the following elements.

![Builder Elements](images/builder-elements.png)

## Business Object

Business Objects are Builder abstractions to application data entities. Each Business Object represents the data model and is linked to a table or a view in a relational database.

![Builder Elements](images/builder-9.jpg)

![Builder Elements](images/builder-10.jpg)

![Builder Elements](images/builder-11.jpg)

![Builder Elements](images/builder-12.jpg)

![Builder Elements](images/builder-13.jpg)

![Builder Elements](images/builder-14.jpg)

## Form

A Builder Form is the way how users interact with the application, executing operations for creating, reading, updating, or deleting data in a Business Objects, or providing information for flow executions.

![Builder Elements](images/builder-16.jpg)

![Builder Elements](images/builder-17.jpg)

![Builder Elements](images/builder-18.jpg)

![Builder Elements](images/builder-19.jpg)

![Builder Elements](images/builder-20.jpg)

![Builder Elements](images/builder-21.jpg)

![Builder Elements](images/builder-22.jpg)

![Builder Elements](images/builder-23.jpg)

![Builder Elements](images/builder-24.jpg)

## Integration Flow

Integration flows allow you to integrate Builder applications with external systems, whether from the 4Biz environment or from third parties. It is a great option for integration with legacy systems.

## Business Process

A Business Process allows the execution of Integration Flows in a periodical and automated way.
Interaction between Builder elements.


In a simple term, we can define the interaction between elements as:

1.	Business Object interacts directly with Forms and external systems (via REST API), making use of Domains and Business Rules for data validation;

2.	Forms interact natively with Business Objects and external systems, using JavaScript / AngularJS programming. User interfaces and business rules applied to Forms can be enriched using shared resources such as JavaScript, CSS and HTML code;

3.	Forms also connect to Integration Flows to interface with legacy systems and databases, and to and ITSM Flows in interface with 4Biz Ticket Management.

