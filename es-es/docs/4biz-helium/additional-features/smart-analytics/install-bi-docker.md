title: Configurar solución BI (Smart Analytics) vía Docker
Description: Este documento tiene por objetivo configurar el BI en la instancia 4biz.
# Configurar solución BI (Smart Analytics) vía Docker

4biz Analytics es la solución de Business Inteligence (BI) para el análisis de los
datos del 4biz. La solución de BI utiliza recursos de las herramientas [Saiku
Analytics](https://www.meteorite.bi/products/saiku-reporting) y [Pentaho](https://www.hitachivantara.com/go/pentaho.html).

Es posible tener el BI en su ambiente utilizando la estructura de contenedores del
Docker, debiendo seguir la siguiente configuración de instalación.

Antes de empezar
----------------

El usuario deberá tener Docker previamente instalado. 


Procedimiento
------------

***Instalación***

1.  Descargue el citBI en:

    ftp://ftpgo.4biz.com.br/10104_DIRETORIA_DE_SOLUCOES/PUBLICO/citBI/citbi-1.0.0/citbi-1.0.0.zip y descomprimir

1.  Escriba el comando y, a continuación, descomprimir:

    
    cd /citbi/files/
    
    ```sh
    unzip storage.zip
    ```
    comando para construir imagen
    
    cd/citbi/
    
    ```
    docker build -t registry.citsmartcloud.com/templates/bi .
    ```
    
1.  En la carpetar /citbi/composes, configurar la base de datos:
    ```sh
    vi /citbi/composes/
    [docker-compose.yml](/citbi/src/master/composes/docker-compose.yml)
    ```
    
    i (introducir)

    ```java
    version: '2'
    services:
      citBI:
        container_name: citBI
        image: registry.citsmartcloud.com/templates/bi:latest
        environment:
    - BI_HOST=127.0.0.1
    - BI_DATABASE= citsmart_equipeteste_equatorial
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
    
    Conferir:

    ```
    cat /citbi/composes/docker-compose.yml
    ```

1.  En la carpeta /citbi/composes:

Construir e iniciar el contenedor:

```
docker-compose up -d
```

Verificar el registro del contenedor:

```
docker logs -f citBI
```

***Configuración***

1.  Acceder al Saiku como administrador:

    <http://127.0.0.1:8282/>

2.  Añadir Schema disponible en:

      /citbi/src/master/files/SchemaEnglish.xml

3.  Añadir DataSource:

    jdbc:postgresql://127.0.0.1:5432/citsmart_equipeteste_equatorial

***Comandos útiles: caja***

1.  Verificar los contenedores activos:

    ```
    docker ps
    ```

1.  Verificar contenedores inactivos:
    
    ```
    docker ps -a
    ```

1.  Parar contenedor:
    
    ```
    docker stop citBI
    ```

1.  Remover contenedor:
    ```
    docker rm citBI
    ```

Lo que hacer después
------------------

1. Para disfrutar de los beneficios del BI en su instancia 4biz, es necesario
configurar los parámetros 401 y 412. Para ello, acceder al menú principal
Parametrización \> Parámetros 4biz;

2. Detalles de los parámetros:

    -   401: URL del servidor Saiku

    Ejemplo: http://127.0.0.1:8282

    -   412: Job para actualizar la contraseña Saiku

    Ejemplo:
    http://127.0.0.1:8282/kettle/executeJob/?job=/home/ec2-user/repo-cit/job_create_users_saiku.kjb&loginParam=loginCitSmart


Relacionado
-----------

[Usar Smart Analytics (BI) para generar informes](/es-es/4biz-helium/additional-features/smart-analytics/use-bi-solution.html)



!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021
