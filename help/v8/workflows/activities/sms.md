---
audience: end-user
title: Use the SMS workflow activity
description: Learn how to use the SMS workflow activity
badge: label="Alpha" type="Positive"
---

# SMS {#sms}

The **SMS** activity provides the functionality to send SMS messages within a workflow. It enables the automation of SMS sending to a specific target determined within the same workflow.

To define the recipients of the SMS, you can set them up before the SMS delivery activity in the workflow using the Build audience activity. Learn more.

1. After creating and configuring a new workflow, add a Build audience activity to select an existing audience or use the rule builder to define your own query.

1. Add an SMS channel activity into your workflow.

    ![](../assets/activity-sms-1.png)
<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the SMS to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the SMS to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the SMS to be sent at regular intervals.
-->

1. Select your activity. From the delivery menu, select the Templates you want to use for this delivery. Learn more about templates

1. Click Create delivery to configure your SMS delivery. For more information on SMS delivery, refer to this page.

1. Once your delivery is ready to be sent, navigate back to your workflow and click Start to launch your workflow.

1. By default, initiating a delivery workflow triggers the message preparation stage, without immediately sending the message.
    
    Click Review & send from the advanced menu of your SMS activity to confirm the sending.

1. From your SMS delivery dashboard, click Send.
