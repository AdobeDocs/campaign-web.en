---
audience: end-user
title: Create a SMS delivery
description: Learn how to create and send SMS with Adobe Campaign Web
badge: label="Beta" 
exl-id: 89c9da76-1e04-41cd-9636-0d3b957875b6
---
# Create an SMS delivery {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="SMS delivery properties"
>abstract="The properties encompass the common delivery parameters that assist you in both naming and classifying your delivery. If your delivery is based on an extended schema, specific Custom options fields are available."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Define the SMS audience"
>abstract="Select the best audience for your SMS message."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="SMS template selection"
>abstract="Select a predefined template to start your SMS delivery."

You can create a standalone SMS delivery, or create a SMS in the context of a campaign workflow. The steps below detail the procedure for a standalone (one-shot) SMS delivery. If you are working in the context of a campaign workflow, creation steps are details in [this section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


To create a new standalone SMS delivery, follow these steps:

1. Browse to the **[!UICONTROL Deliveries]** menu on the left rail, and click the  **[!UICONTROL Create delivery]** button.

1. Under the **[!UICONTROL Channel]** section, choose SMS as the channel and select a template. [Learn more about templates](../msg/delivery-template.md)

1. Click the **[!UICONTROL Create delivery]** button to confirm.

    ![](assets/sms_create_1.png)

1. Enter a **[!UICONTROL Label]** for the delivery and access the **[!UICONTROL Additional options]** drop-down.

    +++Configure the following settings based on your requirements.
    * **[!UICONTROL Internal name]**: Assign a unique identifier to the delivery.
    * **[!UICONTROL Folder]**: Store the delivery in a specific folder.
    * **[!UICONTROL Delivery code]**: Organize your deliveries using your own naming convention.
    * **[!UICONTROL Description]**: Provide a description for the delivery.
    * **[!UICONTROL Nature]**: Specify the email's nature for classification purposes.
    +++

1. Click the **[!UICONTROL Select audience]** button to target an existing audience or create your own. [Learn more](../audience/about-recipients.md).

    ![](assets/sms_create_2.png)

1. Switch on the **[!UICONTROL Enable control]** group option to set a control group to measure the impact of your delivery allowing you to compare the behavior of the population which received the message with the behavior of contacts which did not. [Learn more](../audience/control-group.md)

1. Click **[!UICONTROL Edit content]** to start designing the content of your SMS message. [Learn more](content-sms.md)

    ![](assets/sms_create_4.png)

    From this screen, you can also [simulate your content](../preview-test/preview-test.md) and [set up offers](../content/offers.md).

1. To schedule your delivery to a specific date and time, switch on the **[!UICONTROL Enable scheduling]** option. After you initiate the delivery, the message will be automatically sent on the exact date and time that you have defined for the recipient. Learn more about delivery scheduling in [this section](../msg/gs-messages.md#gs-schedule).

1. Click **[!UICONTROL Configure delivery settings]** to access advanced options related to your delivery template. [Learn more](../advanced-settings/delivery-settings.md)

    ![](assets/sms_create_3.png)
