---
audience: end-user
title: Use the Email workflow activity
description: Learn how to use the Email workflow activity
badge: label="Alpha" type="Positive"
---

# Email, SMS, Push {#email}

Adobe Campaign Web allows you to automate and execute marketing campaigns across multiple channels, such as email, SMS, or push. You can combine channel activities into the canvas to create cross-channel workflows that can trigger actions based on customer behavior. 

For example, you can create a welcome email campaign that includes a series of messages across different channels, such as email, SMS, and push. You can also send a follow-up email after a customer has completed a purchase or send a personalized birthday message to a customer via SMS. 

By using channel activities, you can create comprehensive and personalized campaigns that engage customers across multiple touchpoints and drive conversions.

Here are the steps to add a **Channel** activity in a workflow:

1. Make sure you have added a **Build audience** activity. The audience is the main target of your delivery: the recipients who receive the messages. When sending messages in the context of a campaign workflow, the message audience is not defined in the channel activity, but in the **Build audience** activity. See [this section](build-audience.md).

    ![](../../msg/assets/add-delivery-in-wf.png)

1. Select a delivery activity: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Push notification (Android)]** or **[!UICONTROL Push notification (iOS)]**.

1. Select a **Template**. Templates are pre-configured delivery settings saved for future use. [Learn more](../../msg/delivery-template.md)

1. Click **Create delivery** and define your message the same way you create a standalone delivery. [Learn more](../../msg/gs-message.md)


1. Start the workflow, and check logs.

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->



<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
