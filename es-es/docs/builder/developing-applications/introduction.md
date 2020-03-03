title: Pasos para implementar la Solución Builder
Description: Pasos para implementar la Soluión Builder
# Pasos para implementar la Soluión Builder


![create Builder app](images/Builder-1.png)

Figura 1 - Crear aplicación Builder


![business](images/Builder-2.png)

Figure 2 - Objeto de negocios


!!! Abstract "ATENCIÓN"

    Los pasos se pueden encontrar en la documentación 4biz (docs.4biz.com).

## Diseñar App


Para un mejor desarrollo de las aplicaciones Builder, es necesario el **diseño anterior de las necesidades, requerimientos que la aplicación atenderá**, además de incluir el modelo de entidades de los datos que recorrerán la aplicación.

Una búsqueda de las **interfaces deseadas** y, si Builder es la opción de usar datos para servicios, el **diseño de los servicios** que serán automatizados.

## Configuración Builder


Después de Dibujar la Aplicación reuniendo la información referente a las entidades de datos de su Aplicación Builder, usted irá:

1.  Crear su BASE DE DATOS DE CONEXIÓN y su entrada APLICACIÓN Builder;

2.  Comprobar si va a utilizar cualquier DOMINIO común para su instalación y crear uno si es necesario;

3.  Usted también verificará las REGLAS DE NEGOCIO para el registro, actualización o exclusión de registros en la entidad de datos usted los vinculará al Objeto de Negocio;

4.  Si tiene formularios que utilizarán varios idiomas, creará las CLAVES DE INTERNACIONALIZACIÓN, labels que se utilizarán para todos los campos en sus formularios.

## Desarrollo Builder


El paso de configuración nos preparará para desarrollar la aplicación:

1.  Crear los OBJETOS DE NEGOCIO, conteniendo la estructura de datos de la entidad, en esta etapa usted podrá crear las columnas, PK's y FK's (asignar relaciones), vincular Reglas de Negocio y Dominios, además de poder crear Formularios CRUD y otros recursos;

2.  Crear FORMULARIOS relacionados a su Negocio.

## Conexión 4biz Experience


Después de haber creado sus Objetos de Negocio y Formularios, usted podrá:

1.  VINCULAR EL FORMULARIO A UN SERVICIO como necesario, o

2.  VINCULAR EL FORMULARIO AL MENÚ 4biz Experience O A UN CENTRO DE EXPERIENCIA, esto hará que pueda mantener tablas y datos adicionales que no se utilizarán en la apertura de un ticket



!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>03/20/2019 - Anna Martins  
