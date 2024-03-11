---
audience: end-user
title: Preview & send a direct mail delivery
description: Learn how to preview & send a direct mail delivery with Adobe Campaign Web
---

# Preview & send a direct mail delivery {#send-direct-mail}

## Preview your direct mail delivery {#preview-dm}

Once you have configured the extraction file for your direct mail delivery, you can utilize test profiles to preview and test it. If you have included personalized content, you can examine how this content is displayed in the columns by using test profile data. This allows you to ensure that the file content is being rendered correctly and that the personalized elements are being appropriately incorporated.

The main steps to preview your extraction file are as follows. More details on how to preview deliveries are available in [this section](../preview-test/preview-content.md).

1. From your delivery content page, use **[!UICONTROL Simulate content]** to preview your personalized content.

    ![](assets/dm-simulate.png){zoomable="yes"}

1. Click **[!UICONTROL Add test profile(s)]** to select one or several profiles to preview their data in the extraction file content.

1. In the right pane, you will find a preview of the extraction file, where personalized elements are dynamically replaced with data from the selected profile.

    ![](assets/dm-preview-right.png){zoomable="yes"}

## Test your direct mail delivery {#test-push}

Using **Adobe Campaign**, you have the ability to send proofs before sending them to your main audience. This step is important in validating your delivery and identifying any issues. 

Test recipients can review elements such as personalization settings, ensuring optimal performance and detecting any errors. This process helps you refine and optimize your extraction file before reaching your main audience. [Learn how to send proofs](../preview-test/test-deliveries.md#subscribers)

![](assets/dm-preview-proof.png){zoomable="yes"}

## Send your direct mail delivery {#send-push}

1. After designing the content of your extraction file, click **[!UICONTROL Review & send]** from your **[!UICONTROL Delivery]** page.

    ![](assets/dm-review-send.png){zoomable="yes"}

1. Click **[!UICONTROL Prepare]** and monitor the progress and statistics provided. 

    If any errors occur, refer to the **[!UICONTROL Logs]** menu for detailed information about the failure.

    ![](assets/dm-prepare.png){zoomable="yes"}

1. Send the messages by clicking on **[!UICONTROL Send]** to proceed with the final sending process. 

1. Confirm the send action by clicking the **[!UICONTROL Send]**. 

    If the direct mail delivery has been scheduled, click the **[!UICONTROL Send as scheduled]** button. Learn more about delivery scheduling in [this section](../msg/gs-messages.md#schedule-the-delivery-sending).

Once your delivery is sent, the extraction file is automatically generated and exported to the server specified in your file routing configuration.

You can track your KPIs (Key Performance Indicator) data from your delivery page and data from the **[!UICONTROL Logs]** menu.

<!-- Released later on ? to check when : You can also start measuring the impact of your message with built-in reports. [Learn more](../reporting/push-report.md)-->
