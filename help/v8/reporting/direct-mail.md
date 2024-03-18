---
audience: end-user
title: Direct mail reports
description: Learn how to access and use Direct mail reports
---
# Direct mail delivery report {#direct-mail-report}

The **Direct mail delivery report** offers comprehensive insights and data specific to your Direct mail delivery. It provides detailed information on the performance, effectiveness, and outcomes of your individual deliveries, providing you with a comprehensive overview.

## Delivery summary {#delivery-summary-direct-mail}

### Delivery overview {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="Delivery overview"
>abstract="The **Delivery Overview** presents key performance metrics (KPIs) offering in-depth insights into the interaction of your visitors with each direct mail delivery. The metrics are outlined below."

The **[!UICONTROL Delivery Overview]** provides detailed insights into how your visitors interact with each direct mail delivery, showcasing essential key performance metrics (KPIs).  The metrics are outlined below.

![](assets/direct-overview.png){zoomable="yes"}{align="center"}

+++Learn more on Delivery overview metrics.

* **[!UICONTROL Messages to deliver]**: Total number of messages processed during the delivery preparation.

* **[!UICONTROL Targeted]**: Number of user profiles who qualify as target profiles for your direct mail messages.

* **[!UICONTROL To exclude]**: Number of user profiles, excluded from the targeted profiles, who will not receive your direct mail messages.
+++

### Initial target population {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="Initial target population"
>abstract="The **Initial target population** graph displays data relative to your recipients and messages, based on the results of the delivery preparation."

The **[!UICONTROL Initial target population]** graph displays data relative to your recipients. Metrics are calculated during delivery preparation and show: the initial audience, the number of messages to send, the number of recipients excluded.

![](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"}

Mouse-over a portion of the graph to display the exact number.

![](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"}

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

The **[!UICONTROL Delivery statistics]** graph provides a comprehensive overview of your delivery performance, offering detailed metrics to gauge success and effectiveness.

![](assets/direct-mail-delivery-stats.png){zoomable="yes"}

+++Learn more on Direct mail campaign report metrics.

* **[!UICONTROL Message sent]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

* **[!UICONTROL Errors]**: Total number of errors cumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

* **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (user unknown, invalid domain) in relation to the number of messages to be delivered.

+++

### Causes of exclusion {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="Delivery Causes of exclusion"
>abstract="The **Causes of exclusion** graph illustrates the distribution of rejected messages during the preparation for delivery, categorized by each rule."

The **[!UICONTROL Causes of exclusion]** graph  provides a detailed breakdown of the reasons behind messages being rejected during the process of delivery preparation. This breakdown is organized according to various rules, offering a comprehensive view of the factors contributing to message exclusion. Exclusion rules are detailed in the [Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}.

![](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

+++Learn more on Causes of exclusion metrics.

* **[!UICONTROL Address in quarantine]**: Error type generated when address is placed in quarantine.

* **[!UICONTROL Address not specified]**: Error type generated when sending a delivery to indicate that the address does not exist.

* **[!UICONTROL Bad quality address]**: Error type generated when postal address quality rating is too low.

* **[!UICONTROL Denylisted address]**: Error type generated when the recipient was denylisted when the delivery was performed.

* **[!UICONTROL Double]**: Error type generated when the recipient was excluded because its keys values were not unique.

* **[!UICONTROL Control group]**: 

* **[!UICONTROL Target limited in size]**: 

+++

### Exclusions {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="Exclusions"
>abstract="The **Causes of exclusion** table displays a detailed breakdown, by rule, of messages that were rejected during the delivery preparation process."

The **[!UICONTROL Exclusions]** table provides an in-depth breakdown, categorized by specific rules, of messages that were rejected during the preparation phase of delivery. This comprehensive breakdown allows for a clear understanding of the reasons behind the exclusion of these messages from the delivery process.

![](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

Metrics available are the same as for the [Causes of exclusion](#direct-mail-delivery-exclusions) described above.
