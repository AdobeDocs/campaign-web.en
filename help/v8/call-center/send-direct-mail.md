---
audience: end-user
title: Preview & send a direct mail delivery
description: Learn how to preview & send a direct mail delivery with Adobe Campaign Web
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
---
# Preview & send a direct mail delivery {#send-direct-mail}

Once you configure the extraction file for your direct mail delivery, use test profiles to preview it. If personalized content is included, examine how this content appears in the columns using test profile data. This ensures the file content is rendered correctly and personalized elements are appropriately incorporated.

When the extraction file is ready, send the direct mail delivery to generate the file and share it with your direct mail provider. [Learn how to send your direct mail delivery](#dm-send)

## Preview the extraction file {#preview-dm}

The main steps to preview your extraction file are as follows. More details on how to preview deliveries are available in [this section](../preview-test/preview-content.md).

1. From your delivery content page, use **[!UICONTROL Simulate content]** to preview your personalized content.

    ![Screenshot showing the simulate content option in the delivery content page](assets/dm-simulate.png){zoomable="yes"}

1. Click **[!UICONTROL Add test profile(s)]** to select one or several profiles and preview their data in the extraction file content.

1. In the right pane, view a preview of the extraction file, where personalized elements are dynamically replaced with data from the selected profile.

    ![Screenshot showing the preview of the extraction file in the right pane](assets/dm-preview-right.png){zoomable="yes"}

## Send proofs {#test-dm}

Using **Adobe Campaign**, send proofs before delivering them to your main audience. This step validates your delivery and identifies any issues. Test recipients review elements such as personalization settings, ensuring optimal performance and detecting errors. This process refines and optimizes your extraction file before reaching your main audience.

For direct mail deliveries, sending proofs generates a sample of the extraction file using data from the selected test profiles. To access it, follow these steps:

1. From the simulate content screen, click the **[!UICONTROL Send proof]** button and follow the same steps as for any type of delivery to send a proof. [Learn how to send proofs](../preview-test/test-deliveries.md)

1. Once the proof is sent, access it from the **[!UICONTROL View proofs]** button or from the deliveries list. [Learn how to access sent proofs](../preview-test/test-deliveries.md#access-test-deliveries)

1. In the proof delivery dashboard, click the **[!UICONTROL Preview file]** button to access a preview of the extraction file.

    ![Screenshot showing the preview file option in the proof delivery dashboard](assets/dm-proof.png){zoomable="yes"}

    >[!NOTE]
    >
    >Only the first 100 lines are displayed in the preview file.

## Send your direct mail delivery {#send-dm}

Once your direct mail is ready to be sent to your customers, send the delivery to start the data extraction in the specified extraction file. To do this, follow these steps:

1. After designing the content of your extraction file, click **[!UICONTROL Review & send]** from your **[!UICONTROL Delivery]** page.

    ![Screenshot showing the review and send option in the delivery page](assets/dm-review-send.png){zoomable="yes"}

1. Click **[!UICONTROL Prepare]** and monitor the progress and statistics provided. 

    If any errors occur, refer to the **[!UICONTROL Logs]** menu for detailed information about the failure.

    ![Screenshot showing the prepare option and logs menu](assets/dm-prepare.png){zoomable="yes"}

1. Send the messages by clicking **[!UICONTROL Send]** to proceed with the final sending process. 

1. Confirm the send action by clicking **[!UICONTROL Send]**. 

    If the direct mail delivery is scheduled, click the **[!UICONTROL Send as scheduled]** button. Learn more about delivery scheduling in [this section](../msg/gs-messages.md#schedule-the-delivery-sending).

Once your delivery is sent, the extraction file is automatically generated and exported to the location specified in the **[!UICONTROL Routing]** external account selected in the delivery template's [advanced settings](../advanced-settings/delivery-settings.md).

Track your KPIs (Key Performance Indicator) data from your delivery page and data from the **[!UICONTROL Logs]** menu.

Start measuring the impact of your message with built-in reports. [Learn more](../reporting/direct-mail.md)