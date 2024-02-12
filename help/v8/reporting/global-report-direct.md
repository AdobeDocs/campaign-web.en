---
audience: end-user
title: Global reports for the direct mail channel
description: Learn more about Global reports for the direct mail channel

---
# Global reports for the direct mail channel {#global-report-direct}

The Global reports provide users with a comprehensive overview of traffic and engagement metrics at a channel-level.

Navigate to the **[!UICONTROL Reports]** menu within the **[!UICONTROL Reporting]** section. You can filter your data depending on the Report date, folder or rules. [Learn more](global-reports.md)

## Delivery summary {#delivery-summary-direct}

### Delivery overview {#delivery-overview-direct}

The **[!UICONTROL Delivery Overview]** presents key performance metrics (KPIs) offering in-depth insights into the interaction of your visitors with each email delivery. The metrics are outlined below.

![](assets/global_report_email_delivery_overview.png){zoomable="yes"}{align="center"}

+++Learn more on Delivery overview metrics.

* **[!UICONTROL Messages to deliver]**: Total number of messages processed during the delivery preparation.

* **[!UICONTROL Delivered]**: Number of messages successfully sent, in relation to the total number of sent messages.

* **[!UICONTROL Errors]**: Total of errors cumulated during delivery and automatic return processing in relation to the total number of sent messages.

* **[!UICONTROL Unsubscribes]**: Number of recipients who clicked unsubscriptions.
+++

### Targeted audience {#delivery-summary-direct-initial-target}

The table and graph for **[!UICONTROL Targeted Audience]** showcase data related to your recipients, with detailed metrics provided below.

![](assets/global_report_email_targeted_audience.png){zoomable="yes"}{align="center"}

+++Learn more on Targeted audience metrics.

* **[!UICONTROL Targeted audience]**: Total number of targeted recipients.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Exclusion]**: Total number of addresses ignored during the analysis when applying rules: address missing, quarantined, on denylist, etc.

+++

### Delivery statistics {#delivery-summary-direct-exec-stats}

The **[!UICONTROL Delivery statistics]** table provides a breakdown of the success of every direct mail delivery, with detailed metrics outlined below.

![](assets/global_report_email_delivery_statistics.png){zoomable="yes"}{align="center"}

+++Learn more on Delivery statistics metrics.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

* **[!UICONTROL Errors / Bounces]**: Total number of errors cumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

* **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (user unknown, invalid domain) in relation to the number of messages to be delivered.

+++

### Causes of exclusion {#causes-exclusion}

![](assets/global_report_email_exclusions.png){zoomable="yes"}{align="center"}

The Exclusions graph and table illustrate the reasons that prevented user profiles, excluded from the targeted profiles, from receiving the message.

## Delivery throughput {#delivery-throughput}

This report provides comprehensive details on the delivery throughput within a specified timeframe. The key metric used to measure the speed of message delivery is the number of messages sent per hour.

## Non-deliverables {#non-deliverables-direct}

### Breakdown of errors per type {#delivery-summary-direct-breakdown-per-type}

The **[!UICONTROL Breakdown of errors per type]** table and graph present the data related to potential errors experienced in various domains, with specific metrics provided below.
    
The errors shown in this report trigger the quarantine process. For more on quarantine management, refer to [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++Learn more on Breakdown of errors per type metrics.

* **[!UICONTROL User unknown]**: Error type generated during delivery to indicate that the address is invalid.

* **[!UICONTROL Invalid domain]**: Error type generated when sending a delivery to indicate that the domain of the address is wrong or does not exist.

* **[!UICONTROL Mailbox full]**: Error type generated after five delivery attempts to indicate that the recipients' inbox contains too many messages.

* **[!UICONTROL Account disabled]**: Error type generated when sending a delivery to indicate that the address no longer exists.

* **[!UICONTROL Refused]**: Error type generated when an address is rejected by the IAP (Internet Access Provider), for instance following the application of a security rule (anti-spam software).

* **[!UICONTROL Unreachable]**: Error type which occurs in the message distribution string: incident on the SMTP relay, domain temporarily unreachable, etc

* **[!UICONTROL Not connected]**: Error type to indicate that the recipients' mobile phone is switched off or disconnected from the network at the time of sending.

+++

### Breakdown of errors per domain {#delivery-summary-email-breakdown-per-domain}

The **[!UICONTROL Breakdown of errors per domain]** table and graph showcase the data related to potential errors within each domain. Metrics are common with the **[!UICONTROL Breakdown of errors per type]** table and graph detailed above.

