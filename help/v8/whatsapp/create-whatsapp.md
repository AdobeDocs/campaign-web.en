---
audience: end-user
title: Create a WhatsApp delivery
description: Learn how to create a WhatsApp delivery in the Adobe Campaign Web user interface
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
exl-id: cac6f675-59e0-431d-8c20-f24ef16d7bf2
---

# Create a WhatsApp message {#create-whatsapp}

The **Adobe Campaign Web user interface** lets you design WhatsApp messages that use Meta-approved templates, personalize them for each profile, and test them before send. Create a **standalone** delivery, add a delivery **inside a campaign**, or place a **WhatsApp channel activity** in a workflow, the authoring experience is the same once the delivery editor opens.

Outbound template-based messages are supported as described below.

+++ Learn more about supported message elements and calls to actions

The following message types are supported in WhatsApp:

| Message Feature | Description |
|-|-|
| Headers | Optional text that appears above the body of your message.|
| Text | Supports dynamic content through parameters. |
| Images (JPEG, PNG) | Must be in 8-bit RGB or RGBA format and under 5 MB in size. |
| Videos | Must be 3GPP or MP4, under 16 MB, and hosted via URL. |
| Audio | Only available for response messages. Must be AAC, AMR, MP3, MP4 audio, or OGG format, hosted on a URL, and under 16 MB. |
| Documents | Must be under 100 MB, hosted on a URL, and in one of the following formats: .txt, .xls/.xlsx, .doc/.docx, .ppt/.pptx, or .pdf. |
| Body Text | Supports dynamic content through parameters. |
| Footer Text | Supports dynamic content through parameters. |

The following call-to-action option is available for your WhatsApp messages:

| Call to actions | Description |
|-|-|
| Visit website| Only one button is permitted, with variable parameters included.|
| Call on WhatsApp| Provides a button that opens a WhatsApp chat with the specified phone number directly from the message.|
| Call phone number | Provides a button that initiates a phone call to the specified number when tapped by the user.|

+++

## Create a WhatsApp delivery {#create-whatsapp-journey-campaign}

In the Adobe Campaign Web user interface, follow the steps below to create a standalone WhatsApp delivery.

1. Browse to the **[!UICONTROL Deliveries]** menu on the left rail, and click **[!UICONTROL Create delivery]**.

1. Under **[!UICONTROL Channel]**, choose **[!UICONTROL WhatsApp]** and select a delivery template. [Learn more about templates](../msg/delivery-template.md).

1. Click **[!UICONTROL Create delivery]** to confirm.

1. Enter a **[!UICONTROL Label]** for the delivery. Use **[!UICONTROL Additional options]** if you need internal name, folder, delivery code, description, or nature, same pattern as other channels.

1. Click **[!UICONTROL Select audience]** to target an existing audience or build one. [Learn more about audiences](../audience/about-recipients.md).

1. Click **[!UICONTROL Edit content]** to open the WhatsApp content editor, refer to [Define your WhatsApp content](#whatsapp-content)).

1. You can enable **[!UICONTROL Enable scheduling]** to send on a specific date and time. [Learn more](../msg/gs-deliveries.md#gs-schedule).

1. Click **[!UICONTROL Settings]** for advanced options tied to your template. [Learn more](../advanced-settings/delivery-settings.md)


## Define your WhatsApp content{#whatsapp-content}

>[!BEGINSHADEBOX]

Before designing your WhatsApp message in the Adobe Campaign Web user interface, create and submit your template in Meta. [Learn more](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

Your WhatsApp template must be approved by Meta before use. Approval often takes a few hours but can take up to 24 hours. [Learn more](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#approval-process)

>[!ENDSHADEBOX]

1. From the delivery configuration screen in the Adobe Campaign Web user interface, click **[!UICONTROL Edit content]** to configure the WhatsApp message.

1. Choose your **Template category**:

    * Marketing
    * Utility

    [Learn more about Template categories](https://developers.facebook.com/docs/whatsapp/updates-to-pricing/new-template-guidelines/#template-category-guidelines)

    ![](assets/whatsapp-design-1.png)

1. From the **WhatsApp template** drop-down, select your Meta-approved template.

    [Learn more about how to create WhatsApp templates](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

    ![](assets/whatsapp-design-2.png)

1. Use the personalization editor to map profile fields and expressions into template parameters. [Learn more](../personalization/personalize.md).

    ![](assets/whatsapp-design-4.png)

When the message is ready:

* **Standalone or campaign delivery**: In the Adobe Campaign Web user interface, open the delivery, run preparation if prompted, then use **[!UICONTROL Review & send]** and **[!UICONTROL Send]** from the delivery dashboard.

* **Workflow**: In the Adobe Campaign Web user interface, start or resume the workflow so the delivery reaches a ready state, open the delivery from the activity, then confirm send from the delivery dashboard. [Learn more](../workflows/start-monitor-workflows.md)

In the Adobe Campaign Web user interface, track results from the delivery **[!UICONTROL Reports]** entry points and [delivery reporting](../reporting/delivery-reports.md).
