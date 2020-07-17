Title: Implementing Remote Access

# Implementing Remote Access

The remote access functionality allows the computers to be accessed remotely from your 4biz instance. In this sense, we use the Virtual Network Computing (VNC) protocol resources through the Apache Guacamole - web-based remote access gateway - to make this operation feasible. In addition to being able to remotely access a configuration item, all sessions are saved and made available to the CI information. This ensures better control over the actions taken by providing a reliable and auditable environment.

This functionality is an add-on to the Configuration Management and depends on the inventory process to make viable remote access to a CI.


## Before getting started

* [x] Having the inventory process defined and functional using the 4biz Inventory;
* [x] Having inventoried the configuration items; 

## Procedure

1. Install the GuaCD using the [official documentation][1] or download the container provided by 4biz. It's not necessary to install 
the guacamole-client, since 4biz only uses the Guacamole daemon, that is, the GuaCD;

2. After installation, set up the logs;

    ```sh
    /usr/local/sbin/guacd -b 0.0.0.0 > /var/log/guacd.log 2>&1
    ```

3. Download the (.jar) video encoder (in the partner portal downloads center) - which compiles the videos from the sessions;

4. Copy the video encoder to the server;

5. Perform the configuration by replacing the variables with the information of your server;

    ```java
    java -Durl=${4biz_PROTOCOL}://${4biz_URL}/4biz -DcontainerIdentifier=${4bizGUACD_ID} -DuserName=4biz.local\\${4biz_LOGIN} -Dpassword=${4biz_PASSWORD} -jar /4biz-guacd-encoder.jar &
    ```

6. Set directory for recording videos (eg.: /mp4);

    !!! Abstract "Video recording"
   
        After the remote access session ends, the generated video enters a compilation queue and then made available on the platform.           The time of compilation will depend on the time of the session, in addition, the beginning of the compilation is linked to the           cron routine defined in the remote access connection.
   
7. In the configuration item that will be accessed remotely (eg.: Windows Computer), install a remote access client with VNC protocol support (Example: [TightVNC][3]) and set an access password. Save this password as it will be used in the next step;   

8. Perform the registration of Remote Access connections in your instance [according to the document][4].

## What to do next

With GuaCD service active and communicable, the next step is to remotely access the configured CI.

## Related

[Configuration Management][5]

[Implement 4biz Inventory][6]

[1]:https://guacamole.apache.org/doc/gug/installing-guacamole.html
[3]:https://www.tightvnc.com/
[4]:/en-us/4biz-helium/processes/configuration/configuration/configure-remote-access.html
[5]:/en-us/4biz-helium/processes/configuration/overview.html
[6]:https://docs.run2biz.com/en-us/4biz-helium/additional-features/add-ons/inventory.html
