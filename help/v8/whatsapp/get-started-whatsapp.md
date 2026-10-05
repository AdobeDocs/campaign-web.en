---
audience: end-user
title: Get started with WhatsApp messages
description: Learn how to create and send WhatsApp messages with the Adobe Campaign Web user interface
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
---
# Get started with WhatsApp messages {#get-started-whatsapp}

You can send WhatsApp messages from the **Adobe Campaign Web user interface** using Meta's [Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api/). Use WhatsApp in standalone deliveries, in campaign workflows, or inside marketing campaigns, alongside your other channels.

* **[!UICONTROL Deliveries]**: In the Adobe Campaign Web user interface, create a standalone WhatsApp delivery from the **[!UICONTROL Deliveries]** menu on the left rail—similar to SMS or push. [Learn more](create-whatsapp.md).

* **[!UICONTROL Campaigns]**: In the Adobe Campaign Web user interface, open a campaign and add a WhatsApp delivery from the **[!UICONTROL Deliveries]** tab, or orchestrate sends with a workflow attached to the campaign. [Learn more](../campaigns/create-campaigns.md).

* **[!UICONTROL Workflows]**: In the workflow canvas of the Adobe Campaign Web user interface, add a **[!UICONTROL WhatsApp]** channel activity, choose a delivery template, then define content and settings in the delivery dashboard. Learn more about channel activities in [this section](../workflows/activities/channels.md).

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


