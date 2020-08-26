Title: Third party API

# Third party API

Our virtual assistant Helper provides an area to integrate external API with the chatbot. With this you can use third party API with all Helper resources. This integration is performed through a REST request and requires some steps to be configured.

## Procedure

1.  After access the platform, go to the menu "third party API”;

2.  The screen will present the API previously registered, if any, with the Edit and Delete options;

3.  If you want to search for a specific API, use the search field and click on "Search";

4. To register a new API, click on “New”. The following fields will appear to be completed:

| **Field**   | **Definition** |
|-|-|
| Name| Define the characteristic name of the API being registered.|
| Dependency | If necessary, identify whether that API being created previously requires the execution of another API.|
| Methode| Select which htpp method will be used by the API: POST, GET, PUT, DELETE or PATCH.|
| URL | Set the URL for the new API. If you want to include in the URL a context already registered in the virtual assistant, put the value between {}.|

Once the identification fields are completed, we will complete the necessary attributes to continue the REST requests: header, body, responses and settings.

## Headers

This function allows adding necessary values for the REST request header.

1.  Click on “+” to add the header with the information to:

\- Key;

\- Value.

2\.  Click on Save.

## Body

In the body it's possible to assemble the content that will be sent in the body of the request.

1.  Click on “+” to add the body with the information to:

    \- Format of body: JSON;

    \- Name;

    \- Type: text, number, boolean, list, object, context, chat history, last chat message, user ID, undefined value and empty value;

    \- Value: the value will depend on the type selected.

2\.  Click on Save.

## Responses

In responses we'll configure what we expect from this API.

1.  Click on “+” to add the information to:

\- Format of response: it can be in JSON or Text;

\- Name;

\- Type: text, number, boolean, list, object or context;

\- Identification.

2\.  Click on Save.

## Settings

Here we will define the request settings that will influence the assistant's understanding.

1.  Select the desired code to define the fields:

    \- Successful htpp status;

    \- Htpp status of unauthorized;

    \- Htpp status of not found.

    \* The options presented for these fields are pre-defined by the system.

2\.  Then, define the messages that will appear on the chatbot screen for the following cases:

   \- Chatbot message for content not found;

   \- Chatbot message for request failure;

3\.  Define whether the API being created is an authentication API.

4\.  Click on Save.
