---
audience: end-user
title: Use the Push notification workflow activity
description: Learn how to use the Push notification workflow activity
badge: label="Beta" 
---

# Push notification {#push-activity}

The **Push notification** delivery activity allows you to configure the sending a push notification in a workflow.

>[!BEGINTABS]

>[!TAB Push notification (Android)]

1. After creating and configuring a new workflow, add a Build audience activity to select an existing audience or use the rule builder to define your own query.

1. Add a Push notification (Android) channel activity into your workflow.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Select your activity. From the delivery menu, select the Templates you want to use for this delivery. Learn more about templates

1. Click Create delivery to configure your push notification delivery. For more information on Push notification (Android) delivery, refer to this page.

1. Once your delivery is ready to be sent, navigate back to your workflow and click Start to launch your workflow.

1. By default, initiating a delivery workflow triggers the message preparation stage, without immediately sending the message.
    
    Click Review & send from the advanced menu of your Push notification (Android) channel activity to confirm the sending.

1. From your Push notification delivery dashboard, click Send.

>[!TAB Push notification (iOS)]

1. After creating and configuring a new workflow, add a Build audience activity to select an existing audience or use the rule builder to define your own query.

1. Add a Push notification (iOS) channel activity into your workflow.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Select your activity. From the delivery menu, select the Templates you want to use for this delivery. Learn more about templates

1. Click Create delivery to configure your push notification delivery. For more information on Push notification (iOS) delivery, refer to this page.

1. Once your delivery is ready to be sent, navigate back to your workflow and click Start to launch your workflow.

1. By default, initiating a delivery workflow triggers the message preparation stage, without immediately sending the message.
    
    Click Review & send from the advanced menu of your Push notification (iOS) channel activity to confirm the sending.

1. From your Push notification delivery dashboard, click Send.

>[!ENDTABS]