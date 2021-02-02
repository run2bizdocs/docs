Title: Requerimientos del Sistema

# Requerimientos del Sistema

Para ejecutar la plataforma y las aplicaciones, los requisitos del sistema recomendados pueden variar según el escenario de instalación.

## Aplicación y base de datos en el mismo servidor

Si instala todos los programas y la base de datos relacional en el mismo servidor, recomendamos que el servidor tenga al menos `32GB` de memoria para entornos de producción. Si solo desea realizar algunas pruebas o entornos de aprobación y desarrollo, un servidor de `16GB` es suficiente. En cuanto al tamaño del disco, recomendamos tener al menos `30 GB` de espacio disponible.

## Aplicación y base de datos desmembrados

Si ya tiene un servidor bancario relacional en su entorno, puede usarlo para instalar 4biz. En este caso, el servidor de aplicaciones debe tener al menos `16GB` de memoria. Para el servidor bancario, recomendamos al menos `4GB` para un entorno de producción.

!!! Warning "ATENCIÓN"

    Cualquiera que sea el caso, estos son los valores mínimos recomendados. Recuerda que la plataforma 4biz está compuesta por otras aplicaciones, como Builder, que permite integraciones con los más diversos propósitos. Estas integraciones pueden dar lugar a consumos y cargas de procesamiento diferentes de las normales, por lo que los valores de los requisitos del sistema pueden variar de un entorno a otro.   

# Versiones de paquete recomendadas

A partir de la versión Helium 1.2.23, la tabla de Versiones de Paquete Recomendadas, debe cambiarse para las bases de datos aprobadas:

|Aplicación|Versión|
|-------------- | ------ |
|Wildfly | `12.x` |
|Java JDK | `8.x` |
|PostgreSQL | `12` |
|Driver JDBC |`Depende de la versión de la base. En el documento usaremos la versión 9.3 porque postgreSQL estará en esta versión.` |
|SOLR | `6.4.2` |
|Sistema Operativo| Aunque se puede instalar en cualquier distribución y versión, el documento considera la distribución `Linux CentOS 7.x.`   |
|MongoDB   | `3.4.15`|
|Microsoft SQL Server|`2019`|
|Oracle| `12c`|

