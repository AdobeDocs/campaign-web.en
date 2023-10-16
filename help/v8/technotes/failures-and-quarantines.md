---
title: Failures and quarantines
description: Understand and monitor failures and quarantines in Adobe Campaign Web 
badge: label="Beta" 
---
# Failures and quarantines {#failures-quarantines}

## Quarantine management {#quarantines}

Adobe Campaign manages a list of quarantined addresses for online channels (email, SMS, push notifications). Some service providers automatically consider messages as spam if the rate of invalid addresses is too high. Quarantine therefore allows you to avoid being added to denylist by these providers. Moreover, quarantines help reducing SMS sending costs by excluding erroneous phone numbers from deliveries.

When their address or phone number is quarantined, recipients are excluded from the target during delivery preparation. If those quarantined addresses are present in lists, they are also excluded when sending to those lists. An email address can be quarantined, for example, when the mailbox is full, if the address does not exist, or if the email server is unavailable.

**Quarantine** applies only to an **address**, a **phone number**, or a **device token**, but not to the profile itself. For example, a profile whose email address is quarantined can update their profile and enter a new address, and could then be targeted by delivery actions again. Likewise, if two profiles happen to have the same phone number, they will both be affected if the number is quarantined. The quarantined addresses or phone numbers are displayed in the [exclusion logs](#delivery-quarantines) (for a delivery) or in the [quarantine list](#non-deliverable-bounces) (for the entire platform).

On the other hand, profiles can be on the **denylist** as after an unsubscription (opt-out), for a given channel. When a profile on the denylist for the email channel has two email addresses, both addresses are excluded. You can check if a profile is on the denylist for one or more channels in the **[!UICONTROL No longer contact]** section of the profile. [Learn more](../audience/about-recipients.md)


### Quarantine process {#quarantine-reason}

Adobe Campaign manages quarantine according to the type of delivery failure and its reason. These are assigned during error messages qualification [as described below](#delivery-failures).

Two types or errors can be captured:

* **Hard error**: the email address, phone number or device is immediately sent to quarantine.
* **Soft error**: soft errors increment an error counter, and might quarantine an email, phone number or device token. Campaign performs [retries](#retries): when the error counter reaches the limit threshold, the address, phone number or device token is quarantined. 

In the list of quarantined addresses, the **[!UICONTROL Error reason]** field indicates why the selected address was placed in quarantine. [Learn more](#identifying-quarantined-addresses-for-the-entire-platform).

If a user qualifies an email as a spam,  or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined as **[!UICONTROL Denylisted]**. Their profile is updated accordingly. This status refers to the address or phone number only: the profile is not on the denylist, and can still receive push notifications for example. 

## Access quarantined addresses {#access-quarantined-addresses}

Quarantine addresses are listed during the delivery preparation phase, in the delivery logs of the delivery dashboard.

For each delivery, you can also check the **[!UICONTROL Delivery summary]** report: it shows the number of addresses in quarantine in the delivery target, and displays:

* The number of addresses placed in quarantine during the delivery analysis,
* The number of addresses placed in quarantine following the delivery action.

Learn more about the Delivery Summary report in [this page](../reporting/email-report.md#delivery-summary).


### Remove a quarantined address {#remove-a-quarantined-address}

Addresses that match specific conditions are automatically deleted from the quarantine list by the **Database cleanup** built-in workflow.

The addresses are automatically removed from the quarantine list in the following cases:

* Addresses in a **[!UICONTROL With errors]** status will be removed from the quarantine list after a successful delivery.
* Addresses in a **[!UICONTROL With errors]** status will be removed from the quarantine list if the last soft bounce occurred more than 10 days ago. For more on soft error management, see [this section](#soft-error-management).
* Addresses in a **[!UICONTROL With errors]** status that bounced with the **[!UICONTROL Mailbox full]** error will be removed from the quarantine list after 30 days.

Their status then changes to **[!UICONTROL Valid]**.

>[!CAUTION]
>
>Recipients with an address in a **[!UICONTROL Quarantine]** or **[!UICONTROL Denylisted]** status are never removed, even if they receive an email. 

You can also manually remove an address from the quarantine list. The procedure is described in the [Adobe Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#remove-a-quarantined-address)


## Understand delivery failures {#delivery-failures}

If a message cannot be sent to a profile, the remote server automatically sends an error message to Adobe Campaign. This error is qualified to determine whether the email address, phone number or device should be quarantined. See [Bounce mail management](#bounce-mail-qualification).

Once a message is sent, you can view the delivery status for each profile and the associated failure type and reason in the delivery logs.

When an email address is quarantined, or if a profile is on denylist, the recipient is excluded at the delivery preparation step. Excluded messages are listed in the delivery dashboard.

### Email channel {#email-failures}

#### Failure reasons {#delivery-failure-reasons}

Bounces are the result of a delivery attempt and failure where the Internet Service Provider (ISP) provides back failure notices. After a given email has bounced several times in a row, this process flags it for suppression. This mechanism prevents systems from continuing to send invalid email addresses. Bounces are one of the key pieces of data that ISPs use to determine IP reputation. Keeping an eye on this metric is important. "Delivered" versus "bounced" is probably the most common way of measuring the delivery of marketing messages: the higher the delivered percentage is, the better.

There are two types of error when a message fails. Each delivery failure type determines if an address is sent to [quarantine](quarantines.md#quarantine-reason) or not.

* **Hard bounces**
  Hard bounces are permanent failures generated after an ISP determines a mailing attempt to a subscriber address as not deliverable. Within Adobe Campaign, hard bounces that are categorized as undeliverable are added to the quarantine list, which means they wouldn't be reattempted. There are some cases where a hard bounce would be ignored if the cause of the failure is unknown.
  
  Here are some common examples of hard bounces: Address doesn't exist, Account disabled, Bad syntax, Bad domain

* **Soft bounces**
  Soft bounces are temporary failures that ISPs generate when they have difficulty delivering mail. Soft failures will [retry](#retries) multiple times (with variance depending on use of custom or out-of-box delivery settings) in order to attempt a successful delivery. Addresses that continually soft bounce will not be added to quarantine until the maximum number of retries has been attempted (which again vary depending on settings). 
  
  Some common causes of soft bounces include the following: Mailbox full, Receiving email server down, Sender reputation issues

The  **Ignored** type of error is known to be temporary, such as "Out of office", or a technical error, for example if the sender type is "postmaster".

The feedback loop operates like bounce emails: when a user qualifies an email as spam, you can configure email rules in Adobe Campaign to block all deliveries to this user. The addresses of these users are denylisted even though they did not click the unsubscription link. Addresses are added to the (**NmsAddress**) quarantine table and not to the (**NmsRecipient**) recipient table with the **[!UICONTROL Denylisted]** status. Learn more about feedback loop mechanism in the [Adobe Deliverability Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops).

#### Synchronous and asynchronous errors {#synchronous-and-asynchronous-errors}

A message delivery can fail immediately, in that case we qualify this as a **synchronous** error. If message sending fails or later on, after it has been sent, the error is **asynchronous**.

* For the **synchronous errors**, the remote server contacted by the Adobe Campaign delivery server immediately returns an error message. The delivery is not allowed to be sent to the profile's server. The Mail Transfer Agent (MTA) determines the bounce type and qualifies the error, and sends back that information to Campaign in order to determine whether the email addresses concerned should be quarantined. See [Bounce mail qualification](#bounce-mail-qualification). 

* For **asynchronous error**, a bounce mail or a SR is resent later by the receiving server. This error is qualified with a label related to the error. Asynchronous errors can occur up until one week after a delivery has been sent.


#### Retries {#retries}

Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. 


#### Validity period

The **Delivery duration** field of your [delivery properties](../advanced-settings/delivery-settings.md#validity) lets you enter the limit for global delivery retries. This means that Adobe Campaign sends the messages beginning on the start date, and then, for messages returning an error only, regular, configurable retries are performed until the validity limit is reached.

You can also choose to specify dates. To do this, select **Explicitly set validity dates**. In this case, the delivery and validity limit dates also let you specify the time. The current time is used by default, but you can modify this directly in the input field.

**Resources Validity limit** is used for uploaded resources, mainly for the mirror page and images. The resources on this page are valid for a limited time (to save disk space). After this limit, these resources are no longer available.

#### Error types {#email-error-types}

For the email channel, possible reasons for a delivery failure are listed available in [Adobe Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

### Push notifications quarantines {#push-error-types}

For the push channel, possible reasons for a delivery failure are listed available in [Adobe Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

### SMS quarantines

For the SMS channel, possible reasons for a delivery failure are listed available in [Adobe Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.
