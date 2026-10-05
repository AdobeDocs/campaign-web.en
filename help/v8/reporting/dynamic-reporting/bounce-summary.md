---
title: Bounce summary
description: With the Bounce summary out-of-the-box report, learn about the status of your sent campaigns and errors they may have encountered.
audience: end-user
level: Intermediate
exl-id: b341edad-aa82-43d8-a5a1-b33a19973a1a
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
---
# Bounce summary{#bounce-summary}

This report details the overall hard and soft errors encountered during deliveries as well as the automatic processing of bounces. 

![](assets/campaign_reports_bounces.png)

Each table is represented by summary numbers and charts. You can change how the details are shown in their respective visualization settings.

**Flop 5 repartition** lists the five deliveries with the highest number of quarantines:

The **Bounce reasons** table contains the available data for the types of errors that caused bounces for each delivery:

* **[!UICONTROL User unknown]**: The type of error generated when a delivery is sent to an invalid email address.
* **[!UICONTROL Invalid domain]**: The type of error generated when a delivery is sent to an email address whose domain is wrong or no longer exists.
* **[!UICONTROL Unreachable]**: The type of error encountered in the message delivery string, such as domain temporarily unreachable.
* **[!UICONTROL Account disabled]**: The type of error generated when a delivery is sent to an email address that no longer exists.
* **[!UICONTROL Mailbox full]**: The type of error generated when the recipient's inbox is full. There are five attempts to deliver the message before this error is generated.
* **[!UICONTROL Not connected]**: The type of error generated when the recipient's mobile phone is off or it is not connected to a network at the time the message is sent.

  >[!NOTE]
  >
  >This type of error only concerns deliveries on mobile channels.

* **[!UICONTROL Refused]**: The type of error generated when an address is refused by the Internet service provider (ISP). For example, when a security rule has been applied by anti-Spam software.

The **Domain repartition** table displays the overall problems encountered during the deliveries according to the recipient domain.
