---
audience: end-user
title: Global reports for the email channel
description: Learn more about global reports for the email channel
exl-id: 37c575e5-fd18-4a35-a11a-922d5bda1bae
---
# Global reports for the Email channel {#global-report-direct}

The global reports provide users with a comprehensive overview of traffic and engagement metrics at a channel-level.

Navigate to the **[!UICONTROL Reports]** menu within the **[!UICONTROL Reporting]** section. You can filter your data depending on the Report date, folder or rules. [Learn more](global-reports.md)

## Delivery summary {#delivery-summary-email}

### Delivery overview {#delivery-overview-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_deliveries_overview_email"
>title="Delivery overview"
>abstract="The **Delivery Overview** presents key performance indicators (KPIs) that offer in-depth insights into how your audience interacts with the email deliveries and campaigns you send."

The **[!UICONTROL Delivery Overview]** presents key performance metrics (KPIs) offering in-depth insights into the interaction of your visitors with each email delivery. The metrics are outlined below.

![](assets/global_report_email_delivery_overview.png){zoomable="yes"}{align="center"}

+++Learn more on Delivery overview metrics.

* **[!UICONTROL Messages to deliver]**: Total number of messages processed during the delivery preparation.

* **[!UICONTROL Delivered]**: Number of messages successfully sent, in relation to the total number of sent messages.

* **[!UICONTROL Total opens]**: Total number of targeted recipients who opened a message at least once.

* **[!UICONTROL Total clicks]**: Total number of recipients who clicked in a delivery at least once.

* **[!UICONTROL Bounces & errors]**: Total of errors cumulated during delivery and automatic return processing in relation to the total number of sent messages.

* **[!UICONTROL Unsubscribes]**: Number of recipients who clicked unsubscriptions.
+++

### Targeted audience {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_email"
>title="Initial target audience statistics"
>abstract="The **Targeted Audience** table and graph offer insights into recipient engagement, helping you assess the effectiveness of your campaigns and deliveries."

The table and graph for **[!UICONTROL Targeted Audience]** showcase data related to your recipients, with detailed metrics provided below.

![](assets/global_report_email_targeted_audience.png){zoomable="yes"}{align="center"}

+++Learn more on Targeted audience metrics.

* **[!UICONTROL Targeted audience]**: Total number of targeted recipients.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Exclusion]**: Total number of addresses ignored during the analysis when applying rules: address missing, quarantined, on denylist, etc.

+++

### Delivery statistics {#delivery-summary-email-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_email_delivery_stats"
>title="Delivery statistics"
>abstract="The **Delivery Statistics** graph and table outline key metrics, including successful deliveries, errors, and new quarantines, offering a concise overview to evaluate delivery performance."

The **[!UICONTROL Delivery statistics]** table provides a breakdown of the success of every email delivery, with detailed metrics outlined below.

![](assets/global_report_email_delivery_statistics.png){zoomable="yes"}{align="center"}

+++Learn more on Delivery statistics metrics.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

* **[!UICONTROL Errors / Bounces]**: Total number of errors cumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

* **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (user unknown, invalid domain) in relation to the number of messages to be delivered.

+++

### Causes of exclusion {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusion_email"
>title="Causes of exclusion"
>abstract="The **Causes of Exclusion** graph and table illustrate the specific reasons for message rejections during delivery preparation, offering a detailed breakdown by rule."

![](assets/global_report_email_exclusions.png){zoomable="yes"}{align="center"}

The Exclusions graph and table illustrate the reasons that prevented user profiles, excluded from the targeted profiles, from receiving the message.

Email error types are listed in the [Adobe Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

## Delivery throughput {#delivery-throughput}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_email"
>title="Delivery throughput"
>abstract="This **Delivery throughput** delivers comprehensive insights into delivery throughput, highlighting success and error rates within a specified timeframe."

![](assets/global_report_email_delivery_throughput.png){zoomable="yes"}{align="center"}

The Delivery Throughput report provides in-depth insights into the efficiency of the delivery process, presenting a detailed overview of success and error rates within a specified timeframe.

+++Learn more on Delivery throughput metrics.

* **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

* **[!UICONTROL Errors]**: Total number of errors cumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

+++

## Non-deliverables {#non-deliverables-email}

### Breakdown of errors per type {#delivery-summary-email-breakdown-per-type}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_error_type_email"
>title="Breakdown of errors per type"
>abstract="The table and graph detailing the **Breakdown of errors per type** encompass information on various error types encountered during the process, including user unknown, mailbox full, invalid domain, and others."

![](assets/global_report_email_breakdown_type.png){zoomable="yes"}{align="center"}

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

>[!CONTEXTUALHELP]
>id="acw_global_reporting_error_domain_email"
>title="Breakdown of errors per domain"
>abstract="The table and graph illustrating the **Breakdown of Errors per Domain** present the data corresponding to each error type encountered, categorized by specific domains."

![](assets/global_report_email_breakdown_domain.png){zoomable="yes"}{align="center"}

The **[!UICONTROL Breakdown of errors per domain]** table and graph showcase the data related to potential errors within each domain. Metrics are common with the **[!UICONTROL Breakdown of errors per type]** table and graph detailed above.

## Tracking indicators {#tracking-indicators-email}

### Delivery statistics {#delivery-summary-email-statistics}

>[!CONTEXTUALHELP]
>id="acw_global_delivery_statistics_summary_email"
>title="Delivery statistics"
>abstract="The **Delivery Statistics** Key Performance Indicators (KPIs) provide a comprehensive overview of your deliveries and campaigns performance, offering insights into both successful deliverie, encountered errors and user engagement."

The **[!UICONTROL Delivery statistics]** metrics offer key performance indicators (KPIs) providing detailed information regarding the data associated with every email delivery. Further details on these metrics are provided below.
 
![](assets/global_report_email_delivery_statistics_tracking.png){zoomable="yes"}{align="center"}

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

>[!CONTEXTUALHELP]
>id="acw_global_reporting_open_clickthrough_email"
>title="Open and click-through rate"
>abstract="The table for **Open and click-through rates** reveals recipient engagement with your delivery, showcasing data on open rates and click-through rates for a quick and insightful overview."

The **[!UICONTROL Open and click-trough rate]** table displays data relative to your recipients. Metrics are detailed below.

![](assets/global_report_email_opens.png){zoomable="yes"}{align="center"}

+++Learn more on Open and click-trough rate metrics.

* **[!UICONTROL Sent]**: Total number of messages sent.

* **[!UICONTROL Complaints]**: Number and percentage of messages for this domain that have been reported as undesirable by the recipient.

* **[!UICONTROL Unique Opens]**: Number and percentage of distinct targeted recipients for this domain who have opened a message at least once.

* **[!UICONTROL Unique Clicks]**: Number and percentage of distinct targeted recipients who clicked in the same delivery at least once. 

* **[!UICONTROL Raw reactivity]**: Percentage of the number of recipient who clicked in a delivery at least once compared to the number of recipients who opened a delivery at least once.
    +++

## URLs and click streams {#url-email}

### URLs and click streams KPIs {#url-email-kpis}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_urls_clickstreams_email"
>title="URLs and click streams"
>abstract="The **URLs and click streams** report provides essential Key Performance Indicators (KPIs) offering detailed insights into the most-clicked URLs during a delivery."

The **[!UICONTROL URLs and click streams]** report provides key performance indicators (KPIs) that provide detailed insights into the URLs that received the highest number of clicks during a delivery. Metrics are detailed below.

![](assets/campaign_report_email_9.png){zoomable="yes"}{align="center"}

+++Learn more on URLs and click streams metrics.

* **[!UICONTROL Reactivity]**: Ratio of the number of targeted recipients having clicked in a delivery, in relation to the estimated number of targeted recipients having opened a delivery.

* **[!UICONTROL Unique clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

* **[!UICONTROL Total Clicks]**: Total number of clicks on links in deliveries.

* **[!UICONTROL Platform average]**: This average rate, displayed under each rate (reactivity, distinct clicks, and cumulated clicks), is calculated for deliveries sent over the previous six months. Only deliveries with the same typology and on the same channel are taken into account. Proofs are excluded.
    +++

### Top 10 most visited links {#top10-global-report-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_top10_email"
>title="Top 10 most visited links"
>abstract="The **Top 10 most visited links**  graph and table present comprehensive data on recipient interaction with each link."

The **[!UICONTROL Top 10 most visited links]** graph and table contain the available data for recipient behavior per link. Metrics are detailed below.

![](assets/global_report_email_top10.png){zoomable="yes"}{align="center"}

+++Learn more on Top 10 most visited links metrics.

* **[!UICONTROL Total Clicks]**: Total number of clicks on links in deliveries.

* **[!UICONTROL Percentage]**: Percentage of users who interacted with the delivery.

+++

### Breakdown of clicks over time {#global-report-email-breakdown-clicks}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_urls_click_breakdown_email"
>title="Breakdown of clicks over time"
>abstract="The **Breakdown of clicks over time** graph offers a comprehensive view of how recipients engage with links throughout the designated timeframe."

The **[!UICONTROL Breakdown of clicks over time]** graph contains the available data for recipient behavior per link. 

![](assets/global_report_email_breakdown_clicks.png){zoomable="yes"}{align="center"}

## User Activities {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_user_activities_email"
>title="User activities"
>abstract="The graphical representation of **User Activities** offers a detailed breakdown of recipient interactions, portraying opens and clicks through an informative chart format."

The **[!UICONTROL User activities]** report shows the breakdown of opens and clicks in the form of a chart. Metrics for this report are detailed below.

![](assets/global_report_email_user.png){zoomable="yes"}{align="center"}

+++Learn more on User activities metrics.

* **[!UICONTROL Total Clicks]**: Total number of clicks on links in deliveries.

* **[!UICONTROL Total Opens]**: Total number of distinct targeted recipients for this domain who have opened a message at least once.

+++
