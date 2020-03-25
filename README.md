# DialogFlowChatbot

> Based on user query inside chat (e.g. questions about working hours, booking appointment, etc.), and with help of API.AI Android SDK - text recognition is integrated with dialog scenarios created for agent inside Dialogflow project.

# Table of contents

* [Prerequisites](#Prerequisites)
* [Setup for local development](#Setup Android project)
* [Status](#status)

## Prerequisites
* JDK 8
* Android Studio IDE
* Created Dialogflow project (Agent) and generated service credentials ![Creating Dialogflow project guide](https://cloud.google.com/dialogflow/docs/quick/setup)

## Setup Android project

> Inside build.gradle dependency for API.AI Android SDK is already added. More on: ![Link](https://github.com/dialogflow/dialogflow-android-client)

### Add _gradle.properties_ file to your project and paste inside it your CLIENT_ACCESS_TOKEN
```
CLIENT_ACCESS_TOKEN = 'your token from Dialog Flow'
```
Note: CLIENT_ACCESS_TOKEN can be found inside your created Dialogflow project.
!(client_access_token.PNG)()
### Service account 
Create _raw_ directory inside R.drawable. Inside it paste your private key file and name it _test_agent_credentials.json_ 
More about service account keys on: ![Link](https://cloud.google.com/dialogflow/docs/quick/setup)
