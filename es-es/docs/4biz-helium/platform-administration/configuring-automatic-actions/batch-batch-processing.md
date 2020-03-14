title: Procesamiento Batch
Description: Tiene el objetivo de registrar el procesamiento batch, que podrá ser utilizado en otras rutinas del sistema.
# Procesamiento Batch

Esta funcionalidad tiene el objetivo de registrar el procesamiento batch, que podrá 
ser utilizado en otras rutinas del sistema.

Rutinas como:

   - Verificación de correo electrónico
   
   - Verificación de la hora del servidor
   
   - Distribución automática de Tickets con balance de carga de trabajo 

## Antes de empezar

El procesamiento Batch de 4biz utiliza Quartz para la programación y el procesamiento de rutinas de sistema. Por lo tanto, antes de utilizar cualquier rutina batch es necesario [configurar el Quartz][3].

Procedimiento
-------------

1.  Acceder al menú principal Sistema \> Procesamiento Batch;

2.  Hacer clic en "Nuevo";

3.  Completar los campos disponibles (descripción, tipo [clase Java,
    RhinoScript, SQL]; situación; expresión cron que define el tiempo de
    ejecución de la rutina y el contenido de la rutina, que se describirán en el
    contexto de la rutina para ser ejecutados en la herramienta);
    
    Ejemplo de contenido "Clase Java":
    ```html
    br.com.4biz.citcorpore.quartz.job.JobConfiguracaoAberturaAutomaticaViaEmail
    ``` 

4.  Hacer clic en "Guardar".

Rutinas Batch
-------------

-   Volver a la hora del servidor

    -   Tipo: RhinoScript
    -   Contenido:
    
        [Descargar Script][2]

-   Hacer la lectura de correo electrónico

    -   Tipo: Clase Java
    -   Contenido:

    ```java
    br.com.4biz.citcorpore.quartz.job.JobConfiguracaoAberturaAutomaticaViaEmail
    ```

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Larissa Lourenço


[1]:/es-es/4biz-helium/platform-administration/configuring-automatic-actions/images/verify-email.txt
[2]:/es-es/4biz-helium/platform-administration/configuring-automatic-actions/images/server-time.txt
[3]:/es-es/4biz-helium/get-started/installation-and-upgrade/perform-installation.html#configuracao-do-quartz
