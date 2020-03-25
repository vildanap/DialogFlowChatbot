# DialogFlowChatbot

> Based on user query inside chat (e.g. questions about working hours, booking appointment, etc.), and with help of API.AI Android SDK - text recognition is integrated with dialog scenarios created for agent inside Dialogflow project.

# Table of contents

* [Prerequisites](#Prerequisites)
* [Setup Android project](#Setup)
* [Screenshots](#screenshots)

## Prerequisites
* JDK 8
* Android Studio IDE
* Created Dialogflow project (Agent) and generated service credentials. Guide on: [Creating Dialogflow project](https://cloud.google.com/dialogflow/docs/quick/setup)

## Setup Android project

> Inside _build.gradle_ file dependency for API.AI Android SDK is **already** added. More on: [Link](https://github.com/dialogflow/dialogflow-android-client)
```
implementation 'ai.api:sdk:2.0.7@aar'
implementation 'ai.api:libai:1.6.12'
implementation 'com.google.cloud:google-cloud-dialogflow:0.67.0-alpha'
```
### Add _gradle.properties_ file to the project and paste your CLIENT_ACCESS_TOKEN inside it 
```
CLIENT_ACCESS_TOKEN = 'your token from Dialog Flow'
```
Note: CLIENT_ACCESS_TOKEN can be found inside your created Dialogflow project.
![client_access_token](https://github.com/vildanap/DialogFlowChatbot/screenshots/client_access_token.PNG)
### Service account 
Create _raw_ directory inside R.drawable. Inside it paste your private key file and name it _test_agent_credentials.json_. 
More about service account keys on: [Link](https://cloud.google.com/dialogflow/docs/quick/setup)
![client_access_token](https://github.com/vildanap/DialogFlowChatbot/screenshots/raw_file.PNG)

## Screenshots

