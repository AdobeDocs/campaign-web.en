---
audience: end-user
title: Create a SMS delivery
description: Learn how to create and send SMS with Adobe Campaign Web
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
---
# Create an SMS delivery {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="SMS delivery properties"
>abstract="The properties include the common delivery parameters that help you name and classify your delivery. If your delivery uses an extended schema, specific Custom options fields are available."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Define the SMS audience"
>abstract="Create a new audience or select an existing one by clicking the **Select audience** button. If needed, add a control group to measure the impact of your delivery."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Set a control group"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="SMS template selection"
>abstract="Select a predefined template to start your SMS delivery. Delivery templates allow you to reuse custom content and settings across your campaigns and deliveries."

You can create a standalone SMS delivery, or create an SMS in the context of a campaign workflow. The steps below explain the procedure for a standalone (one-shot) SMS delivery. If you are working in the context of a campaign workflow, creation steps are explained in [this section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

To create a new standalone SMS delivery, follow these steps:

1. Browse to the **[!UICONTROL Deliveries]** menu on the left rail, and click the **[!UICONTROL Create delivery]** button.

1. Under the **[!UICONTROL Channel]** section, choose SMS as the channel, and select a template. [Learn more about templates](../msg/delivery-template.md)

1. Click the **[!UICONTROL Create delivery]** button to confirm.

    ![Screenshot showing the Create delivery button and SMS channel selection](assets/sms_create_1.png){zoomable="yes"}

1. Enter a **[!UICONTROL Label]** for the delivery and access the **[!UICONTROL Additional options]** drop-down. If your delivery uses an extended schema, specific **Custom options** fields are available.

    +++Configure the following settings based on your requirements.
    * **[!UICONTROL Internal name]**: Assign a unique identifier to the delivery.
    * **[!UICONTROL Folder]**: Store the delivery in a specific folder.
    * **[!UICONTROL Delivery code]**: Organize your deliveries using your own naming convention.
    * **[!UICONTROL Description]**: Provide a description for the delivery.
    * **[!UICONTROL Nature]**: Specify the delivery's nature for classification purposes.
    +++

1. Click the **[!UICONTROL Select audience]** button to target an existing audience or create your own. [Learn more about audiences](../audience/about-recipients.md).

    ![Screenshot showing the Select audience button](assets/sms_create_2.png){zoomable="yes"}

    Learn how to select an existing audience in [this page](../audience/add-audience.md).

    Learn how to create a new audience in [this page](../audience/one-time-audience.md).

1. Switch on the **[!UICONTROL Enable control group]** option to set a control group to measure the impact of your delivery. Messages are not sent to that control group, so you can compare the behavior of the population that received the message with the behavior of contacts that did not. [Learn more](../audience/control-group.md)

1. You can configure your SMS delivery as a multilingual delivery to send messages based on a profile's preferred language. [Learn more](../msg/multilingual.md).

1. Click **[!UICONTROL Edit content]** to start designing the content of your SMS message. [Learn more](content-sms.md)

    ![Screenshot showing the Edit content button](assets/sms_create_4.png){zoomable="yes"}

    From this screen, you can also [simulate your content](../preview-test/preview-test.md) and [set up offers](../msg/offers.md).

1. To schedule your delivery to a specific date and time, switch on the **[!UICONTROL Enable scheduling]** option. After you initiate the delivery, the message is automatically sent on the exact date and time that you define for the recipient. Learn more about delivery scheduling in [this section](../msg/gs-deliveries.md#gs-schedule).

    >[!NOTE]
    >
    >When a delivery is sent in the context of a workflow, use the **Scheduler** activity. Learn more in [this page](../workflows/activities/scheduler.md).

1. Click **[!UICONTROL Settings]** to access advanced options related to your delivery template. [Learn more](../advanced-settings/delivery-settings.md)

    ![Screenshot showing the Settings button](assets/sms_create_3.png){zoomable="yes"}