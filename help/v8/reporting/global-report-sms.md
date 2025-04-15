---
audience: end-user
title: Global reports for the SMS channel
description: Understand global reports for the SMS channel
exl-id: 346cf2ff-b6e4-4d8f-ba26-197eadeaf5e6
---
# Global reports for the SMS channel {#campaign-reports-sms}

The global reports provide users with a comprehensive overview of traffic and engagement metrics at a channel level.

Navigate to the **[!UICONTROL Reports]** menu within the **[!UICONTROL Reporting]** section. You can filter your data depending on the report date, folder, or rules. [Learn more](global-reports.md)

## Delivery summary {#delivery-summary-sms}

### Delivery overview {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="SMS delivery overview"
>abstract="The **SMS delivery overview** KPIs provide a thorough summary of your SMS delivery, offering detailed insights and specific data. It delivers comprehensive information about the performance, effectiveness, and outcomes of your delivery."

The **[!UICONTROL Delivery Overview]** report offers comprehensive key performance indicators (KPIs), providing in-depth insights into the interaction patterns of your visitors with each SMS delivery. The following metrics are outlined below.

![A screenshot of the Delivery Overview report, showing key performance indicators for SMS delivery.](assets/global_report_sms_delivery_overview.png){zoomable="yes"}

+++Learn more on Delivery overview metrics.

* **[!UICONTROL Messages to deliver]**: Total number of messages processed during the delivery preparation.

* **[!UICONTROL Delivered]**: Percentage of messages successfully sent, in relation to the total number of sent messages.

* **[!UICONTROL Click-through rate]**: Percentage of distinct recipients who clicked in a delivery at least once.

* **[!UICONTROL Errors]**: Percentage of errors accumulated during delivery and automatic return processing, in relation to the total number of sent messages.

+++

### Targeted audience {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="SMS targeted population"
>abstract="The graph and table for the **Targeted population** present data related to your SMS audience, including information on messages to be delivered and exclusions."

The **[!UICONTROL Targeted audience]** table and graph present data related to your recipients for each sent SMS delivery. Metrics are detailed below.

![A screenshot of the Targeted Audience report, showing data on recipients and exclusions for SMS deliveries.](assets/global_report_sms_targeted_audience.png){zoomable="yes"}

+++Learn more on Targeted audience metrics.

* **[!UICONTROL Targeted audience]**: Total number of targeted recipients.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Exclusion]**: Total number of addresses ignored during the analysis when applying rules, such as address missing, quarantined, or on a denylist.

+++

### Delivery statistics {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="SMS Delivery statistics"
>abstract="The **Delivery statistics** report provides comprehensive insights into the sent SMS, offering a breakdown of various metrics such as success rates, error occurrences, and audience placed in quarantine. This detailed presentation allows for a thorough examination of the overall performance and outcomes of the SMS delivery process."

The **[!UICONTROL Delivery statistics]** table details the success of every SMS delivery. Metrics are detailed below.

![A screenshot of the Delivery Statistics report, showing success rates, errors, and quarantines for SMS deliveries.](assets/global_report_sms_delivery_statistics.png){zoomable="yes"}

+++Learn more on Delivery statistics metrics.

* **[!UICONTROL Total messages]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Success]**: Number of messages processed successfully, in relation to the number of messages to be delivered.

* **[!UICONTROL Errors / Bounces]**: Total number of errors accumulated during deliveries and automatic rebound processing, in relation to the number of messages to be delivered.

* **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (e.g., user unknown, invalid domain), in relation to the number of messages to be delivered.

    SMS error types are listed in the [Adobe Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Causes of exclusion {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="SMS Causes of exclusion"
>abstract="The **Causes of exclusion** graph and table illustrate the diverse reasons that prevented user profiles from receiving the SMS messages."

The **[!UICONTROL Causes of exclusion]** graph and table display the reasons that prevented user profiles, which were excluded from the targeted profiles, from receiving your SMS deliveries.

Error types are listed in the [Adobe Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![A screenshot of the Causes of Exclusion report, showing reasons for SMS delivery exclusions.](assets/global_report_sms_causes_exclusion.png){zoomable="yes"}

## Delivery throughput {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="SMS delivery throughput"
>abstract="The **Delivery throughput** report provides extensive insights into the efficiency of the SMS message delivery system, presenting a detailed overview of success and error rates within a specified timeframe."

![A screenshot of the Delivery Throughput report, showing success and error rates for SMS deliveries over time.](assets/global_report_sms_delivery_throughput.png){zoomable="yes"}

The **[!UICONTROL Delivery Throughput]** report offers comprehensive insights into the effectiveness of the SMS message delivery system, offering a detailed summary of success and error rates over a specified period.