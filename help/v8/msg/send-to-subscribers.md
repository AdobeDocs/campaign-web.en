---
audience: end-user
title: Send messages to the subscribers of a service
description: Learn how to send messages to the subscribers of a service
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
---
# Send messages to the subscribers of a service {#send-to-subscribers}

You can create subscription services in Adobe Campaign, and send messages to your subscribers. Learn how to create subscription services on [this page](../audience//manage-services.md#create-service).

To send messages to your subscribers, create a specific audience to identify the subscribers, and then create the delivery as detailed below.

1. Create an audience. A new workflow is automatically created. [Learn more about audiences](../audience/create-audience.md).

1. For better readability, change the name of the workflow in the workflow settings' **Label** field. [Learn how to configure workflow settings](../workflows/workflow-settings.md).

1. Open the **[!UICONTROL Build audience]** activity, and select **[!UICONTROL Create audience]**. [Learn how to configure a Build audience activity](../workflows/activities/build-audience.md).

    ![Screenshot showing the Build audience activity configuration in Adobe Campaign.](assets/service-create-audience.png){zoomable="yes"}

1. In the audience creation flow, select the following custom conditions: **[!UICONTROL Subscriptions]** exist, such as **[!UICONTROL Service]** is equal to the service you defined. In this example, select your **Luma yoga newsletter**.

    ![Screenshot showing the audience creation flow with custom conditions for subscriptions in Adobe Campaign.](assets/service-audience-subscribers.png){zoomable="yes"}

1. Select **[!UICONTROL Confirm]**, and click **[!UICONTROL Start]** to execute the workflow.

1. Create a delivery. Steps to create a delivery are detailed on [this page](../msg/gs-messages.md#create-delivery).

1. Browse to your delivery settings, and change the default target mapping to **Subscriptions (nms:subscriptions)**.

    ![Screenshot showing the delivery settings with the target mapping changed to Subscriptions in Adobe Campaign.](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. In the main target section of the delivery, select the audience that you created above.

    ![Screenshot showing the main target section of the delivery with the selected audience in Adobe Campaign.](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. Create your message content, test it, and send the delivery, as detailed in [this section](../preview-test/preview-test.md).

    ![Screenshot showing the delivery ready to be sent in Adobe Campaign.](assets/service-delivery-ready.png){zoomable="yes"}

Your delivery is sent to the subscribers of that service only.