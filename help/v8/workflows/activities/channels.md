---
audience: end-user
title: Use a delivery workflow activity
description: Learn how to add a delivery workflow activity (Email, Push, SMS, Direct mail)
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
---
# Email, SMS, Push, Direct mail activities {#channel}

Adobe Campaign Web allows you to automate and execute marketing campaigns across email, SMS, direct mail, and push channels. You can combine channel activities into the workflow canvas to create cross-channel workflows that trigger actions based on customer behavior and data.

For example, create a welcome email campaign that includes a series of messages across different channels, such as email, SMS, push, and direct mail. You can also send a follow-up email after a customer completes a purchase or send a personalized birthday message to a customer via SMS.

By using channel activities, create comprehensive and personalized campaigns that engage customers across multiple touchpoints and drive conversions.

>[!NOTE]
>
>You can also create a one-shot delivery outside the context of a campaign workflow. Learn more in these sections:
>* [Create standalone email delivery](../../email/create-email.md)
>* [Create standalone SMS delivery](../../sms/create-sms.md)
>* [Create standalone push delivery](../../push/create-push.md)
>* [Create standalone direct mail delivery](../../direct-mail/create-direct-mail.md)

## Prerequisites {#channel-activity-prereq}

Start building your workflow with the relevant activities:

* Before inserting a channel activity, define the audience. The audience is the main target of your delivery: the profiles who receive the messages. When sending messages in the context of a campaign workflow, the message audience is not defined in the channel activity but within a dedicated activity, such as:
    
    * A **Build audience** activity. [Learn more](build-audience.md).

        ![Screenshot showing the addition of a delivery in a workflow](../../msg/assets/add-delivery-in-wf.png)
    
    * A **Load file** activity followed by a **Reconciliation** activity. [Learn more](load-file.md).

        ![Screenshot showing workflow reconciliation criteria](../assets/workflow-reconciliation-criteria.png)

* To send a recurring delivery, start your workflow with a **Scheduler** activity. Use a **Scheduler** activity for one-shot single deliveries to set the contact date for that delivery. That contact date can also be set in the delivery settings. See [this section](scheduler.md).

## Configure the Channel activity {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="Email activity"
>abstract="The Email activity facilitates email sending within your workflow, allowing for both one-time and recurring messages. It automates the process of sending emails to a target calculated within the same workflow. You can combine channel activities into the workflow canvas to create cross-channel workflows that trigger actions based on customer behavior and data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="SMS activity"
>abstract="The SMS activity facilitates SMS sending within your workflow, allowing for both one-time and recurring messages. It automates the process of sending SMS to a target calculated within the same workflow. You can combine channel activities into the workflow canvas to create cross-channel workflows that trigger actions based on customer behavior and data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="Push iOS activity"
>abstract="The Push iOS activity streamlines the process of sending iOS Push notifications as part of your workflow. It enables the delivery of both one-time and recurring messages, automating the sending of iOS Push notifications to a predefined target within the same workflow. You can combine channel activities into the workflow canvas to create cross-channel workflows that trigger actions based on customer behavior and data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Push Android activity"
>abstract="The Push Android activity streamlines the process of sending Android Push notifications as part of your workflow. It enables the delivery of both one-time and recurring messages, automating the sending of Android Push notifications to a predefined target within the same workflow. You can combine channel activities into the workflow canvas to create cross-channel workflows that trigger actions based on customer behavior and data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_directmail"
>title="Direct mail activity"
>abstract="The Direct mail activity facilitates direct mail sending within your workflow, allowing for both one-time and recurring messages. It automates the process of generating the extraction file required by direct mail providers. You can combine channel activities into the workflow canvas to create cross-channel workflows that trigger actions based on customer behavior and data."

To set up a delivery in the context of a workflow, follow the steps below:

1. Add a channel activity: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Push notification (Android)]**, **[!UICONTROL Push notification (iOS)]**, or **[!UICONTROL Direct mail]**.

1. Select the **Type of delivery**: single or recurring. 

   * A **Single delivery** is a one-shot delivery sent only once, such as a Black Friday email.
   * A **Recurring delivery** is sent multiple times based on its execution frequency defined in a [scheduler activity](scheduler.md). Each time the workflow runs, the audience is re-calculated, and the delivery is sent to the updated audience with the updated content. This can be a weekly newsletter or a recurring birthday email.

1. Select a delivery **Template**. Templates are pre-configured delivery settings specific to a channel. A built-in template is available for each channel and pre-filled by default. [Learn more](../../msg/delivery-template.md)

    ![Screenshot showing delivery activity in a workflow](../assets/delivery-activity-in-wf.png)
   
    Select the template from the channel activity configuration left pane. If the previously selected audience is not compatible with the channel, you cannot select a template. To solve this, update the **Build audience** activity to select an audience with the correct target mapping. Learn more about target mappings in [this section](../../audience/targeting-dimensions.md).

1. Click **Create delivery**. Define your message settings and content the same way you create a standalone delivery. Test and simulate the content. [Learn more](../../msg/gs-messages.md)

1. Navigate back to your workflow. To continue your workflow, toggle the **Generate an outbound transition** option to add a transition after the channel activity.

1. Click **Start** to launch your workflow.

    By default, starting a workflow triggers the message preparation stage without immediately sending the message.
    
1. Open your channel activity to confirm the sending from the **Review & send** button.

1. From your delivery dashboard, click **Send**.

## Examples {#cross-channel-workflow-sample}

Here is a cross-channel workflow example with segmentation and two deliveries. The workflow targets all customers who live in Paris and are interested in coffee machines. Among this population, an email is sent to regular customers, and an SMS is sent to VIP clients.

![Screenshot showing a cross-channel workflow example](../assets/workflow-channel-example.png)

You can also create a recurring workflow to send a personalized SMS every first day of the month at 8 PM to all customers living in Paris.

![Screenshot showing a recurring workflow example](../assets/workflow-channel-example2.png)

<!--
description, which use case you can perform (common other activities that you can link before or after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending of an email in a workflow. 
-->

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->