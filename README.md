# Integrating Watson Assistant Webchat w/ Salesforce ServiceDesk 

In this repo we will illustrate two usecases: 
- Watson Assistant Webchat integration with SalesForce Service Desk to a Live Agent handoff 
- Live Agent - Agent Assist usecase incorporating Watson Assistant with Watson Discovery

## Terms

We will define a few terms:<br />
User: This will be a customer that will interact via chat(Watson Assistant) to a live agent<br />
SalesForce ServiceCloud: App that helps deliver fast, personalized customer service & improves customer satisfaction to help agents deliver the right answers and service insights<br />
Live Agent: This will be the service desk employee who will interact with SalesForce ServiceCloud to receive chat handoff

## Setup
This is a two part setup. The first is Salesforce Service Cloud Setup and the second is Watson Assistant Web Chat setup.

### Part 1 - Salesforce Setup & ServiceCloud setup 

- Obtain a Salesforce instance with Administrator access and log in
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/sflogin.png)

- Go to service app
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/serviceapp.png)

- Click on gear and go to service settings
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/SalesForceSysAdminProfile.png)

- Ensure ServiceCloud user & chat user is checked on the user profile you are testing with by using QuickFind and searching "users"
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/quickfinduser.png)

![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/SalesForceSysAdminProfile.png)
- Enable Omni Channel Settings by utilizing QuickFind

### Part 2 - Watson Assistant Web Chat setup
