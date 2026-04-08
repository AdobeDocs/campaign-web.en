---
audience: end-user
title: Get started with WhatsApp messages
description: Learn how to create and send WhatsApp messages with the Adobe Campaign Web user interface
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
exl-id: 22df2bfa-4d86-464e-ad83-3aa457e3a747
---
# Get started with WhatsApp messages {#get-started-whatsapp}

You can send WhatsApp messages from the **Adobe Campaign Web user interface** using Meta's [Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api/). Use WhatsApp in standalone deliveries, in campaign workflows, or inside marketing campaigns, alongside your other channels.

* **[!UICONTROL Deliveries]**: In the Adobe Campaign Web user interface, create a standalone WhatsApp delivery from the **[!UICONTROL Deliveries]** menu on the left rail—similar to SMS or push. [Learn more](create-whatsapp.md).

* **[!UICONTROL Campaigns]**: In the Adobe Campaign Web user interface, open a campaign and add a WhatsApp delivery from the **[!UICONTROL Deliveries]** tab, or orchestrate sends with a workflow attached to the campaign. [Learn more](../campaigns/create-campaigns.md).

* **[!UICONTROL Workflows]**: In the workflow canvas of the Adobe Campaign Web user interface, add a **[!UICONTROL WhatsApp]** channel activity, choose a delivery template, then define content and settings in the delivery dashboard. Learn more about channel activities in [this section](../workflows/activities/channels.md). (Availability depends on your Adobe Campaign Web user interface entitlement, package, and build.)

![](assets/do-not-localize/whatsapp-beta.png){zoomable="yes"}

>[!NOTE]
>
>Channel configuration (routing account, Meta credentials, webhooks) is performed in the **[!UICONTROL Administration]** section of the Adobe Campaign Web user interface. [Configure the WhatsApp channel](whatsapp-configuration.md) before authoring deliveries.

## Pre-requisites {#prereq}

Integrating WhatsApp requires the following:

* Meta Business Manager account
* [WhatsApp Business Account with verified sender name and phone number](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [User authorization token with appropriate permissions](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [Approved Meta templates](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

You also need to acknowledge the following before proceeding:

* [WhatsApp content rules](https://www.whatsapp.com/legal/messaging-guidelines)
* [Compliance with Meta Policies](https://www.whatsapp.com/legal)
* [24 Hour conversation limits](https://developers.facebook.com/docs/whatsapp/messaging-limits/)

## Limitations {#limitations}

The following limitations apply to the WhatsApp channel:

* The WhatsApp channel can be deployed in HIPAA-ready environments; third-party vendors are not covered under Adobe's BAA. Customers are responsible for their own compliance and vendor validation.

* Automated or predefined response messages may not be available in all configurations.

* Starting April 2025, delivery of all marketing template messages to WhatsApp users who have a United States phone number (a number composed of a +1 dialing code and a US area code) has been temporarily suspended. [Learn more in Meta documentation](https://developers.facebook.com/docs/whatsapp/cloud-api/guides/send-message-templates#per-user-marketing-template-message-limits)

* The native integration does not support integration with third-party Business Service Providers (BSP).


