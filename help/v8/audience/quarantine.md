---
audience: end-user
title: About quarantine
description: Understand the management of quarantine addresses
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
---
# Quarantine management {#quarantines}

Adobe Campaign manages quarantine addresses for email, push, and SMS channels.

Quarantine applies only to an **email address**, a **phone number**, or a **device token**, but not to the profile itself. For example, a profile whose email address is quarantined can update the profile and enter a new address. The profile could then be targeted by delivery actions again. Likewise, if two profiles share the same phone number, both will be affected if the number is quarantined.

>[!CAUTION]
>
>Quarantine in Adobe Campaign is case sensitive.

## What is quarantine {#quarantines-what}

Quarantine is the method used to **manage invalid addresses in deliveries**.

If a delivery has a high rate of invalid addresses, it may be considered spam. Managing those addresses with quarantine helps prevent being denylisted by internet providers. This is important for maintaining your reputation.

When an address is quarantined in Adobe Campaign, the profile is automatically excluded from the target during delivery analysis.

Quarantine reduces SMS sending costs by excluding erroneous phone numbers from deliveries.

Learn more about quarantines in the [Campaign v8 (console) documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"}.

## Why an address is sent to quarantine {#quarantines-why}

Many reasons can send an address to quarantine: 

* For SMS, erroneous phone numbers
* For SMS, when the profile replies to an SMS message with a keyword such as "STOP"
* For email, when your message is reported as spam. The message is automatically redirected to a technical mailbox managed by Adobe. The user's email address is then automatically sent to quarantine with the Denylisted status.
* An email address can be quarantined, for example, when the mailbox is full, if the address does not exist, or if the email server is unavailable.

Learn more about delivery failures in the [Campaign v8 (console) documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures){target="_blank"}.

## Where to find the quarantine addresses {#quarantines-where}

You can view all the quarantine addresses in your instance in **[!UICONTROL Explorer]** > **[!UICONTROL Administration]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Non deliverables Management]** > **[!UICONTROL Non deliverables and addresses]**. This section lists quarantined elements for email, SMS, and Push notification channels.

![Quarantine location in Adobe Campaign interface](assets/quarantine_location.png){zoomable="yes"}

You can also access a report about the quarantine in your instance:

![Quarantine reports in Adobe Campaign interface](assets/quarantine_reports.png){zoomable="yes"}

For each delivery, you can check the Delivery summary report. It shows the number of addresses in quarantine in the delivery target:

![Delivery summary report showing quarantined addresses](assets/quarantine_delivery.png){zoomable="yes"}

You can explore more options to manage quarantine addresses in the Adobe Campaign console. [Learn more](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses).