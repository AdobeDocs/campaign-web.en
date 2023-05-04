---
audience: end-user
title: Work with workflows channel activities
description: Learn how to use channel activities into Adobe Campaign Web workflows
badge: label="Alpha" type="Positive"
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
---
# Channel activities {#channel}

Adobe Campaign Web enables you to automate and execute marketing campaigns across multiple channels, such as email, SMS, or push. With Adobe Campaign  workflows, you can combine channel activities into the canvas to create cross-channel workflows that can trigger actions based on customer behavior. 

For example, you can create a welcome email campaign that includes a series of messages across different channels, such as email, SMS, and push. You can also send a follow-up email after a customer has completed a purchase or send a personalized birthday message to a customer via SMS. 

By using channel activities, you can create comprehensive, personalized campaigns that engage customers across multiple touchpoints and drive conversions.

Channel activities are available from the palette, on the left-hand side of the screen, in the Channels section.

## Email {#email}

description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow


The Email delivery activity allows you to configure the sending an email in a workflow. 

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->