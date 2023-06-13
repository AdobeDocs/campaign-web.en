---
audience: end-user
title: Create a push notification delivery
description: Learn how to create a push notification delivery with Adobe Campaign Web
badge: label="Alpha" 
---
# Create a push notification delivery {#create-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Define the Push audience"
>abstract="Select the best audience for your Push message."

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Push Notification template"
>abstract="Select a push notification template to start your push delivery."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Push delivery properties"
>abstract="Manage the Push delivery properties."

1. From the **[!UICONTROL Deliveries]** homepage, click **[!UICONTROL Create delivery]**.

1. Under the **[!UICONTROL Channel]** section, choose Push notification as the channel and select a template depending on the chosen Operational system: Android or iOS. [Learn more about templates](../msg/delivery-template.md)

1. Click the **[!UICONTROL Create delivery]** button to confirm.

    ![](assets/push_create_1.png)

1. Enter a **[!UICONTROL Label]** for the delivery and access the **[!UICONTROL Additional options]** drop-down.

    +++Configure the following settings based on your requirements.
    * **[!UICONTROL Internal name]**: Assign a unique identifier to the delivery.
    * **[!UICONTROL Folder]**: Store the delivery in a specific folder.
    * **[!UICONTROL Delivery code]**: Organize your deliveries using your own naming convention.
    * **[!UICONTROL Description]**: Provide a description for the delivery.
    * **[!UICONTROL Nature]**: Specify the email's nature for classification purposes.
    +++

1. From the **[!UICONTROL Audience]** menu, select the application you want to use for this delivery.

1. Click the **[!UICONTROL Select audience]** button to target an existing audience or create your own. [Learn more](../audience/about-audiences.md)

    Note that, by default, your push notification will be sent to all subscribers of the application.

    ![](assets/push_create_2.png)

1. Switch on the **[!UICONTROL Enable control]** group option to set a control group to measure the impact of your delivery allowing you to compare the behavior of the population which received the message with the behavior of contacts which did not. [Learn more](../audience/control-group.md)

1. Click **[!UICONTROL Edit content]** to start designing the content of your  push notification.

1. To schedule your delivery to a specific date and time, switch on the **[!UICONTROL Enable scheduling]** option. After you initiate the delivery, the message will be automatically sent on the exact date and time that you have defined for the recipient.

    ![](assets/push_create_3.png)

1. Click **[!UICONTROL Configure delivery settings]** to access advanced options related to your delivery template. [Learn more](../advanced-settings/delivery-settings.md)

    ![](assets/push_create_4.png)
