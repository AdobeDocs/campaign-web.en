---
audience: end-user
title: Get started with LINE messages
description: Learn how to create and send LINE messages with the Adobe Campaign Web user interface
feature: Line App
topic: Content Management
role: User
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
subfeature_v2:
  - id: d9d413df-4e9e-4906-bbbc-28c06c2ccf59
    internal-label: LINE App
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
---
# Get started with LINE messages {#get-started-line}

LINE is an application for free instant messaging, voice and video calls, available on all mobile devices and on PC. You can use Adobe Campaign to send LINE messages. Use LINE in standalone deliveries or in workflows, alongside your other channels.

![Example of a LINE message received on a mobile device](assets/line-message.png)

* **[!UICONTROL Deliveries]**: Create a standalone LINE delivery from the **[!UICONTROL Deliveries]** menu on the left rail, similar to SMS or push. [Learn more](send-line.md).

* **[!UICONTROL Workflows]**: In the workflow canvas, add a **[!UICONTROL LINE]** channel activity, choose a delivery template, then define content and settings in the delivery dashboard. Learn more about channel activities in [this section](../workflows/activities/channels.md).

    >[!NOTE]
    >
    >In the **[!UICONTROL Build audience]** activity that feeds your **[!UICONTROL LINE]** channel activity, change the targeting dimension to **[!UICONTROL Visitor subscriptions]**. Make sure you enable **[!UICONTROL Show all schemas]** in the side panel. The delivery template selector only becomes available once this targeting dimension is set.
