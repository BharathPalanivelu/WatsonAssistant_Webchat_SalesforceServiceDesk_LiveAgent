# Integrating Watson Assistant Webchat w/ Salesforce ServiceDesk 

In this repo we will illustrate two usecases: 
- Watson Assistant Webchat integration with SalesForce Service Desk to a Live Agent handoff 
- Live Agent - Agent Assist usecase incorporating Watson Assistant with Watson Discovery

## Terms

We will define a few terms:<br />
User: This will be a customer that will interact via chat(Watson Assistant) to a live agent<br />
SalesForce ServiceCloud: App that helps deliver fast, personalized customer service & improves customer satisfaction to help agents deliver the right answers and service insights<br />
Live Agent: This will be the service desk employee who will interact with SalesForce ServiceCloud to receive chat handoff
Omni-channel:
Routing Configuration:
Queue:


## Setup
This is a two part setup. The first is Salesforce Service Cloud Setup and the second is Watson Assistant Web Chat setup.

### Part 1 - Salesforce Setup & ServiceCloud setup 

- Obtain a Salesforce instance with Administrator access and log in
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/sflogin.png)


- Go to service app
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/serviceapp.png)


- Click on gear and go to service settings
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/setup.png)
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/SalesForceSysAdminProfile.png)

- Ensure ServiceCloud user & chat user is checked on the user profile you are testing with by using QuickFind and searching "users"
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/quickfindusers.png)
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/SalesForceSysAdminProfile.png)


- Enable Omni Channel Settings by utilizing QuickFind
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/omnichannel.png)


- Setup a routing configuration
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/routingconfiguration.png)


- Presence Config(DO NOT HAVE TO CHANGE) shows the max capacity of both cases & chats your agent can handle
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/presenceconfig.png)

- Setup agents available and not available status to external users for chat, you create one per channel per agent
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/presencestatus.png)
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/presencestatus_chat.png)


- Assign chat statuses to an agent(user profile)
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/servicepresencestatusesaccess.png)
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/agentchatoptions.png)


- OPTIONAL: Add Service Channels(if applicable) e.g. Cases
![test](https://github.com/bmguillo/WatsonAssistant_Webchat_SalesforceServiceDesk_LiveAgent_AgentAssist/blob/master/img/servicechannels.png)




### Part 2 - Watson Assistant Web Chat setup
