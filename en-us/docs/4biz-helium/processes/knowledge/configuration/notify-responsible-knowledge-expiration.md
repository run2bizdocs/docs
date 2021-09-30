title: Notify responsible for the knowledge expiration
Description: Configure the e-mail notification to notify the responsible (creator and publisher) about the expiration of knowledge.

# Notify responsible for the knowledge expiration

This knowledge is intended to guide into the configuration of the e-mail notification to notify the responsible (creator and publisher) about the expiration of knowledge article.

## Before getting started

It's necessary to have at least one knowledge registered in the knowledge base.

**Procedure**

1. Configure the parameter 78 with the amount of the days previous to the knowledge expiration, which is intended to notify the responsible for the knowledge;

2.	Create a routine for the batch processing notification:
        •	Access the functionality through the main menu System > Batch Processing and click on "New";
        •	Define the routine description, select the type "Java Class" and put the situation as "Active";
        •	Select the appointment as "Daily" and indicate the time at which the routine process will happen;
        •	In the area "Content", copy the script below:
        •	br.com.4biz.citcorpore.quartz.job.VerificaValidadeBaseConhecimento
        •	Click on "Save".

3.	It's possible to customize the email template. Just access the functionality through the main menu System > Settings > Email template, select the email template with ID = "7" and make the needed change.


Related
-------

[Configure parametrization - knowledge](/en-us/4biz-helium/platform-administration/parameters-list/configure-parametrization-knowledge.html)

[Create knowledge](/en-us/4biz-helium/processes/knowledge/use/create-knowledge.html)


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021
