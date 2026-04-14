---
audience: end-user
title: Create a WhatsApp delivery
description: Learn how to create a WhatsApp delivery in the Adobe Campaign Web user interface
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
exl-id: cac6f675-59e0-431d-8c20-f24ef16d7bf2
hide: true
---

# Create a WhatsApp message {#create-whatsapp}

The **Adobe Campaign Web user interface** lets you design WhatsApp messages that use Meta-approved templates, personalize them for each profile, and test them before send.


+++ Learn more about supported message elements and calls to actions

The following message types are supported in WhatsApp:

| Message Feature | Description |
|-|-|
| Headers | Optional text that appears above the body of your message.|
| Text | Supports dynamic content through parameters. |
| Header image | Optional image that appears above the body of your message. |
| Body Text | Supports dynamic content through parameters. |
| Footer Text | Supports dynamic content through parameters. |

+++


## Create a WhatsApp delivery {#create-whatsapp-journey-campaign}

>[!IMPORTANT]
>
>WhatsApp message feedback is not currently supported.

In the Adobe Campaign Web user interface, follow the steps below to create a standalone WhatsApp delivery.

1. Browse to the **[!UICONTROL Deliveries]** menu, and click **[!UICONTROL Create delivery]**.

    ![](assets/whatsapp-create-1.png)

1. Cchoose **[!UICONTROL WhatsApp]** and select a delivery template. [Learn more about templates](../msg/delivery-template.md).

    ![](assets/whatsapp-create-2.png)

1. Click **[!UICONTROL Create delivery]** to confirm.

1. Click **[!UICONTROL Settings]** for advanced options tied to your template. [Learn more](../advanced-settings/delivery-settings.md)

    ![](assets/whatsapp-create-3.png)

1. Enter a **[!UICONTROL Label]** for the delivery. Use **[!UICONTROL Additional options]** if you need internal name, folder, delivery code, description, or nature, same pattern as other channels.

1. Click **[!UICONTROL Select audience]** to target an existing audience or build one. [Learn more about audiences](../audience/about-recipients.md).

1. Click **[!UICONTROL Edit content]** to open the WhatsApp content editor, refer to [Define your WhatsApp content](#whatsapp-content)).

    ![](assets/whatsapp-create-4.png)

1. You can enable **[!UICONTROL Enable scheduling]** to send on a specific date and time. [Learn more](../msg/gs-deliveries.md#gs-schedule).


## Define your WhatsApp content{#whatsapp-content}

>[!BEGINSHADEBOX]

Before designing your WhatsApp message in the Adobe Campaign Web user interface, create and submit your template in Meta. [Learn more](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

Your WhatsApp template must be approved by Meta before use. Approval often takes a few hours but can take up to 24 hours. [Learn more](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#approval-process)

>[!ENDSHADEBOX]

1. From the delivery configuration page in the Adobe Campaign Web user interface, click **[!UICONTROL Edit content]** to configure the WhatsApp message.

1. Choose Marketing as your **Template category**:

    [Learn more about Template categories](https://developers.facebook.com/docs/whatsapp/updates-to-pricing/new-template-guidelines/#template-category-guidelines)

    ![](assets/whatsapp-design-1.png)

1. From the **WhatsApp template** drop-down, select your Meta-approved template.

    [Learn more about how to create WhatsApp templates](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

    ![](assets/whatsapp-design-2.png)

1. If your Meta-approved template includes an image, provide the **[!UICONTROL Image URL]**.

    ![](assets/whatsapp-design-3.png)

1. In the **Personalization placeholder** field, use the personalization editor to map profile fields and expressions to the template parameters. [Learn more](../personalization/personalize.md).

    ![](assets/whatsapp-design-4.png)

When the message is ready:

* **Standalone or campaign delivery**: Use **[!UICONTROL Review & send]** and **[!UICONTROL Send]** on the delivery dashboard.

* **Workflow**: Open the delivery from the workflow activity when the execution makes it available, then use the delivery dashboard in the same manner. [Learn more](../workflows/start-monitor-workflows.md)

You can then track results from the delivery **[!UICONTROL Reports]** entry points and [delivery reporting](../reporting/delivery-reports.md).
