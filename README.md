# Smarty Postman Collections

Welcome to [Smarty](https://www.smarty.com), one of the fastest address verification and geocoding services available! This repository will help you familiarize yourself with the Smarty APIs. The following steps will guide you through creating a Smarty account and sending Smarty API requests using [Postman](https://www.postman.com/home).

## Table of contents
- [Getting started](#getting-started)
    - [Configuration](#configuration)
* [Making Smarty API calls](#making-smarty-api-calls)

## Getting started

Follow these steps to get started with the Smarty APIs:
1. [Sign up](https://www.smarty.com/signup) with Smarty to get a set of API keys that are required for interacting with the APIs. If you already have an account, [log in](https://www.smarty.com/login) with your credentials.
2. Click the "Run in Postman" button below. You will be directed to a new tab, then click the "Fork Collection" button. You will be required to create a [free account](https://www.postman.com/postman-account) with Postman.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/26488730-bc1bdca1-977e-4c98-b36c-ca8ccc5bf6c0?action=collection%2Ffork&collection-url=entityId%3D26488730-bc1bdca1-977e-4c98-b36c-ca8ccc5bf6c0%26entityType%3Dcollection%26workspaceId%3Da9f6b737-2143-4ddc-8e2b-0344eec8aaba#?env%5BSmarty%5D=W3sia2V5IjoiYXV0aC1pZCIsInZhbHVlIjoiWU9VUl9BVVRIX0lEIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6InNlY3JldCIsInNlc3Npb25WYWx1ZSI6IllPVVJfQVVUSF9JRCIsInNlc3Npb25JbmRleCI6MH0seyJrZXkiOiJhdXRoLXRva2VuIiwidmFsdWUiOiJZT1VSX0FVVEhfVE9LRU4iLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoic2VjcmV0Iiwic2Vzc2lvblZhbHVlIjoiWU9VUl9BVVRIX1RPS0VOIiwic2Vzc2lvbkluZGV4IjoxfV0=)

3. If you do not want to fork the collection using the "Run in Postman" button, you can download the JSON files from the postman-download folder in this repository. You will need to [import these](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#importing-postman-data) into Postman.
4. Once the Smarty APIs collection and the Smarty environment are imported into Postman, see the [Configuration](#configuration) section on how to configure API keys in the environment.

### Configuration

The Smarty Postman collection uses [Postman environment variables](https://learning.postman.com/docs/sending-requests/variables/#variables-quick-start") to provide authentication for each API request. These steps will help you set up the necessary environment variables to use the Smarty APIs.
1. Select the Smarty environment in the top right corner of Postman.
2. Click the eye icon to open the environment settings.
3. Open your Smarty account [Dashboard](https://www.smarty.com/account).
4. Select the [API Keys](https://www.smarty.com/account/keys) section on the left side of your Smarty Dashboard.

![image](https://user-images.githubusercontent.com/62493355/228678037-0d0e4911-2f32-43b7-a840-9f741d46fcc9.png)
5. Copy your Smarty API secret key information into each "current value" field in the Smarty environment:

    - `auth-id`
    - `auth-token`

![image](https://user-images.githubusercontent.com/62493355/228653244-8cf19b64-2a4c-4b7d-9a51-5c313880903c.png)

6. Save your changes in the environment and start making Smarty API requests!

## Making Smarty API calls

Once you have completed the steps in the Configuration section above, you are ready to make API requests using Postman! Complete the following steps to make your first API request.
1. Select the "Collection" pane on the left side of Postman. Expand the "Smarty API" folder on the left and navigate to Smarty API -> US Street Address API -> Single Address.
2. In the pane on the right, which has the options "Params", "Authorization", "Headers" etc. click on the "Params" tab.
3. Update the "license" parameter value using the license value on your Smarty Dashboard [subscriptions tab](https://www.smarty.com/account/subscriptions). Each license value is associated with different API requests. (insert information on what APIs use each license?)
4. (Optional) If you want, update the parameter values to match the address you would like to send to the API, such as `street`, `city`, etc.
5. Click the blue "Send" button on the right.
6. The response body should appear in Postman. If there was an error, an error message will show in the response body.
7. Continue trying Smarty APIs! Be aware that you will only have access to the APIs that use the subscription(s) that you currently have. You can sign up for free trials [here](https://www.smarty.com/account).
