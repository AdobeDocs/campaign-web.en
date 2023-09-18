---
audience: end-user
title: Campaign reports
description: Learn how to access and use campaign reports
badge: label="Beta" 
---
# Campaign reports {#campaign-reports}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="Reporting Sending"
>abstract="The Sending tab within your report provides in-depth insights into your visitors' interactions with your deliveries and any potential errors they may have encountered."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="Reporting tracking"
>abstract="The Sending tab within your report offers valuable data, including recipient behavior per link, breakdown of opens and clicks, as well as detailed information about the most frequently clicked URLs during a delivery."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Delivery overview"
>abstract="The Delivery Overview provides key performance indicators (KPIs) that give detailed information about how your visitors engage with your email delivery."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Initial target audience statistics"
>abstract="The Initial target audience statistics table displays data relative to your recipients"

The Campaign report is divided into different widgets detailing your campaign’s success and errors.

The Campaign report page will be displayed with the following tabs:

* [Email channel](#email-channel) 
* [SMS channel](#sms-channel)
* [Push channel](#push-channel)

To access your Campaign report, click Reports from your campaign's dashboard.

![](assets/campaign_report_email_13.png) 

## Email channel {#email-channel}

### Delivery summary {#delivery-summary-email}

* **[!UICONTROL Delivery Overview]** provides key performance indicators (KPIs) that give detailed information about how your visitors engage with your email delivery.

    ![](assets/campaign_report_email_1.png) 

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL Total sent]**: Total number of messages processed during the delivery analysis.

    * **[!UICONTROL Delivered]**: Number of messages successfully sent, in relation to the total number of sent messages.

    * **[!UICONTROL Bounces]**: Total of errors cumulated during delivery and automatic return processing in relation to the total number of sent messages.

    * **[!UICONTROL Distinct opens]**: Total number of targeted recipients who opened a message at least once.

    * **[!UICONTROL Distinct clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

    +++

* **[!UICONTROL Initial target audience statistics]** table displays data relative to your recipients:

    ![](assets/campaign_report_email_2.png)

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL Initial audience]**: Total number of targeted recipients.

    * **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery analysis.

    * **[!UICONTROL Rejected by rules]**: Total number of addresses ignored during the analysis when applying rules: address missing, quarantined, on denylist, etc.

    +++

* **[!UICONTROL Execution statistics]** table details the success of your delivery.

    ![](assets/campaign_report_email_3.png)

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery analysis.

    * **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

    * **[!UICONTROL Errors]**: Total number of errors cumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

    * **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (user unknown, invalid domain) in relation to the number of messages to be delivered.

    +++

* **[!UICONTROL Reaction statistics]** table contains the available data for recipient activity for your delivery.

    ![](assets/campaign_report_email_4.png)

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL Distinct opens]**: Total number of targeted recipients who opened a message at least once.

    * **[!UICONTROL Opens]**: Number of distinct targeted recipients for this domain who have opened a message at least once.

    * **[!UICONTROL Unsubscriptions]**: Number of recipients who clicked unsubscriptions for the concerned period.

    * **[!UICONTROL Mirror page]**: Number of recipients who clicked on the mirror page link.

    * **[!UICONTROL Forwards]**:  Number of recipients who clicked who forwarded the email. 
    +++

* **[!UICONTROL Generated click streams]** table displays data relative to how your recipients interacted with your delivery.

    ![](assets/campaign_report_email_5.png) 

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL Distinct clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

    * **[!UICONTROL Clicks]**: Total number of clicks on links in deliveries.

    * **[!UICONTROL Reactivity]**: Ratio of the number of targeted recipients having clicked in a delivery, in relation to the estimated number of targeted recipients having opened a delivery.

    +++

### Non-deliverables {#non-deliverables-email}

* **[!UICONTROL Breakdown of errors per type]** and **[!UICONTROL Breakdown of errors per domain]** tables and graphs contain the available data for possible errors encountered with each domain.
    
    The errors shown in this report trigger the quarantine process. For more on quarantine management, refer to [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

    ![](assets/campaign_report_email_6.png)

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL User unknown]**: Error type generated during delivery to indicate that the email address is invalid.

    * **[!UICONTROL Invalid domain]**: Error type generated when sending a delivery to indicate that the domain of the email address is wrong or does not exist.

    * **[!UICONTROL Mailbox full]**: Error type generated after five delivery attempts to indicate that the recipients’ inbox contains too many messages.

    * **[!UICONTROL Account disabled]**: Error type generated when sending a delivery to indicate that the address no longer exists.

    * **[!UICONTROL Refused]**: Error type generated when an address is rejected by the IAP (Internet Access Provider), for instance following the application of a security rule (anti-spam software).

    * **[!UICONTROL Unreachable]**: Error type which occurs in the message distribution string: incident on the SMTP relay, domain temporarily unreachable, etc

    * **[!UICONTROL Not connected]**: Error type to indicate that the recipients’ mobile phone is switched off or disconnected from the network at the time of sending.

    +++

### Tracking indicators {#tracking-indicators-email}

* **[!UICONTROL Delivery statistics]** provides key performance indicators (KPIs) that give detailed information about data available for sent emails.

    ![](assets/campaign_report_email_7.png)

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

    * **[!UICONTROL Distinct opens]**: Total number of targeted recipients who opened a message at least once.

    * **[!UICONTROL Opens]**: Number of distinct targeted recipients for this domain who have opened a message at least once.

    * **[!UICONTROL Clicks on the opt-out link]**:  Number of clicks on the unsubscription link.

    * **[!UICONTROL Clicks on the mirror link]**: Number of clicks on the link to the mirror page.

    * **[!UICONTROL Estimation of forwards]**: Estimation of the number of emails forwarded by the targeted recipients. 
    +++

* **[!UICONTROL Initial target audience statistics]** table displays data relative to your recipients.

    ![](assets/campaign_report_email_8.png) 

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL Sent]**: Total number of messages sent.

    * **[!UICONTROL Complaints]**: Number of messages for this domain that have been reported as undesirable by the recipient.

    * **[!UICONTROL Opens]**: Number of distinct targeted recipients for this domain who have opened a message at least once.

    * **[!UICONTROL Clicks]**: Number of distinct targeted recipients who clicked in the same delivery at least once. 

    * **[!UICONTROL Raw reactivity]**: Percentage of the number of recipient who clicked in a delivery at least once compared to the number of recipients who opened a delivery at least once.
    +++

### URLs and click streams {#url-email}

* **[!UICONTROL URLs and click streams]** provides key performance indicators (KPIs) that give detailed information about the URLs that were clicked the most during a delivery.

    ![](assets/campaign_report_email_9.png)

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL Reactivity]**: Ratio of the number of targeted recipients having clicked in a delivery, in relation to the estimated number of targeted recipients having opened a delivery.

    * **[!UICONTROL Distinct clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

    * **[!UICONTROL Clicks]**: Total number of clicks on links in deliveries.

    * **[!UICONTROL Platform average]** : This average rate, displayed under each rate (reactivity, distinct clicks, and cumulated clicks), is calculated for deliveries sent over the previous six months. Only deliveries with the same typology and on the same channel are taken into account. Proofs are excluded.
    +++

* **[!UICONTROL Top 10 most visited links]** graph and table contain the available data for recipient behavior per link.

    ![](assets/campaign_report_email_10.png)

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL Clicks]**: Total number of clicks on links in deliveries.

    * **[!UICONTROL Percentage]**: Percentage of users who interacted with the delivery.

    +++

* **[!UICONTROL Breakdown of clicks over time]** graph contains the available data for recipient behavior per link.

    ![](assets/campaign_report_email_11.png)

### User Activities {#user-activities-email}

* **[!UICONTROL User activities]** shows the breakdown of opens and clicks in the form of a chart.

    ![](assets/campaign_report_email_12.png)

    +++Learn more on Email campaign report metrics.

    * **[!UICONTROL Clicks]**: Total number of clicks on links in deliveries.

    * **[!UICONTROL Opens]**: Number of distinct targeted recipients for this domain who have opened a message at least once.

    +++

## SMS channel {#sms-channel}

### Delivery summary {#delivery-summary-sms}

* **[!UICONTROL Delivery Overview]** provides key performance indicators (KPIs) that give detailed information about how your visitors engage with your SMS delivery.
    
    ![](assets/campaign_report_sms_1.png)

    +++Learn more on SMS campaign report metrics.

    * **[!UICONTROL Total sent]**: Total number of messages processed during the delivery analysis.

    * **[!UICONTROL Delivered]**: Number of messages successfully sent, in relation to the total number of sent messages.

    * **[!UICONTROL Errors]**: Total of errors cumulated during delivery and automatic return processing in relation to the total number of sent messages.

    * **[!UICONTROL Distinct clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

    +++

* **[!UICONTROL Initial target audience statistics]** table displays data relative to your recipients:

    ![](assets/campaign_report_sms_2.png)

    +++Learn more on SMS campaign report metrics.

    * **[!UICONTROL Initial audience]**: Total number of targeted recipients.

    * **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery analysis.

    * **[!UICONTROL Rejected by rules]**: Total number of addresses ignored during the analysis when applying rules: address missing, quarantined, on denylist, etc.

    +++

* **[!UICONTROL Execution statistics]** table details the success of your delivery:

    ![](assets/campaign_report_sms_3.png)

    +++Learn more on SMS campaign report metrics.

    * **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery analysis.

    * **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

    * **[!UICONTROL Errors]**: Total number of errors cumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

    * **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (user unknown, invalid domain) in relation to the number of messages to be delivered.

    +++

* **[!UICONTROL Generated click streams]** table displays data relative to how your recipients interacted with your delivery:

    ![](assets/campaign_report_sms_4.png)

    +++Learn more on SMS campaign report metrics.

    * **[!UICONTROL Distinct clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

    * **[!UICONTROL Clicks]**: Total number of clicks on links in deliveries.

    * **[!UICONTROL Reactivity]**: Ratio of the number of targeted recipients having clicked in a delivery, in relation to the estimated number of targeted recipients having opened a delivery.

    +++

## Push channel {#push-channel}

### Delivery summary {#delivery-summary-push}

* **[!UICONTROL Delivery Overview]** provides key performance indicators (KPIs) that give detailed information about how your visitors engage with your push notification delivery.
    
    +++Learn more on Push campaign report metrics.

    * **[!UICONTROL Total sent]**: Total number of messages processed during the delivery analysis.

    * **[!UICONTROL Delivered]**: Number of messages successfully sent, in relation to the total number of sent messages.

    * **[!UICONTROL Errors]**: Total of errors cumulated during delivery and automatic return processing in relation to the total number of sent messages.

    * **[!UICONTROL Distinct clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

    +++

* **[!UICONTROL Initial target audience statistics]** table displays data relative to your recipients:

    +++Learn more on Push campaign report metrics.

    * **[!UICONTROL Initial audience]**: Total number of targeted recipients.

    * **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery analysis.

    * **[!UICONTROL Rejected by rules]**: Total number of addresses ignored during the analysis when applying rules: address missing, quarantined, on denylist, etc.

    +++

* **[!UICONTROL Execution statistics]** table details the success of your delivery:

    +++Learn more on Push campaign report metrics.

    * **[!UICONTROL Message to deliver]**: Total number of messages to be delivered after delivery analysis.

    * **[!UICONTROL Success]**: Number of messages processed successfully in relation to the number of messages to be delivered.

    * **[!UICONTROL Errors]**: Total number of errors cumulated during deliveries and automatic rebound processing in relation to the number of messages to be delivered.

    * **[!UICONTROL New quarantines]**: Total number of addresses quarantined following a failed delivery (user unknown, invalid domain) in relation to the number of messages to be delivered.

    +++

* **[!UICONTROL Generated click streams]** table displays data relative to how your recipients interacted with your delivery:

    +++Learn more on Push campaign report metrics.

    * **[!UICONTROL Distinct clicks]**: Total number of distinct recipients who clicked in a delivery at least once.

    * **[!UICONTROL Clicks]**: Total number of clicks on links in deliveries.

    * **[!UICONTROL Reactivity]**: Ratio of the number of targeted recipients having clicked in a delivery, in relation to the estimated number of targeted recipients having opened a delivery.

    +++
