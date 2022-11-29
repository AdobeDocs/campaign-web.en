---
audience: end-user
title: Prepare and send an email
description: Campaign v8 Web documentation
---
# Prepare and send your email {#prepare-send}


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

During preparation, the target population is calcultated and the message content generated for each profile included in the target. Once the preparation is finished, the messages are ready to be sent, either immediately or at the scheduled date and time.

1. To start preparing the send, click the **Prepare** button located in the top right corner.

1. The preparation progress is displayed alongside with three KPIs: number of targeted messages, number of messages to send, etc.

1. Depending on the size of the targeted population, this operation may take some time.



Stop the preparation at any time using the Stop button, located in the action bar.

During the preparation phase, no messages are sent. You can therefore start or stop this without risk of impacting anything.



Your message is automatically saved during the preparing for delivery stage. If you need to make any changes to your message’s schedule after the preparation step, you will need to make sure that you click the Prepare button again for those changes to be taken into account. For more information on how to schedule a message, refer to this page.



To view the preparation logs, click the button located in the bottom right of the block.



The Deployment window opens, correct any errors then restart the preparation.

The last log message displays any error messages and the number of errors. A specific icon shows the encountered error type: the yellow icon indicates a non-critical processing error, the red icon indicates a critical error that prevents the delivery from being started.



Check the preparation statistics before confirming sending the messages. If the number of messages to send does not correspond to your configuration, edit the targeted population (see Selecting an audience in a message) and restart the preparation.

Once the preparation has been completed, your message is ready to be sent. For more on this, see Confirming send.

Typology rules

Adobe Campaign comes with a set of build-in typology rules that are applied during the message preparation. They are used to check whether a message is valid and meets your quality criteria. See Typologies. You can define your own typology rules, for example, can set global cross-channel fatigue rules that will automatically exclude oversollicited profiles from campaigns. See Fatigue rules.

Confirming the send
Once you have finished preparing your messages and the approval steps have been carried out, you can send them. For more on messages preparation, refer to Preparing the send.

Only users with the Start deliveries role can confirm sending. For more on this, refer to the List of roles section.

## Send the message

Once preparation is complete, follow the steps below to send your message.

Click the Confirm send button found in the message’s action bar.



Finalize the send by clicking the OK button.



Wait while the message is being sent. The Deployment block shows the progress of the send.

NOTE
If the message is scheduled, it is sent when sending time is reached. For more on scheduling messages, refer to this section.

If you are using a recurring delivery with no aggregation period, you can request confirmation before the delivery is sent. When configuring your message, open the Schedule block of the delivery dashboard and activate the dedicated option.





preparation:

This operation calcultates the target population and generates the message contents for each profile included in the target. Once preparation is finished, the messages are ready to be sent, either immediately or at the scheduled date and time. Learn how to prepare and send an email


Depending on the size of the targeted population, this operation may take some time.

>[!NOTE]
>
>You can stop the preparation at any time using the **Stop preparation** button. During the preparation phase, no messages are sent. You can therefore start or stop this without risk of impacting anything. 
>
>Your message is automatically saved during the preparing for delivery stage. If you need to make any changes to your message's schedule after the preparation step, you will need to make sure that you click the **[!UICONTROL Prepare]** button again for those changes to be taken into account.
