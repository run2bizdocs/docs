title: Configure BI solution (Smart Analytics) via Docker
Description: This document is intended to configure the BI in the 4biz instance.
# Configure BI solution (Smart Analytics) via Docker

4biz Analytics is a solution of Business Intelligence (BI) for analyzing the data
from 4biz. The BI solution uses resources of the tools [Saiku
Analytics](https://www.meteorite.bi/products/saiku-reporting) and [Pentaho](https://www.hitachivantara.com/go/pentaho.html).

It's possible to have BI in your environment using the container structure of
Docker, following the installation configuration.

Before getting started
----------------

The user must have Docker previously installed.

Procedure
------------

***Installation***

1.  Download citBI in:

    ftp://ftpgo.4biz.com.br/10104_DIRETORIA_DE_SOLUCOES/PUBLICO/citBI/citbi-1.0.0/citbi-1.0.0.zip and then unzip

1.  Enter the command and then unzip:

    
    cd /citbi/files/
    
    ```sh
    unzip storage.zip
    ```
    command to build image
    
    cd/citbi/
    
    ```
    docker build -t registry.4bizcloud.com/templates/bi .
    ```
    
1.  In the folder /citbi/composes, configure the database:
    ```sh
    vi /citbi/composes/
    [docker-compose.yml](/citbi/src/master/composes/docker-compose.yml)
    ```
    
    i (enter)

    ```java
    version: '2'
    services:
      citBI:
        container_name: citBI
        image: registry.4bizcloud.com/templates/bi:latest
        environment:
    - BI_HOST=127.0.0.1
    - BI_DATABASE= 4biz_equipeteste_equatorial
    - BI_PORT=5432
    - BI_USER=root
    - BI_PASSWORD=1
    - BI_LANGUAGE=pt-br
    - URL_SAIKU=http://localhost:8282
    volumes:
    - /citbi/files/home:/home
    ports:
    - 8282:8282
    - 8085:8085
    ```

    Ctrl+C

    :wq!
    
    Check:

    ```
    cat /citbi/composes/docker-compose.yml
    ```

1.  In the folder /citbi/composes:

Build and start container:

```
docker-compose up -d
```

Verify log of container:

```
docker logs -f citBI
```

***Configuration***

1.  Access the Saiku as a manager:

    <http://127.0.0.1:8282/>

2.  Add the Schema available on:

     /citbi/src/master/files/SchemaEnglish.xml

3.  Add DataSource:

    jdbc:postgresql://127.0.0.1:5432/4biz_equipeteste_equatorial

***Useful commands: box***

1.  Verify active containers:

    ```
    docker ps
    ```

1.  Verify inactive containers:
    
    ```
    docker ps -a
    ```

1.  Stop container:
    
    ```
    docker stop citBI
    ```

1.  Remove container:
    ```
    docker rm citBI
    ```

What to do next
------------------

1. To enjoy the benefits of BI in your 4biz instance, it's necessary to
configure the parameters 401 and 412. To do so, access the main menu
Parametrization \> 4biz Parameters;

2. Detais of the parameters:

    -   401: URL of Saiku server

    Example: http://127.0.0.1:8282

    -   412: Job to update the password Saiku

    Example:
    http://127.0.0.1:8282/kettle/executeJob/?job=/home/ec2-user/repo-cit/job_create_users_saiku.kjb&loginParam=login4biz


Related
-----------

[Using Smart Analytcs (BI) to generate reports](/en-us/4biz-helium/additional-features/smart-analytics/use-bi-solution.html)



!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
