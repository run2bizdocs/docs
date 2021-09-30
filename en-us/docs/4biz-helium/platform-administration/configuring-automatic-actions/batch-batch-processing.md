title: Batch Processing
Description: This functionality allows for the registration of batch processing routines, that can be later used in other system routines.

# Batch Processing

This functionality allows for the registration of batch processing routines, that can be later used in other system routines.

These Routines include:

    •	Email verification

    •	Server time verification

    •	Automatic ticket distribution with workload balancing

   
## Before getting started

4biz Batch processing uses Quartz for scheduling and processing system routines. Therefore, before using any batch routine it is necessary to  [configure Quartz][3].   

## Procedure

1.	Access the functionality through the main menu System > Batch Processing;
2.	Click on "New";
3.	Fill in the available fields (description, type [Java class, RhinoScript, SQL]; status; cron expression that defines the routine execution time and the context of the routine to be executed in the system);

Example of "Class Java" content:

br.com.4biz.citcorpore.quartz.job.JobConfiguracaoAberturaAutomaticaViaEmail

4\.	Click on "Save".



!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021



[1]:/en-us/4biz-helium/platform-administration/configuring-automatic-actions/images/verify-email.txt
[2]:/en-us/4biz-helium/platform-administration/configuring-automatic-actions/images/server-time.txt
[3]:/en-us/4biz-helium/get-started/installation-and-upgrade/perform-installation.html#configuracao-do-quartz
