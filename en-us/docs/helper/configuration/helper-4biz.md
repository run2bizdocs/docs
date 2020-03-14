Title: Making Helper available on the 4biz interface
# Making Helper available on the 4biz interface

Helper is already natively integrated with 4biz, so it is easy to add it to your environment.

## Procedure

1. With Administrator access, access the 4biz parameter screen;
2. Change the parameter value “402 Helper Assistant - External URL” to http://[name-server].helperassistant.com    
3. Change the parameter value “441 Helper Assistant - Conversation API” to http://[name-server][acronym-language].helperassistant.com/webhooks/rest/webhook and click on “Save”   
4. Change the parameter value “442 Helper Assistant - Parameters API” to http://[name-server][acronym-language].helperassistant.com/conversations/
5. Configure parameter 453 "Default Helper Assistant Fallback Message", with a message that Helper will answer whenever it has no answer to that question.
6. Enable parameter 423 "Enable Helper Assistant in the internal area of the system", a parameter that allows analysts to iterate with ANUVA
7. Enable parameter 450 "Enable Helper Assistant in the external area of the system", parameter that allows end users to iterate with ANUVA.    
    

!!! note "NOTE"
    
    For the acronym of the languages, use EN (English) and PT (Portuguese-Brazil).
    If these parameters are not available, upgrade your version of 4biz.
   
 
!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>04/07/2019 - Anna Martins
