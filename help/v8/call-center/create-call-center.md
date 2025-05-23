---
audience: end-user
title: Create a call center delivery
description: Learn how to create a call center delivery with Adobe Campaign Web
exl-id: fe8d4773-2271-46ec-9b2e-f50311a4ccf3
---
# Create and send a call center delivery {#create-call-center}

You can create a standalone call center delivery, or create one in the context of a campaign workflow. The steps below detail the procedure for a standalone (one-shot) delivery. If you are working in the context of a campaign workflow, creation steps are detailed in [this section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

To create and send a new standalone call center delivery, follow these main steps:

1. Create the delivery, [read more](#create-delivery)
1. Define the audience, [read more](#select-audience)
1. Edit the content, [read more](#edit-content)
1. Preview and send the delivery, [read more](#preview-send)

## Create the delivery{#create-delivery}

Follow these steps to create the delivery and configure its properties:

1. Select the **[!UICONTROL Deliveries]** menu and click the **[!UICONTROL Create delivery]** button.

1. Choose **[!UICONTROL Call center]** as the channel and click **[!UICONTROL Create delivery]** to confirm.

    ![Screenshot showing the creation of a call center delivery](assets/cc-create.png){zoomable="yes"}

    >[!NOTE]
    >
    >If you wish to select a different template, refer to this [page](../msg/delivery-template.md).

1. Under **[!UICONTROL Properties]**, enter a **[!UICONTROL Label]** for the delivery. Additional options are detailed in this [section](../email/create-email.md#create-email).

    ![Screenshot showing the properties configuration for a call center delivery](assets/cc-properties.png){zoomable="yes"}

>[!NOTE]
>
>You can schedule your delivery to be sent at a specific date. For more on this, refer to this [section](../msg/gs-deliveries.md#gs-schedule).

## Define the audience{#select-audience}

Now, you need to define the audience that will be targeted for the extraction file.

1. From the **[!UICONTROL Audience]** section of the delivery page, click **[!UICONTROL Select audience]**.

    ![Screenshot showing audience selection for a call center delivery](assets/cc-audience.png){zoomable="yes"}

1. Choose an existing audience or create your own.

    * [Learn how to select an existing audience](../audience/add-audience.md)
    * [Learn how to create a new audience](../audience/one-time-audience.md)

    ![Screenshot showing audience selection for a call center delivery](assets/cc-audience2.png){zoomable="yes"}

>[!NOTE]
>
>Call center recipients must contain at least their names and telephone number. Any recipients with incomplete information will be excluded from call center deliveries.
>
>To learn how to configure control groups, refer to this [page](../audience/control-group.md).

## Edit the content{#edit-content}

Now, let's edit the content of the extraction file that will be generated by the call center delivery. 

1. From the delivery page, click the **[!UICONTROL Edit content]** button.

    ![Screenshot showing content editing for a call center delivery](assets/cc-content0.png){zoomable="yes"}

1. Specify the **[!UICONTROL File name]**. To learn how to personalize the file name, refer to this [page](../personalization/personalize.md).

1. Select a **[!UICONTROL File format]**: **Text**, **Text using fixed-width columns**, **CSV (Excel)**, or **XML**.

    ![Screenshot showing content editing for a call center delivery](assets/cc-content.png){zoomable="yes"}

    >[!NOTE]
    >
    >Extraction format options are detailed in this [page](../direct-mail/content-direct-mail.md#properties).

1. Toggle on the **[!UICONTROL Requested quantity]** option if you cant to restrict the number of recipients for your delivery.

1. In the **[!UICONTROL Content]** section, click the **[!UICONTROL Add Attribute]** button to create a new column to display in the extraction file.

1. Choose the attribute to display in the column, then confirm. To learn more on how to select attributes and add them to favorites, refer to this [page](../get-started/attributes.md).

    ![Screenshot showing the Add Attribute button and options for adding attributes to the extraction file.](assets/cc-add-attribute.png)

1. Repeat these steps to add as many columns as needed for your extraction file.

    You can then edit the attributes, sort the extraction file, or change the position of the columns. For more on this, refer to this [page](../direct-mail/content-direct-mail.md#content).

    ![Screenshot showing the attributes configuration options for the extraction file.](assets/cc-content-attributes.png)

## Preview and send the delivery{#preview-send}

When the delivery content is ready, you can preview it using test profiles and send proofs. You can then send the call center delivery to generate the extraction file.

The main steps to preview and send the extraction file are as follows. More details are available in [this page](../direct-mail/send-direct-mail.md).

1. From the delivery content page, click the **[!UICONTROL Simulate content]** button.

    ![Screenshot showing the simulate content option in the delivery content page](assets/cc-simulate0.png){zoomable="yes"}

1. Select one or several test profiles to preview the personalized content. You can also send proofs. [Read more](../direct-mail/send-direct-mail.md#preview-dm)

    ![Screenshot showing the simulate content option in the delivery content page](assets/cc-simulate.png){zoomable="yes"}

1. From the delivery page, click **[!UICONTROL Review & send]**.

    ![Screenshot showing the review and send option in the delivery page](assets/cc-review-send.png){zoomable="yes"}

1. Click **[!UICONTROL Prepare]** and monitor the progress and statistics provided, then confirm.

    ![Screenshot showing the prepare option and logs menu](assets/cc-prepare.png){zoomable="yes"}

1. Click **[!UICONTROL Send]** to proceed with the final sending process, then confirm.

Once your delivery is sent, the extraction file is automatically generated and exported to the location specified in the **[!UICONTROL Routing]** external account selected in the delivery template's [advanced settings](../advanced-settings/delivery-settings.md). You can also preview the file by clicking the **Preview file** button, in the **Content** section of the screen. 

Track your KPIs (Key Performance Indicator) data from your delivery page and data from the **[!UICONTROL Logs]** menu.

Start measuring the impact of your message with built-in reports. [Learn more](../reporting/direct-mail.md)
