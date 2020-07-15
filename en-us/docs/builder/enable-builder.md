Title: Enable Builder

# Enable Builder

The requisites for enabling Builder in 4Biz are:

- 4biz version is Helium or higher;

- 4biz configured for HTTPS access;

- Configure the following parameters.


--


- **Parameter 309:**

    ```sh
    Value: Yes
    ```

- **Parameter 310:**

    ```sh
    https://localhost:8443/cit-esi-web
    ```

Note that if Builder does not reside on the same machine as 4Biz, localhost must be changed to the server name on which Builder is installed.

- **Parameter 311:**

    ```sh
    domain\username
    ```

For the integration to work correctly it is necessary that the configuration of Builder username contains the identification of the domain which it belongs. For example: **4biz.local\builder**.
