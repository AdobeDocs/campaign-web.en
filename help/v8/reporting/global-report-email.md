---
audience: end-user
title: Global reports for the email channel
description: Learn more about Global reports for the email channel
badge: label="Limited availability"
---
# Global reports for the email channel {#global-report-direct}

The Global reports provide users with a comprehensive overview of traffic and engagement metrics at a channel-level.

Navigate to the **[!UICONTROL Reports]** menu within the **[!UICONTROL Reporting]** section. You can filter your data depending on the Report date, folder or rules. [Learn more](global-reports.md)

## Delivery summary {#delivery-summary-email}

### Delivery overview {#delivery-overview-email}

The **[!UICONTROL Delivery Overview]** presents key performance metrics (KPIs) offering in-depth insights into the interaction of your visitors with each email delivery. The metrics are outlined below.

![](assets/global_report_email_delivery_overview.png){align="center"}

+++Learn more on Delivery overview metrics.

* **[!UICONTROL Messages to deliver]**: Total number of messages processed during the delivery preparation.

* **[!UICONTROL Delivered]**: Number of messages successfully sent, in relation to the total number of sent messages.

* **[!UICONTROL Total opens]**: Total number of targeted recipients who opened a message at least once.

* **[!UICONTROL Total clicks]**: Total number of recipients who clicked in a delivery at least once.

* **[!UICONTROL Bounces & errors]**: Total of errors cumulated during delivery and automatic return processing in relation to the total number of sent messages.

* **[!UICONTROL Unsubscribes]**: Number of recipients who clicked unsubscriptions.
+++

### Targeted audience {#delivery-summary-email-initial-target}

The table and graph for **[!UICONTROL Targeted Audience]** showcase data related to your recipients, with detailed metrics provided below.

![](assets/global_report_email_targeted_audience.png){align="center"}

+++Learn more on Targeted audience metrics.

* **[!UICONTROL Targeted audience]**: Total number of targeted recipients.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Exclusion]**: Total number of addresses ignored during the analysis when applying rules: address missing, quarantined, on denylist, etc.

+++

### Delivery statistics {#delivery-summary-email-exec-stats}

The **[!UICONTROL Delivery statistics]** table provides a breakdown of the success of every email delivery, with detailed metrics outlined below.

![](assets/global_report_email_delivery_statistics.png){align="center"}

+++Learn more on Delivery statistics metrics.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

* **[!UICONTROL Errors / Bounces]**: Total number of errors cumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

* **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (user unknown, invalid domain) in relation to the number of messages to be delivered.

+++

### Causes of exclusion {#causes-exclusion}

![](assets/global_report_email_exclusions.png){align="center"}

The Exclusions graph and table illustrate the reasons that prevented user profiles, excluded from the targeted profiles, from receiving the message.

Email error types are listed in the [Adobe Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

## Delivery throughput {#delivery-throughput}

![](assets/global_report_email_delivery_throughput.png){align="center"}

This report provides comprehensive details on the delivery throughput within a specified timeframe.

## Non-deliverables {#non-deliverables-email}

### Breakdown of errors per type {#delivery-summary-email-breakdown-per-type}

![](assets/global_report_email_breakdown_type.png){align="center"}

The **[!UICONTROL Breakdown of errors per type]** table and graph present the data related to potential errors experienced in various domains, with specific metrics provided below.
    
The errors shown in this report trigger the quarantine process. For more on quarantine management, refer to [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++Learn more on Breakdown of errors per type metrics.

* **[!UICONTROL User unknown]**: Error type generated during delivery to indicate that the email address is invalid.

* **[!UICONTROL Invalid domain]**: Error type generated when sending a delivery to indicate that the domain of the email address is wrong or does not exist.

* **[!UICONTROL Mailbox full]**: Error type generated after five delivery attempts to indicate that the recipients' inbox contains too many messages.

* **[!UICONTROL Account disabled]**: Error type generated when sending a delivery to indicate that the address no longer exists.

* **[!UICONTROL Refused]**: Error type generated when an address is rejected by the IAP (Internet Access Provider), for instance following the application of a security rule (anti-spam software).

* **[!UICONTROL Unreachable]**: Error type which occurs in the message distribution string: incident on the SMTP relay, domain temporarily unreachable, etc

* **[!UICONTROL Not connected]**: Error type to indicate that the recipients' mobile phone is switched off or disconnected from the network at the time of sending.

+++

### Breakdown of errors per domain {#delivery-summary-email-breakdown-per-domain}

![](assets/global_report_email_breakdown_domain.png){align="center"}

The **[!UICONTROL Breakdown of errors per domain]** table and graph showcase the data related to potential errors within each domain. Metrics are common with the **[!UICONTROL Breakdown of errors per type]** table and graph detailed above.

## Tracking indicators {#tracking-indicators-email}

### Delivery statistics {#delivery-summary-email-statistics}

The **[!UICONTROL Delivery statistics]** metrics offer key performance indicators (KPIs) providing detailed information regarding the data associated with every email delivery. Further details on these metrics are provided below.
 
![](assets/global_report_email_delivery_statistics_tracking.png){align="center"}

+++Learn more on Delivery statistics metrics.

* **[!UICONTROL Messages to deliver]**: Total number of messages processed during the delivery preparation.

* **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

* **[!UICONTROL Unique opens]**: Total number of targeted recipients who opened a message at least once. 

* **[!UICONTROL Total Opens]**: Number of distinct targeted recipients for this domain who have opened a message at least once.

* **[!UICONTROL Clicks on the opt-out link]**:  Number of clicks on the unsubscription link.

* **[!UICONTROL Clicks on the mirror link]**: Number of clicks on the link to the mirror page.

* **[!UICONTROL Estimation of forwards]**: Estimation of the number of emails forwarded by the targeted recipients. 
+++

### Open and click-trough rate {#delivery-summary-open-rate}

The **[!UICONTROL Open and click-trough rate]** table displays data relative to your recipients. Metrics are detailed below.

![](assets/global_report_email_opens.png){align="center"}

+++Learn more on Open and click-trough rate metrics.

* **[!UICONTROL Sent]**: Total number of messages sent.

* **[!UICONTROL Complaints]**: Number and percentage of messages for this domain that have been reported as undesirable by the recipient.

* **[!UICONTROL Unique Opens]**: Number and percentage of distinct targeted recipients for this domain who have opened a message at least once.

* **[!UICONTROL Unique Clicks]**: Number and percentage of distinct targeted recipients who clicked in the same delivery at least once. 

* **[!UICONTROL Raw reactivity]**: Percentage of the number of recipient who clicked in a delivery at least once compared to the number of recipients who opened a delivery at least once.
    +++

## URLs and click streams {#url-email}

### URLs and click streams KPIs {#url-email-kpis}

The **[!UICONTROL URLs and click streams]** report provides key performance indicators (KPIs) that provide detailed insights into the URLs that received the highest number of clicks during a delivery. Metrics are detailed below.

![](assets/campaign_report_email_9.png){align="center"}

+++Learn more on URLs and click streams metrics.

* **[!UICONTROL Reactivity]**: Ratio of the number of targeted recipients having clicked in a delivery, in relation to the estimated number of targeted recipients having opened a delivery.

* **[!UICONTROL Unique clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

* **[!UICONTROL Total Clicks]**: Total number of clicks on links in deliveries.

* **[!UICONTROL Platform average]** : This average rate, displayed under each rate (reactivity, distinct clicks, and cumulated clicks), is calculated for deliveries sent over the previous six months. Only deliveries with the same typology and on the same channel are taken into account. Proofs are excluded.
    +++

### Top 10 most visited links {#top10-campaign-report-email}

The **[!UICONTROL Top 10 most visited links]** graph and table contain the available data for recipient behavior per link. Metrics are detailed below.

![](assets/global_report_email_top10.png){align="center"}

+++Learn more on Top 10 most visited links metrics.

* **[!UICONTROL Total Clicks]**: Total number of clicks on links in deliveries.

* **[!UICONTROL Percentage]**: Percentage of users who interacted with the delivery.

+++

### Breakdown of clicks over time {#campaign-report-email-breakdown-clicks}

The **[!UICONTROL Breakdown of clicks over time]** graph contains the available data for recipient behavior per link. 

![](assets/global_report_email_breakdown_clicks.png){align="center"}

## User Activities {#user-activities-email}

The **[!UICONTROL User activities]** report shows the breakdown of opens and clicks in the form of a chart. Metrics for this report are detailed below.

![](assets/global_report_email_user.png){align="center"}

+++Learn more on User activities metrics.

* **[!UICONTROL Total Clicks]**: Total number of clicks on links in deliveries.

* **[!UICONTROL Total Opens]**: Total number of distinct targeted recipients for this domain who have opened a message at least once.

+++
