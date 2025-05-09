---
title: Key Performance Indicators
description: Learn how understand Key Performance Indicators
exl-id: 4b182219-100b-4101-919b-b0b770dd8515
---
# Key Performance Indicators {#kpis}

>[!CONTEXTUALHELP]
>id="acw_homepage_kpi"
>title="Key performance indicators"
>abstract="The **Key performance indicators** section lets you check your platform effectiveness through common KPIs."

<!-- à enlever? -->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="Spam KPI"

Browse to the home page to check key performance indicators for your platform. These indicators show the number and percentage of messages delivered, opened, clicked, unsubscriptions, and error rates.

Metrics are calculated for deliveries sent over the previous seven days by default. You can change the period from the drop-down list in the upper-right section of the card. Messages sent to test profiles are excluded.

You can select the channel to display. By default, these indicators reflect metrics for the email channel.

![Screenshot showing the KPI card with metrics for the email channel.](assets/kpi.png){zoomable="yes"} 

## Message delivered {#ui-delivered-kpi} 

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Delivered"
>abstract="This metric shows, for the selected channel, the sum of all messages processed with success, and the percentage of messages delivered with success compared to the total number of messages sent."

The number of messages delivered reflects your deliverability rate. It can never be 100% for the following reasons: some addresses or phone numbers can be wrong, spam blockers at email providers may reject your messages, or deliverability issues can happen.

The **Delivered** indicator shows the following KPIs for each channel:

* Percentage of the number of messages delivered with success compared to the total number of messages sent.

* Sum of all messages processed with success.

In Adobe Campaign, the rule to mark a message as 'Delivered' is:

Count of messages for which the "seed address" field equals "No" and with a status equal to "Taken into account by the service provider" (for SMS), "Sent" (for Emails), or "Received on the mobile" (for Push notifications).

## Total opens {#ui-open-kpi} 

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Opens"
>abstract="This metric shows, for the selected channel, the sum of all messages opened, and the percentage of messages opened compared to the total number of messages delivered with success."

Total opens are calculated by tracking the total number of times a message is opened, regardless of how many individual recipients generate those opens. This indicator is only available for emails.

The **Opens** indicator shows the following KPIs for each channel:

* Percentage of the number of messages opened compared to the total number of messages delivered with success.

* Sum of all messages opened, per channel.

Adobe Campaign detects message opens when the recipient downloads the images in the email. HTML and Multipart/Alternative emails include a 0-pixel image, which enables you to detect messages that have been opened. Since messages in text format do not include any images, it is impossible to detect whether they have been opened. Values calculated based on message opens are always estimates due to the error margin linked to image display.

## Click-through rate {#ui-click-kpi} 

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Clicks"
>abstract="This metric shows, for the selected channel, the sum of all URLs clicked in messages, and the percentage of clicks compared to the total number of messages delivered with success."

Add URLs in your message content to redirect recipients to a particular page. The click-through rate measures the number and percentage of recipients who clicked on a link in the message.

The **Clicks** indicator shows the following KPIs for each channel:

* Percentage of the number of clicks compared to the total number of messages delivered with success. 

* Number of distinct people who clicked at least once in a delivery. Unsubscription links and links to the email mirror page are excluded.

These metrics are based on the Consolidated tracking table (`nms:trackingStats`). This aggregate table is used for performance reasons when displaying reports, instead of the Recipient tracking logs table (`nms:trackingLogRcp`). It is not calculated in real-time. The table is generated a few minutes after the tracking logs are retrieved.

## Subscription rates {#ui-sub-kpi} 

>[!CONTEXTUALHELP]
>id="acw_keyindicators_subscriptions"
>title="Subscriptions"
>abstract="This metric shows, for the selected channel, the sum of all subscriptions to a service, and the percentage of subscriptions compared to the total number of messages delivered with success."

Recipients can opt in to Email and SMS communications.

The **Subscriptions** indicator shows the following KPIs for each channel:

* Percentage of the number of subscriptions compared to the total number of messages delivered with success.

>[!NOTE]
>
> Subscription and unsubscription KPIs vary based on the service type. For instance, email subscriptions and unsubscriptions encompass all email-related services, whether they result from manual actions or web forms. It's important to distinguish this approach from the delivery-level unsubscription metric, which tracks unsubscription link clicks rather than actual unsubscribed users.

## Unsubscription rates {#ui-unsub-kpi} 

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Unsubscriptions"
>abstract="This metric shows, for the selected channel, the sum of all unsubscriptions from a service, and the percentage of unsubscriptions compared to the total number of messages delivered with success."

Recipients must be able to opt out from Email and SMS through a dedicated unsubscription link in the email content or by replying STOP to an SMS.

The **Unsubscriptions** indicator shows the following KPIs for each channel:

* Percentage of the number of unsubscriptions compared to the total number of messages delivered with success.

* Sum of all clicks to an unsubscription link, meaning with a URL category equal to "Opt-out."

>[!NOTE]
>
> Subscription and unsubscription KPIs vary based on the service type. For instance, email subscriptions and unsubscriptions encompass all email-related services, whether they result from manual actions or web forms. It's important to distinguish this approach from the delivery-level unsubscription metric, which tracks unsubscription link clicks rather than actual unsubscribed users.

## Error rates {#ui-error-kpi} 

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Errors"
>abstract="Total number of errors cumulated during deliveries and automatic bounce processing. The associated rate is the ratio with the number of messages to be delivered."

Some messages sent by your Adobe Campaign platform might not reach their destination. It can happen when the user address or phone has typos, if the recipient changed their email address, or if their mailbox is full. If a message cannot be sent to a profile, the remote server automatically sends an error message to Adobe Campaign. This error is qualified to determine whether the email address, phone number, or device should be quarantined.

Check and update your database regularly, and ensure all profiles are active and real. Delivery errors can be temporary or permanent—soft or hard bounce—depending on why the message was not delivered.

The **Errors** indicator shows the following KPIs for each channel:

* Percentage of the number of errors compared to the total number of messages to be delivered.

* Total number of errors cumulated during deliveries and automatic rebound processing.

## Message sent {#ui-sent-kpi} 

<!--DRAFT - This section requires a validation-->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_sent"
>title="Sent"
>abstract="This metric shows, for the direct mail channel, the sum of all messages sent, and the percentage of messages sent to the provider, compared to the total number of messages prepared during the delivery preparation phase."

During the preparation phase, the direct mail extraction file is generated, but information concerning recipients (delivery logs) is not updated. The status of a delivery moves from Pending delivery to Sent when the Campaign user confirms the sending of the delivery. Then the delivery is set to Finished.

It can never be 100% of messages sent compared to the total of messages prepared, as some addresses can be missing or incomplete.

The **Sent** indicator shows the following KPIs for the Direct mail channel:

* Percentage of the number of messages sent compared to the total number of messages prepared.

* Sum of all messages sent.