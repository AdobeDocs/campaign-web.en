---
audience: end-user
title: Create a push notification delivery
description: Learn how to create a push notification delivery with Adobe Campaign Web
badge: label="Beta" 
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

You can create a standalone push notification delivery, or create a push notification in the context of a campaign workflow. The steps below detail the procedure for a standalone (one-shot) push delivery. If you are working in the context of a campaign workflow, creation steps are details in [this section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


To create a new standalone push delivery, follow these steps:

1. Browse to the **[!UICONTROL Deliveries]** menu on the left rail, and click the  **[!UICONTROL Create delivery]** button.

1. Under the **[!UICONTROL Channel]** section, choose **Push notification** as the channel and select a template, depending on the chosen device operational system: Android or iOS. [Learn more about templates](../msg/delivery-template.md)

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

1. Click the **[!UICONTROL Select audience]** button to target an existing audience or create your own. [Learn more](../audience/about-recipients.md)

    Note that, by default, your push notification will be sent to all subscribers of the application.

    ![](assets/push_create_2.png)

1. Switch on the **[!UICONTROL Enable control]** group option to set a control group to measure the impact of your delivery allowing you to compare the behavior of the population which received the message with the behavior of contacts which did not. [Learn more](../audience/control-group.md)

1. Click **[!UICONTROL Edit content]** to start designing the content of your  push notification. [Learn more](content-push.md)

    ![](assets/push_create_5.png)

    From this screen, you can also [simulate your content](../preview-test/preview-test.md) and [set up offers](../content/offers.md).

1. To schedule your delivery to a specific date and time, switch on the **[!UICONTROL Enable scheduling]** option. After you initiate the delivery, the message will be automatically sent on the exact date and time that you have defined for the recipient. Learn more about delivery scheduling in [this section](../msg/gs-messages.md#gs-schedule)

    ![](assets/push_create_3.png)

1. Click **[!UICONTROL Configure delivery settings]** to access advanced options related to your delivery template. [Learn more](../advanced-settings/delivery-settings.md)

    ![](assets/push_create_4.png)
