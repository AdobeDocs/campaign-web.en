---
audience: end-user
title: Validate transactional messages
description: Learn how to validate a transactional message in Campaign Web User Interface
exl-id: 4a24792f-b9f4-4224-b3a8-75f6969b64da
---
# Validate transactional messages

During or after creating your transactional message, you may want to validate the content using a data sample.

## Simulate content {#simulate-content}

Follow these steps to simulate the content of your message:

* Ensure that the personalization path in your message content matches your context sample. In the example below, to display the first name of the test profile, use the path *rtEvent.ctx.basicDetails.firstName*. 

    You can modify the message content or the context sample to make them align.

    ![Screenshot showing the verification of personalization paths in the message content](assets/validate-verification.png){zoomable="yes"}

* Click on the **[!UICONTROL Simulate content]** button to preview your transactional message with the data entered in the context sample.

    ![Screenshot showing the Simulate content button and preview functionality](assets/validate-simulate.png){zoomable="yes"}

    After reviewing your content, click on the **[!UICONTROL Close]** button.

* Ensure you click the **[!UICONTROL Republish]** button if you have made any changes to your content.

## Send proof

To test and experience the transactional message as it would be delivered through your chosen channel, such as email, SMS, or push notification, use the proof feature.

In the [simulation content window](#simulate-content), click on the **[!UICONTROL Send proof]** button.

![Screenshot showing the Send proof button in the simulation content window](assets/transactional-proof.png){zoomable="yes"}

In the new window that appears, enter the email address or phone number, depending on the channel, where you would like to receive the proof. After entering the desired address, click on the **[!UICONTROL Send proof]** and **[!UICONTROL Confirm]** buttons. This action sends a sample of your transactional message, ensuring that all personalizations, dynamic content, and formatting appear correctly as they would for your end users.

![Screenshot showing the Send proof functionality and confirmation process](assets/transactional-sendproof.png){zoomable="yes"}

This step is essential for identifying any potential issues before publishing your transactional message.