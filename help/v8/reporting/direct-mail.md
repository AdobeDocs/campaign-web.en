---
audience: end-user
title: Direct mail reports
description: Learn how to access and use Direct mail reports
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
---
# Direct mail delivery report {#direct-mail-report}

The **Direct mail delivery report** provides comprehensive insights and data specific to your Direct mail delivery. It includes detailed information on the performance, effectiveness, and outcomes of individual deliveries, offering a complete overview.

## Delivery summary {#delivery-summary-direct-mail}

### Delivery overview {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="Delivery overview"
>abstract="The **Delivery Overview** presents key performance metrics (KPIs) offering in-depth insights into the interaction of your visitors with each direct mail delivery. The metrics are outlined below."

The **[!UICONTROL Delivery Overview]** provides detailed insights into visitor interactions with each direct mail delivery, showcasing essential key performance metrics (KPIs). The metrics are outlined below.

![](assets/direct-overview.png){zoomable="yes"}{align="center"} [Delivery overview metrics graph showing key performance indicators for direct mail delivery.]

+++Learn more on Delivery overview metrics.

* **[!UICONTROL Messages to deliver]**: Total number of messages processed during delivery preparation.
* **[!UICONTROL Targeted]**: Number of user profiles qualifying as target profiles for direct mail messages.
* **[!UICONTROL To exclude]**: Number of user profiles excluded from the targeted profiles who will not receive direct mail messages.
+++

### Initial target population {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="Initial target population"
>abstract="The **Initial target population** graph displays data relative to your recipients and messages, based on the results of the delivery preparation."

The **[!UICONTROL Initial target population]** graph displays data related to recipients. Metrics are calculated during delivery preparation and include the initial audience, the number of messages to send, and the number of recipients excluded.

![](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"} [Initial target population graph showing audience size, messages to send, and exclusions.]

Mouse over a portion of the graph to display the exact number.

![](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"} [Detailed view of the initial target population graph with hover functionality.]

+++Learn more on Direct mail delivery report metrics.

* **[!UICONTROL Initial audience]**: Total number of targeted recipients.
* **[!UICONTROL To deliver]**: Total number of messages to be delivered after delivery preparation.
* **[!UICONTROL Exclusion]**: Total number of recipients excluded from the target population.
+++

### Delivery statistics {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="Delivery statistics"
>abstract="The **Delivery statistics** graph details the success of your Direct mail delivery, and errors that occurred."

The **[!UICONTROL Delivery statistics]** graph provides an overview of delivery performance, offering detailed metrics to measure success and effectiveness.

![](assets/direct-mail-delivery-stats.png){zoomable="yes"} [Delivery statistics graph showing success rates, errors, and quarantines.]

+++Learn more on Direct mail campaign report metrics.

* **[!UICONTROL Message sent]**: Total number of messages to be delivered after delivery preparation.
* **[!UICONTROL Success]**: Number of messages processed successfully compared to the number of messages to be delivered.
* **[!UICONTROL Errors]**: Total number of errors accumulated during deliveries and automatic rebound processing compared to the number of messages to be delivered.
* **[!UICONTROL New quarantines]**: Total number of addresses quarantined following failed delivery (e.g., user unknown, invalid domain) compared to the number of messages to be delivered.
+++

### Causes of exclusion {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="Delivery Causes of exclusion"
>abstract="The **Causes of exclusion** graph illustrates the distribution of rejected messages during the preparation for delivery, categorized by each rule."

The **[!UICONTROL Causes of exclusion]** graph provides a breakdown of reasons for message rejection during delivery preparation. This breakdown is organized by various rules, offering a detailed view of factors contributing to message exclusion. Exclusion rules are detailed in the [Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}.

![](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"} [Causes of exclusion graph showing distribution of rejected messages by rule.]

+++Learn more on Causes of exclusion metrics.

* **[!UICONTROL Address in quarantine]**: Error type generated when an address is placed in quarantine.
* **[!UICONTROL Address not specified]**: Error type generated when an address does not exist.
* **[!UICONTROL Bad quality address]**: Error type generated when postal address quality rating is too low.
* **[!UICONTROL Denylisted address]**: Error type generated when the recipient was denylisted during delivery.
* **[!UICONTROL Double]**: Error type generated when the recipient was excluded due to non-unique key values.
* **[!UICONTROL Control group]**: The recipient's address is part of the control group.
* **[!UICONTROL Target limited in size]**: The maximum delivery size was reached for the recipient.
+++

### Exclusions {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="Exclusions"
>abstract="The **[!UICONTROL Exclusions]** table displays a detailed breakdown, by rule, of messages that were rejected during the delivery preparation process."

The **[!UICONTROL Exclusions]** table provides a detailed breakdown, categorized by specific rules, of messages rejected during delivery preparation. This breakdown offers a clear understanding of the reasons behind message exclusions.

![](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"} [Exclusions table showing detailed breakdown of rejected messages by rule.]

Metrics available are the same as for the [Causes of exclusion](#direct-mail-delivery-exclusions) described above.