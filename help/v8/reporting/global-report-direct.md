---
audience: end-user
title: Global reports for the direct mail channel
description: Learn more about Global reports for the direct mail channel
exl-id: a42536fe-375b-4169-8775-d47ed26692f8
---
# Global reports for the direct mail channel {#global-report-direct}

The Direct mail global reports provide users with a comprehensive overview of traffic and engagement metrics at a channel-level.

Navigate to the **[!UICONTROL Reports]** menu within the **[!UICONTROL Reporting]** section. You can filter your data depending on the Report date, folder or rules. [Learn more](global-reports.md)

## Delivery summary {#delivery-summary-direct}

### Delivery overview {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_overview_direct_mail"
>title="Delivery overview"
>abstract="The **Delivery Overview** presents key performance metrics (KPIs) offering in-depth insights into the interaction of your visitors with each direct mail delivery. The metrics are outlined below."

The **[!UICONTROL Delivery Overview]** presents key performance metrics (KPIs) offering in-depth insights into the interaction of your visitors with each direct mail delivery. The metrics are outlined below.

![](assets/global_report_direct_mail_delivery_overview.png){zoomable="yes"}{align="center"}

+++Learn more on Delivery overview metrics.

* **[!UICONTROL Messages to deliver]**: Total number of messages processed during the delivery preparation.

* **[!UICONTROL Delivered]**: Number of messages successfully sent, in relation to the total number of sent messages.

* **[!UICONTROL Errors]**: Total of errors cumulated during delivery and automatic return processing in relation to the total number of sent messages.

* **[!UICONTROL Unsubscribes]**: Number of recipients who clicked unsubscriptions.
+++

### Targeted audience {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_graph"
>title="Targeted audience"
>abstract="The recipient data and message information are displayed in the **Targeted audience** graph, reflecting the delivery preparation analysis."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_table"
>title="Targeted audience"
>abstract="The **Targeted audience** table provides a detailed breakdown of your recipients and the corresponding messages, based on the results of the delivery preparation process."

The table and graph for **[!UICONTROL Targeted Audience]** showcase data related to your recipients, with detailed metrics provided below.

![](assets/global_report_direct_mail_targeted_audience.png){zoomable="yes"}{align="center"}

+++Learn more on Targeted audience metrics.

* **[!UICONTROL Targeted audience]**: Total number of targeted recipients.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Exclusion]**: Total number of addresses ignored during the analysis when applying rules: address missing, quarantined, on denylist, etc.

+++

### Delivery statistics {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_graph"
>title="Delivery statistics"
>abstract="The **Delivery statistics** graph provides insights into the effectiveness of your Direct mail deliveries, including successful deliveries and any encountered errors."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_table"
>title="Delivery statistics"
>abstract="The **Delivery statistics** table details the success of your Direct mail delivery, and errors that occurred."

The **[!UICONTROL Delivery statistics]** graph and table provide a breakdown of the success of every direct mail delivery, with detailed metrics outlined below.

+++Learn more on Delivery statistics metrics.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

* **[!UICONTROL Errors / Bounces]**: Total number of errors cumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

* **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (user unknown, invalid domain) in relation to the number of messages to be delivered.

+++

### Causes of exclusion {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusions_direct_mail_table"
>title="Exclusions"
>abstract="The **Causes of exclusion** table displays a detailed breakdown, by rule, of messages that were rejected during the delivery preparation process."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_causes_exclusion_direct_mail_graph"
>title="Causes of exclusion"
>abstract="The **Causes of exclusion** graph illustrates the distribution of rejected messages during the preparation for delivery, categorized by each rule."

![](assets/global_report_direct_mail_exclusions.png){zoomable="yes"}{align="center"}

The Exclusions graph and table illustrate the reasons that prevented user profiles, excluded from the targeted profiles, from receiving the message.

+++Learn more on Causes of exclusion metrics.

* **[!UICONTROL Address in quarantine]**: Error type generated when address is placed in quarantine.

* **[!UICONTROL Address not specified]**: Error type generated when sending a delivery to indicate that the address does not exist.

* **[!UICONTROL Bad quality address]**: Error type generated when postal address quality rating is too low.

* **[!UICONTROL Denylisted address]**: Error type generated when the recipient was denylisted when the delivery was performed.

* **[!UICONTROL Double]**: Error type generated when the recipient was excluded because its keys values were not unique.

* **[!UICONTROL Control group]**: The recipient's address is part of the control group.

* **[!UICONTROL Target limited in size]**: The maximum delivery size was reached for the recipient.

+++
