# Camunda Ad Hoc Example
This is an example of how you can use BPMN's adhoc subprocess to make for far more dynamic processes. 

![ProcessTokenSim](./img/ProcessWithTokenSim.gif)

## What it does
This is BPMN model that is executable by Camunda 8/Zeebe. It works by asking a user to ask a question via a front end and then they can select one or more services. 
1. Answer Question with AI
1. A Friend Answers the Question
1. Set a reminder about the question

An Ad-hoc subprocess then activates the tasks selected and runs them in parallel.

### Addional Functionality. 
1. Starting an event subprocess with an escelation event.
1. Wait and resume functionality with Signals
1. SendGrid Connector for sending emails
1. OpenAI Connector for geting ChatGPT prompts answered
