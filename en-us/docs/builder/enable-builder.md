Title: Enable Builder

# Enable Builder

For 4biz/Builder integration to work:

- The 4biz version is 8.0.0.0 or higher
- 4biz configured for HTTPS access: //
- The integration parameters are configured in the 4biz 

![Builder Conection][1]

- **Parameter 309:**

    ```sh
    Value: Yes
    ```

- **Parameter 310:**

    ```sh
    https://localhost:8443/cit-esi-web
    ```

- **Parameter 311:**

    ```sh
    4biz.local\builder.user
    ```

[1]:images/builder-conection.png
