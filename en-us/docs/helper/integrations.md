Helper already integrates natively with 4biz, so it's very easy to add it to your environments

# Integrations

Integrations with the virtual assistant Helper concern the channels on which the administrator will make the assistant available. This functionality will allow the insertion of the links of the desired platforms to integrate the virtual assistant with the selected system.

We will see later that the chatbot can be integrated natively with 4biz, in addition to Facebook or the user's own system through API Rest.

## Procedure

1.  After access the platform, go to the menu "Integrations”;

2.  The following integration options will be presented: Facebook Messenger, 4biz and API Rest;

3.  Select which option you want to integrate.

## 4biz

Helper already integrates natively with 4biz, so it's very easy to add it to your environment.

To perform the integration, you need to configure the necessary parameters in your own production environment. To do this, access the system and in side menu, select Parameterization > 4biz Parameters.

Find and complete the following parameters:

|Parameter| Value|
|-|-|
| 402 Helper Assistant - External URL     | http://[server-name].helperassistant.com                                     |
| 441 Helper Assistant - Conversation API | http://[server-name][acronym-language].helperassistant.com/webhooks/rest/webhook |
| 442 Helper Assistant - Parameters API   | http://[server-name][acronym-language].helperassistant.com/conversations/        |

!!! info "Important"

    The values to be completed in the parameters above will depend on the value presented in the Helper tool. To do this, access your virtual assistant and select "Integrations". To integrate with the platform, select “4biz” and the values for copying and pasting will be shown in the value of the 4biz platform itself. These parameters cannot be changed by the client.


## Facebook Messenger

It's also possible to integrate the Helper virtual assistant with Facebook Messenger chat. In this case the instructions are provided by Facebook itself and we provide the necessary information to perform the integration:

- Callback URL

-  Verify Token

-  Secret

-  Page Access Token


## API Rest

In this functionality the customer can customize the virtual assistant for another channel. For example, if the customer already has an institutional website and wants to include the virtual assistant for their chat. To do so, simply select the API Rest communication option.

API Rest is the communication protocol of the virtual assistant. It contains the following information to successfully integrate it:

-   Endpoint

-   Method

-   Media Type

And the formats needed for integration:

-   Format of sending messages to the bot:


` {"sender": "jhon", "message": "tell me something about you" } `



-   Return format of bot message in text:

` { "recipient_id": "jhon", "text": "I can help you work smarter, rather than harder" }`



-   Return format of bot message in button:


` { "recipient_id": "jhon", "text": "Could you rate my service??", "buttons": [ { "title": "Yes", "payload": "yes" }, {"title": "No","payload": "no" } ] }`



-   Return format of bot message in image:

` {"image": "https://helperassistantimages.s3.amazonaws.com/dev/fe711b50-d974-11e9-9622-94de80f33bee.png",   "recipient_id": "jhon"} `

Or

` {"attachment": "https://helperassistantimages.s3.amazonaws.com/dev/fe711b50-d974-11e9-9622-94de80f33bee.png","recipient_id": "jhon"} `

