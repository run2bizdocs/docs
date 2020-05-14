title: Batch Processing
Description: Intended to register the batch processing, that can be used in other system routines.
# Batch Processing

This functionality is intended to register the batch processing, that can be
used in other system routines.

Routines like:

   - Email verification
   
   - Server time verification
   
   - Automatic ticket distribution with workload balancing 
   
## Before getting started

4biz Batch processing uses Quartz for scheduling and processing system routines. Therefore, before using any batch routine it is necessary to [configure Quartz][3].   

Procedure
-------------

1.  Access the functionality through the main menu System \> Batch Processing;

2.  Click on "New";

3.  Complete the fields available (description, type [Java class, RhinoScript,
    SQL]; status; cron expression that defines the routine execution time and
    the context of the routine to be executed in the system);
    
    Example of "Class Java" content:
    ```html
    br.com.4biz.citcorpore.quartz.job.JobConfiguracaoAberturaAutomaticaViaEmail
    ```

4.  Click on "Save".

Batch Routines
------------------

-   Return server time

    -   Type: RhinoScript
    -   Content:
    
        [Download Script][2]

-   Perform e-mail reading

    -   Type: Java class
    -   Content:
    
    ```java
    br.com.4biz.citcorpore.quartz.job.JobConfiguracaoAberturaAutomaticaViaEmail
    ```


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020



[1]:/en-us/4biz-helium/platform-administration/configuring-automatic-actions/images/verify-email.txt
[2]:/en-us/4biz-helium/platform-administration/configuring-automatic-actions/images/server-time.txt
[3]:/en-us/4biz-helium/get-started/installation-and-upgrade/perform-installation.html#configuracao-do-quartz
