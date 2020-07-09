title: Configure mandatory fields
Description: The manager is responsible to choose which fields will be mandatory for users to complete.
# Configure mandatory fields

By configuring the mandatory fields, the manager will choose which fields will be mandatory for users to complete when contacting the attendants. Its purpose is to get the necessary information form the requesters to help them solve their request.

## Procedure

1.	Access the main menu System > Settings > Pages - Field configuration;
2.	Select which page layout you want to edit: Problem Management or Request/Incident Management.

    
### Configure fields of the "Problem" funtionality.

*When deciding to use mandatory fields, it's possible to demand certain information to be registered when creating a problem.*

1.	After access the home page of the functionality, choose the option "Problem" and click on "Edit";
2.	Select the fields you want to make mandatory. They are:



    |     **Field**            | **Mandatory** |
    |:------------------------:|:--------------:|
    |         Catalog          |      :ballot_box_with_check:                  |
    |     Service Category     |       :ballot_box_with_check:                 |
    |          Service         |       :ballot_box_with_check:                 |
    |           Phone          |          :ballot_box_with_check:              |
    |         Extension        |        :ballot_box_with_check:                |
    |     Physical Location    |      :ballot_box_with_check:                  |
    |        Observation       |           :ballot_box_with_check:             |
    |      Executor group      |        :ballot_box_with_check:                |
    |   Solve/Workaround till  |    :ballot_box_with_check:                    |

3.  Click on "Save".

### Configure fields of "Ticket Management" functionality

*When deciding to use mandatory fields, it's possible to demand certain information to be registered when creating a request/incident.*

1.	After accessing the home page of the functionality, choose the option "Incident/Request Management" and click on "Edit";
2.	Select the fields you want to make mandatory. They are:


    | **Field**         | **Mandatory** |
    |:-----------------:|:--------------:|
    |       Phone       |       :ballot_box_with_check:                 |
    |       E-mail      |          :ballot_box_with_check:              |
    |       Unit        |           :ballot_box_with_check:             |
    | Physical Location |       :ballot_box_with_check:                 |
    |  Contact's Origin |     :ballot_box_with_check:                   |


    !!! Abstract "NOTE"
    
        The parameters 65 (that identifies the default call origin ID of the service request) and 105 (identifies the source ID that will default when creating a new incident) automatically set up a contact source when the user registers a ticket. Therefore, if the field "Contact origin", in the ticket screen, is not mandatory, but, if there's an indication in the previously mentioned parameters, the field will be completed automatically.  
        
3.  Click on "Save".

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
