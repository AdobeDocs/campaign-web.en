---
audience: end-user
title: Global reports for the Push channel
description: Understand global reports for the Push channel
exl-id: 829a9b68-5c41-47dd-843c-412b6d255e8b
---
# Global reports for the Push channel {#campaign-reports-push}

The global reports provide users with a comprehensive overview of traffic and engagement metrics at a channel level.

Navigate to the **[!UICONTROL Reports]** menu within the **[!UICONTROL Reporting]** section. You can filter your data depending on the report date, folder, or rules. [Learn more](global-reports.md)

## Delivery summary {#delivery-summary-push}

### Delivery overview {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Push delivery overview"
>abstract="The Push **delivery overview** KPIs provide a thorough examination of your push deliveries, delivering detailed insights and specific data. It furnishes comprehensive details regarding the deliveries' performance, effectiveness, and outcomes."

The **[!UICONTROL Delivery Overview]** report provides key performance indicators (KPIs) that give detailed information about how your visitors engage with every push notification delivery. Metrics are detailed below.

![Delivery overview metrics, showing KPIs related to push notification performance.](assets/global_report_push_delivery_overview.png){zoomable="yes"}

+++Learn more about Delivery overview metrics.

* **[!UICONTROL Messages to deliver]**: Total number of messages processed during the delivery preparation.

* **[!UICONTROL Delivered]**: Number of messages successfully sent, in relation to the total number of sent messages.

* **[!UICONTROL Total clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

* **[!UICONTROL Errors]**: Total of errors accumulated during delivery and automatic return processing in relation to the total number of sent messages.

+++

### Targeted audience {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="Push targeted population"
>abstract="The **Targeted population** graph and table showcase data related to your push messaging audience, presenting information about messages to be delivered and exclusions."

The **[!UICONTROL Targeted audience]** table and graph present data related to your recipients for each sent Push notification delivery. Metrics are detailed below.

![Targeted audience metrics, showing data related to recipients and exclusions for push notifications.](assets/global_report_push_targeted_audience.png){zoomable="yes"}

+++Learn more about Targeted audience metrics.

* **[!UICONTROL Targeted audience]**: Total number of targeted recipients.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Exclusion]**: Total number of addresses ignored during the analysis when applying rules: address missing, quarantined, on denylist, and similar reasons.

+++

### Delivery statistics {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Push Delivery statistics"
>abstract="The **Overall statistics** report provides information on sent push notifications, including success rates, errors, and quarantines."

The **[!UICONTROL Delivery statistics]** table details the success of every Push notification delivery. Metrics are detailed below.

![Delivery statistics metrics, showing success rates, errors, and quarantines for push notifications.](assets/global_report_push_delivery_statistics.png){zoomable="yes"}

+++Learn more about Delivery statistics metrics.

* **[!UICONTROL Total messages]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

* **[!UICONTROL Errors / Bounces]**: Total number of errors accumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

* **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (invalid registration, message rejection, payload error, and similar reasons) in relation to the number of messages to be delivered.

    Push notifications error types are listed in the [Adobe Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Causes of exclusion {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Push Causes of exclusion"
>abstract="The **Causes of Exclusion** graph and table illustrate the diverse reasons that prevented user profiles from receiving the push notifications."

The **[!UICONTROL Causes of exclusion]** graph and table display the reasons that prevented user profiles, which were excluded from the targeted profiles, from receiving the message.

Push notifications error types are listed in the [Adobe Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

## Delivery throughput {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Delivery throughput report"
>abstract="The **Delivery throughput** report presents detailed information regarding the push notification delivery throughput of the entire platform within a specified timeframe."

![Delivery throughput metrics, showing success and error rates for push notifications over a specified period.](assets/global_report_push_delivery_throughput.png){zoomable="yes"}

The **[!UICONTROL Delivery Throughput]** report offers comprehensive insights into the effectiveness of the push notification delivery system, offering a detailed summary of success and error rates over a specified period.