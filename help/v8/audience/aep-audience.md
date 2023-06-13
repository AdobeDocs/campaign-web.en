---
audience: end-user
title: Use an Adobe Experience Platform audience
description: Learn how to use an audience from Adobe Experience Platform
badge: label="Alpha" type="Positive"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
---
# Use an Adobe Experience Platform audience{#aep-audience}

The Adobe Campaign Managed Cloud Service Destination and Source connectors allow seamless integration between Adobe Campaign and Adobe Experience Platform.

Once you have created an Adobe Experience Platform audience and it is available in the client console, you can use it in the same way as you would for a Campaign audience to personalize and send messages.

>[!NOTE]
>
>To use Adobe Experience Platform audiences in Campaign, you need to configure the integration with Adobe Sources and Destinations. Refer to [Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.


You can also:

* Build a new audience. [Learn more](segment-builder.md)
* Load an audience from an external file. [Learn more](file-audience.md)
* Use an existing Campaign audience. [Learn more](add-audience.md).

To select an Adobe Experience Platform audience for your message, follow the steps below:

1. From the **Audience** section of the delivery creation assistant, click the **[!UICONTROL Select audience]** button.

   ![](assets/create-audience.png)

1. Choose **[!UICONTROL Select audience]** to use an existing audience. To create a new audience to be used in this email, choose **Create your own**. Refer to this [section](segment-builder.md).

    This screen displays all existing audiences defined in the Adobe Campaign client console, for the current folder. To choose an audience from Adobe Experience Platform, browse to the `AEP Audiences folder` from the filter section of the screen.

    ![](assets/select-audience-folder.png)

    You can also define a rule to filter on the origin of the audiences, as below:

    ![](assets/filter-on-aep-audience.png)

1. Choose an audience and click **Select**.

1. Click **Edit rules** if you want to refine your audience.

   ![](assets/refine-audience.png)

1. Using the rule builder, you can enrich your audience with additional filters or by combining different audiences. See this [section](segment-builder.md).

1. Click **Save**. 

You can also set a control group to measure the impact of your campaigns. The control group do not receive the message. This allows you to compare the behavior of the population which received the message with the behavior of contacts which did not. See [section](control-group.md).

