title: Database Connection
Description: Database Connection

# Database Connection

Builder requires setting up a database connection to interface with database tables.

## Before getting started

You must have a working database driver in your operating environment before setting up a Builder Database Connection.

**Steps**


1.	Access the Database Connection configuration page through navigation in the menu Builder > Configuration > Database Connection;

2.	Click on the "New" button;

3.	Fill in the information for the fields Name, Description and Type;

4.	Type can be either JNDI Connection or Direct Connection:

- For JNDI connection, enter the JNDI name as configured in the operating environment;
- For direct connection, enter Database type, JDBC Path  and database credentials (User and Password).

5\.	Click on the "Save" button.


## MS SQL SERVER CONNECTION
Since Builder uses the jtds driver to connect to MS SQL Server databases, the connection URL must follow the pattern jdbc:jtds:sqlserver://{server}:{port};DatabaseName = {name of the database}. In addition, the driver name for the Integration Flow connector must be net.sourceforge.jtds.jdbc.Driver.


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020  

