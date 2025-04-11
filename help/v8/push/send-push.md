---
audience: end-user
title: Send a push notification delivery
description: Learn how to send a push notification delivery with Adobe Campaign Web
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
---
# Preview and send a push delivery {#send-push-delivery}

## Preview your push notification delivery {#preview-push}

Once you define your message content, use test subscribers to preview and test the message. If personalized content is included, examine how this content is displayed in the message by using test profile data. This ensures the message is rendered correctly and personalized elements are appropriately incorporated.

The main steps to preview your push notification are as follows. More details on how to preview deliveries are available in [this section](../preview-test/preview-content.md).

1. From your delivery content page, use **[!UICONTROL Simulate content]** to preview your personalized content.

    ![Previewing personalized content in the delivery content page](assets/push_send_1.png){zoomable="yes"}

1. Click **[!UICONTROL Add subscribers(s)]** to select one or several profiles to preview their data in the push notification content.

    <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. In the right pane, find a preview of the push notification, where personalized elements are dynamically replaced with data from the selected profile.

    ![Preview pane showing personalized elements replaced with profile data](assets/push_send_7.png){zoomable="yes"}

Review and send your push notification to your audience.

## Test your push notification delivery {#test-push}

Using **Adobe Campaign**, send proofs before delivering them to your main audience. This step validates your delivery and identifies any issues.

Test profiles act as proof recipients. They review and validate components and settings such as links, images, and personalization, ensuring optimal performance and detecting errors. This process refines and optimizes your push notifications before reaching your main audience. [Learn how to send proofs](../preview-test/test-deliveries.md#subscribers).

![Testing push notification delivery with proof recipients](assets/push_send_6.png){zoomable="yes"}

## Send your push notification delivery {#send-push}

1. After personalizing your push notification content, click **[!UICONTROL Review & send]** from your **[!UICONTROL Delivery]** page.

    ![Review and send button on the delivery page](assets/push_send_2.png){zoomable="yes"}

1. Click **[!UICONTROL Prepare]** and monitor the progress and statistics provided. 

    If errors occur, refer to the Logs menu for detailed information about the failure.

    ![Monitoring preparation progress and statistics](assets/push_send_3.png){zoomable="yes"}

1. Send the messages by clicking **[!UICONTROL Send]** to proceed with the final sending process. 

1. Confirm the send action by clicking **[!UICONTROL Send]**. 

    If the push delivery is scheduled, click the **[!UICONTROL Send as scheduled]** button. Learn more about delivery scheduling in [this section](../msg/gs-messages.md#schedule-the-delivery-sending).

    ![Send as scheduled button for scheduled push delivery](assets/push_send_4.png){zoomable="yes"}

Once your delivery is sent, track your Key Performance Indicator (KPI) data from your delivery page and data from the **[!UICONTROL Logs]** menu.

Start measuring the impact of your message with built-in reports. [Learn more](../reporting/push-report.md).