---
audience: end-user
title: Prepare and send an email
description: Campaign v8 Web documentation
---
# Prepare and send your email {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Prepare and send your email"
>abstract="Discover how to prepare your email and learn more about sending KPIs."

>[!NOTE]
>
>This documentation is under construction and frequently updated. The final version of this content will be ready in January 2023.

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Prepare the send

During the preparation, the target population is calcultated and the message content generated for each profile included in the target. Once the preparation is finished, the messages are ready to be sent, either immediately or at the scheduled date and time. The validation rules used during analysis are described in this [section](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. Click the **Prepare** button located in the top right corner.

1. The preparation progress is displayed. Depending on the size of the targeted population, this operation may take some time.

    >[!NOTE]
    >
    >You can stop the preparation at any time using the **Stop preparation** button. During the preparation phase, no messages are sent. You can therefore start or stop this without risk of impacting anything.

1. When the preparation is finished, check the **Targeted**, **To deliver** and **To exclude** KPIs. If the number of messages to send does not match your expectations, modify your audience and restart the preparation.

1. Click the **Logs** button and check that there is no error. All the validation steps, warnings and errors are listed. Colored icons show the message type:

    * The grey icon indicates an informative message.
    * The yellow icon indicates a non-critical processing error.
    * The red icon indicates a critical error that prevents sending the delivery. 

1. After making the changes, restart the preparation.

Once the preparation has been completed, your message is ready to be sent. For more on this, see Confirming send.


## Send the message

Once the preparation is complete, follow the steps below to send your message.

1. Click the **Send button** in the top right corner and confirm. 

1. The sending progress is displayed alongside with three KPIs: Delivered, Opens, Clicks.

1. Finalize the send by clicking the OK button.

LOGS

>[!NOTE]
>
>If the message is scheduled, it is sent when sending time is reached. For more on scheduling messages, refer to this section.

