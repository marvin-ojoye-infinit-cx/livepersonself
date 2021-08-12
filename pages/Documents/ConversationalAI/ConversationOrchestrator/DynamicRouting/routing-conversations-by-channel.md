---
pagename: Routing Conversations by Channel
redirect_from:
Keywords:
sitesection: Documents
categoryname: "Conversational AI"
documentname: Conversation Orchestrator
subfoldername: Dynamic Routing
permalink: conversation-orchestrator-dynamic-routing-routing-conversations-by-channel.html
indicator: messaging
---

You can create policies to recognize a consumer's channel: Web, Facebook Messenger, and so on, and transfer to the appropriate agent or skill. This is very useful in cases where you have specialized skills or agents for respective channels.

**Examples** 
* When a consumr messages from Facebook Messenger, transfer them to the FBMessengerSkill.
* When a consumer messages from the Web channel, transfer them to WebSkill.

### Prerequisites
* [Configure the routing bot](conversation-orchestrator-dynamic-routing-getting-started.html).
* Deploy the engagement and campaign on the respective channel.
 
### Process

1. Modify your routing bot to power the desired experience. In the example below, the bot responds to a customer greeting of “Hi," "Hello," etc., and immediately performs dynamic routing.

    <img class="fancyimage" width="800" src="img/convorchestrator/co_dr_routechannel1.png">

2. In the Dynamic Routing interaction, click **Manage routing policies** to go to the policy management interface.

3. Create the policy by selecting “orchestrator.channel” as the attribute and “channel’ as data type. Then choose from the available list of channels.

    <img class="fancyimage" width="800" src="img/convorchestrator/co_dr_routechannel3.png">       
 
4. Save and enable the policy.

    <img class="fancyimage" width="800" src="img/convorchestrator/co_dr_routechannel4.png"> 

5. Launch a messaging conversation from the respective channel and test the flow.
 
    For example, launch messaging from Facebook Messenger. Start by saying “Hi. And then immediately get routed to the respective skill. Here below, “Agentbob” is an agent who is mapped to the User3Skill.

    <img class="fancyimage" width="250" src="img/convorchestrator/co_dr_routechannel5.png">

6. You can also create one such policy for every unique channel. And you can also add more conditions to the policies if required.

    <img class="fancyimage" width="800" src="img/convorchestrator/co_dr_routechannel4.png">