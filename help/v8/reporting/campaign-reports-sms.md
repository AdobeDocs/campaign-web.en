---
audience: end-user
title: Campaign reports for the SMS channel
description: Understand campaign reports for the SMS channel
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
---
# Campaign reports for the SMS channel {#campaign-reports-sms-channel}

Each campaign report is divided into different widgets detailing your campaign's success and errors. For the SMS channel, reports and metrics are detailed below. Learn how to access your campaign reports on [this page](campaign-reports.md).

## Delivery summary {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="Delivery overview"
>abstract="The **Delivery Overview** report provides key performance indicators (KPIs) that give detailed information about how your visitors engage with your SMS delivery."

The **[!UICONTROL Delivery Overview]** report provides key performance indicators (KPIs) that give detailed information about how your visitors engage with your SMS delivery. Metrics are detailed below.

![Delivery Overview report showing SMS metrics](assets/campaign_report_sms_1.png){zoomable="yes"}

+++Learn more about SMS campaign report metrics.

* **[!UICONTROL Total sent]**: Total number of messages processed during the delivery preparation.

* **[!UICONTROL Delivered]**: Number of messages successfully sent, in relation to the total number of sent messages.

* **[!UICONTROL Errors]**: Total of errors accumulated during delivery and automatic return processing, in relation to the total number of sent messages.

* **[!UICONTROL Distinct clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

+++

### Initial target audience statistics {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="Initial target audience statistics"
>abstract="The **Initial target audience statistics** table displays data relative to your recipients."

The **[!UICONTROL Initial target audience statistics]** table displays data relative to your recipients. Metrics are detailed below.

![Initial target audience statistics table showing recipient data](assets/campaign_report_sms_2.png){zoomable="yes"}

+++Learn more about SMS campaign report metrics.

* **[!UICONTROL Initial audience]**: Total number of targeted recipients.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Rejected by rules]**: Total number of addresses ignored during the analysis when applying rules, such as address missing, quarantined, or on denylist.

+++

### Execution statistics {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="Execution statistics"
>abstract="The **Execution statistics** table details the success of your delivery: messages to deliver, success, errors, and new quarantines."

The **[!UICONTROL Execution statistics]** table details the success of your delivery. Metrics are detailed below.

![Execution statistics table showing delivery success metrics](assets/campaign_report_sms_3.png){zoomable="yes"}

+++Learn more about SMS campaign report metrics.

* **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery preparation.

* **[!UICONTROL Success]**: Number of messages processed successfully, in relation to the number of messages to be delivered.

* **[!UICONTROL Errors]**: Total number of errors accumulated during deliveries and automatic rebound processing, in relation to the number of messages to be delivered.

* **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (user unknown, invalid domain), in relation to the number of messages to be delivered.

    SMS error types are listed in the [Adobe Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Generated click streams {#delivery-summary-sms-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="Generated click streams"
>abstract="The **Generated click streams** table shows the available data relative to how your recipients interacted with your delivery."

The **[!UICONTROL Generated click streams]** table displays data relative to how your recipients interacted with your delivery. Metrics are detailed below.

![Generated click streams table showing recipient interaction data](assets/campaign_report_sms_4.png){zoomable="yes"}

+++Learn more about SMS campaign report metrics.

* **[!UICONTROL Distinct clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

* **[!UICONTROL Clicks]**: Total number of clicks on links in deliveries.

* **[!UICONTROL Reactivity]**: Ratio of the number of targeted recipients having clicked in a delivery, in relation to the estimated number of targeted recipients having opened a delivery.

+++