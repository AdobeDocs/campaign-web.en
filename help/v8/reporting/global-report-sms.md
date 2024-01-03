---
audience: end-user
title: Global reports for the SMS channel
description: Understand Global reports for the SMS channel
badge: label="Limited Availability"
---
# Global reports for the SMS channel {#campaign-reports-sms}

The Global reports provide users with a comprehensive overview of traffic and engagement metrics at a channel-level.

Navigate to the **[!UICONTROL Reports]** menu within the **[!UICONTROL Reporting]** section. You can filter your data depending on the Report date, folder or rules. [Learn more](global-reports.md)

## Delivery summary {#delivery-summary-sms}

### Delivery overview {#delivery-overview-sms}

The **[!UICONTROL Delivery Overview]** report offers comprehensive key performance indicators (KPIs) providing in-depth insights into the interaction patterns of your visitors with each SMS delivery. The following metrics are outlined below.
    
![](assets/global_report_sms_delivery_overview.png)

+++Learn more on Delivery overview metrics.

* **[!UICONTROL Messages to deliver]**: Total number of messages processed during the delivery preparation.

* **[!UICONTROL Delivered]**: Percentage of messages successfully sent, in relation to the total number of sent messages.

* **[!UICONTROL Click-through rate]**: Percentage of distinct recipients who clicked in a delivery at least once.

* **[!UICONTROL Errors]**: Percentage of errors cumulated during delivery and automatic return processing in relation to the total number of sent messages.

+++

### Targeted audience {#delivery-summary-sms-initial-target}

The **[!UICONTROL Targeted audience]** table and graph present data related to your recipients for each sent SMS delivery. Metrics are detailed below.

![](assets/global_report_sms_targeted_audience.png)

+++Learn more on Targeted audience metrics.

* **[!UICONTROL Targeted audience]**: Total number of targeted recipients.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Exclusion]**: Total number of addresses ignored during the analysis when applying rules: address missing, quarantined, on denylist, etc.

+++

### Delivery statistics {#delivery-summary-sms-exec-stats}

The **[!UICONTROL Delivery statistics]** table details the success of your every SMS delivery. Metrics are detailed below.

![](assets/global_report_sms_delivery_statistics.png)

+++Learn more on Delivery statistics metrics.

* **[!UICONTROL Total messages]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

* **[!UICONTROL Errors / Bounces]**: Total number of errors cumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

* **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (user unknown, invalid domain) in relation to the number of messages to be delivered.

    SMS error types are listed in the [Adobe Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Causes of exclusion {#causes-exclusion}

The **[!UICONTROL Causes of exclusion]** graph and table display the reasons that prevented user profiles, which were excluded from the targeted profiles, from receiving your SMS deliveries.

Error types are listed in the [Adobe Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## Delivery throughput {#delivery-throughput-sms}

![](assets/global_report_sms_delivery_throughput.png)

This report provides comprehensive details on the delivery throughput within a specified timeframe.
