title: Construir y mantener informes Smart - V. 8.0
Description: Proveer la facilidad de elaboración de informes personalizados con los datos de las funcionalidades requeridas, sin necesidad de nuevas actualizaciones o software adicional.
# Construir y mantener informes Smart - V. 8.0


Esta funcionalidad tiene el objetivo de proveer la facilidad de elaboración de
informes personalizados con los datos de las funcionalidades requeridas, sin
necesidad de nuevas actualizaciones o software adicional.

Antes de empezar
--------------------

- [x] Es necesario tener permiso de acceso. 

- [x] Para utilizar el Designer es necesario definir el nombre del Schema de la base de datos a partir del parámetro 32 (por ejemplo: public).

- [x] Es necesario conocimientos de Standard Query Language (SQL) para crear o manipular informes.

Procedimiento
-----------------

1.  Acceder al menú principal Informes \> Informes Smart \> Generador de
    Informes Smart;

2.  Hacer clic en "Nuevo";

3.  Completar los campos necesarios. Definir el tipo:

       +  **SQL**: crea un Sub Informe "SQL" (este tipo permite crear informes que
        devuelven la información de la Base de datos a través de una consulta).
        Al seleccionar esta opción, será necesario informar también el tipo de
        informe que se va a crear, la regla de negocio correspondiente, el
        diseñador del informe, el parámetro y el script;

       +  **RhinoScript**: crea un informe que devuelve la información de la base de
        datos a través de un "script" es necesario seleccionar el tipo
        "RhinoScript". Es necesario elegir el tipo de informe, definir los
        parámetros y describir el script;

       +  **JSP**: crea un informe con contenido dinámico, el tipo elegido debe ser el
        "JSP". Al optar por este tipo, deberá informar los parámetros y el
        script "JSP";

       +  **Builder**: crea un informe del tipo "Builder", basta enlazar un formulario
        "Builder" previamente registrado.

    !!! Abstract "NOTA"

        Para crear un Sub Informe (Drill) el" Tipo de informe "debe ser"
        Gráfico de pizza "o" Gráfico de barra".

4.  Definir el módulo (funcionalidad) donde se muestra el informe que se está
    creando:

    -   **N/A**: seleccionar esta opción si desea que el informe no aparezca en
    ningún módulo;

    -   **General**: seleccionar esta opción para ver el informe en uno o más
    módulos, donde desea que el informe aparezca (Configuración,
    Incidentes/Solicitudes (gráfico), Incidentes/Solicitudes, Liberación,
    Cambios, Problemas);

    -   **Específico**: seleccionar un solo módulo donde desea que el informe
    aparezca (Configuración, Incidentes/Solicitudes (gráfico),
    Incidentes/Solicitudes, Liberación, Cambios, Problemas).

5.  Hacer clic en "Guardar";

6.  También existe la posibilidad de importar un informe. Para intentar, haga
    clic en "Importar" y vincular el archivo conteniendo la información que
    quiera;

    !!! Abstract "ATENCIÓN"

        Los informes aquí creados aparecerán en la pantalla de "Informes Smart",
        donde podrá ver los datos pertinentes de cada informe.



Relacionado
-------

[Emitir informe utilizando Smart Report](/es-es/4biz-helium/additional-features/reports/create/smart-reports/configuration/create-smart-report.html)


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
