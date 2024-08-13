---
audience: end-user
title: Create a push notification delivery
description: Learn how to create a push notification delivery with Adobe Campaign Web
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
---
# Create a push notification delivery {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Push Notification template"
>abstract="Select a push notification template to start your push delivery. Delivery templates allow you to easily reuse custom content and settings across your campaigns and deliveries."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html" text="Use delivery templates"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Push delivery properties"
>abstract="Define your Push delivery properties. Enter the label of the push and use the **Additional Options** to configure the internal name, delivery folder and code. You can also enter a custom description."

You can create a standalone push notification delivery, or create a push notification in the context of a campaign workflow. The steps below detail the procedure for a standalone (one-shot) push delivery. If you are working in the context of a campaign workflow, creation steps are details in [this section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Create a push delivery {#create-push-delivery}

To create a new standalone push delivery, follow these steps:

1. Browse to the **[!UICONTROL Deliveries]** menu on the left rail, and click the  **[!UICONTROL Create delivery]** button.

1. Under the **[!UICONTROL Channel]** section, choose **Push notification** as the channel, and select a template, depending on the chosen device operation system: Android or iOS. [Learn more about templates](../msg/delivery-template.md)

1. Click the **[!UICONTROL Create delivery]** button to confirm.

    ![](assets/push_create_1.png){zoomable="yes"}

## Configure the delivery settings {#configure-push-settings}

Configure your delivery settings as detailed below:

1. Enter a **[!UICONTROL Label]** for the delivery. By default, the label is set with the label of the selected template. It should be updated.

1. Browse the **[!UICONTROL Additional options]** drop-down to customize the options, if needed. If your delivery is based on an extended schema, specific **Custom options** fields are available.

    +++Configure the following settings based on your requirements.
    * **[!UICONTROL Internal name]**: Assign a unique identifier to the delivery.
    * **[!UICONTROL Folder]**: Store the delivery in a specific folder.
    * **[!UICONTROL Delivery code]**: Organize your deliveries using your own naming convention.
    * **[!UICONTROL Description]**: Provide a description for the delivery.
    * **[!UICONTROL Nature]**: Specify the delivery's nature for classification purposes.
    +++


## Select your push delivery audience {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Define the push notification audience"
>abstract="To define the audience of your message, you must first select the app associated to the Push delivery. By default, your push notification is sent to all subscribers of the application. You can refine to a specific audience by clicking the **Select audience** button. If needed, add a control group to measure the impact of your delivery."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Set a control group"


You must first select the app, and then you can refine the Push notification audience, as detailed below:

1. From the **[!UICONTROL Audience]** section, select the application you want to use for this delivery. By default, your push notification is sent to all subscribers of the application. You can refine to a specific audience by clicking the **[!UICONTROL Select audience]** button.

    ![](assets/push_create_2.png){zoomable="yes"}

1. Select an existing audience, or create your own audience, to refine the target population for your Push delivery. For Push notification, the default [target dimension](../audience/about-recipients.md#targeting-dimensions) is **Subscriber application** (nms:appSubscriptionRcp), which is linked to the recipients table. 

    Learn how to select an existing audience in [this page](../audience/add-audience.md)

    Learn how to create a new audience in [this page](../audience/one-time-audience.md)

1. Switch on the **[!UICONTROL Enable control group]** option to set a control group to measure the impact of your delivery. Messages are not sent to that control group, so that you can compare the behavior of the population which received the message with the behavior of contacts which did not. [Learn more](../audience/control-group.md)

## Define the Push notification content {#create-content-push}

To define the content of your notification, click **[!UICONTROL Edit content]**. [Learn more](content-push.md)

![](assets/push_create_5.png){zoomable="yes"}

From this screen, you can also [simulate your content](../preview-test/preview-test.md) and [set up offers](../msg/offers.md).

## Schedule your delivery sending {#schedule-push}

When a delivery is sent in the context of a workflow, you must use the **Scheduler** activity. Learn more in [this page](../workflows/activities/scheduler.md). Steps below only apply to standalone deliveries.

To schedule a standalone push delivery to a specific date and time, follow these steps:

1. Browse to the **[!UICONTROL Schedule]** section of the delivery properties.

1. Use the **[!UICONTROL Enable scheduling]** toggle to activate it.

1. Set the desired date and time for sending.

After you initiate the delivery, the message is automatically sent on the exact date and time that you have defined for the recipient. 

![](assets/push_create_3.png){zoomable="yes"}

Learn more about delivery scheduling in [this section](../msg/gs-deliveries.md#gs-schedule)

## Delivery advanced settings {#adv-push}

Click **[!UICONTROL Configure delivery settings]** to access advanced options related to your delivery template. [Learn more](../advanced-settings/delivery-settings.md)

![](assets/push_create_4.png){zoomable="yes"}
