# Introduction

The feedback review can be used to ad hoc feedback for performance for colleagues, for example during mid year review , end of year review or any adhoc review.
The app can help to provide constructive, clear, and respectful feedback for work colleagues. Feedback is generated based on a rating scale from 1 to 5, where 1 represents poor performance and 5 represents excellent performance with the help of Copilot Agent which opens up on the side panel within the app as well as Azure Open AI chat completion to generate a sample.
It connects to the Azure AI Content and Safety feature as well to ensure there is no element of hate, self harm, harm, sexual and violence in the feedback. Using phrases like "You are lazy" or "Stop mansplaining" which might cause distress and prejudice to the recipients will be stopped by the Azure Content and Safety check before sending the feedback.

## Solution components

The solution contains the following
 - 1 Copilot Studio Agent : Colleague Feedback Agent with agent components
 - 1 Canvas app : Feedback
 - 2 Cloud flows : 'Content Safety Check' and 'Execute Feedback Copilot'
 - 3 connection references : Office 365 Users, Office 365 Groups, Office Outlook
 - 4 Environment variables: Azure AI Content Safety Endpoint, Azure AI Content Safety key, Azure AI OpenAI Endpoint and Azure AI OpenAI Endpoint key

## Steps to import solution

Create Azure AI Foundry and deploy a model for Azure Open AI

1. Navigate to a Power App environment, https://make.powerapps.com/ and select your environment
2. Import the solution zip file FeedbackReview_1_0_0_3.zip
3. Associate or create the connections: Outlook, M365 Users and M365 Groups when prompted
[Connections](./assets/Connection_create.png)
4. Fill in the environment variables with Azure AI Content Safety Endpoint, Azure AI Content Safety key, Azure AI OpenAI Endpoint and Azure AI OpenAI Endpoint key from Azure AI Foundry resources.
[Environment Variables](./assets/Environ_Variables.png)    
