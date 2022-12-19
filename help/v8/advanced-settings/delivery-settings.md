---
audience: end-user
title: Advanced Settings
description: Campaign v8 Web documentation
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
---
# Advanced settings {#advanced-settings}

>[!NOTE]
>
>This documentation is under construction and frequently updated. The final version of this content will be ready in January 2023.

These settings are technical delivery parameters that are defined in the email template. If you want to modify any of them for a specific delivery, proceed with caution.

## Email delivery settings {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

All the technical delivery parameters from the template.
Only change parameters, no creation here. 
According to permissions
Practionners should not modify this, caution. Only check and change typology rule -> rest defined in template

## Typology {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typology"
>abstract="Typology lets you control, filter and monitor the sending of deliveries."

Typologies are sets of typology rules, that are executed during the message analysis phase. They allow you to make sure your emails always contain certain elements (such as an unsubscription link or a subject line) or filtering rules to exclude groups from your intended target (like unsubscribers, competitors, or non-loyalty customers).

When associating a typology with a message or message template, the typology rules included in the typology will be executed to check the message validity.

### Pressure parameters {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Delivery weight"
>abstract="Delivery weights let you identify top-priority deliveries within the framework of pressure management. Messages with the highest weight have priority."

In this section, pressure parameters let you define a threshold. This is the maximum number of messages that can be sent to one profile over a given period. Once this threshold has been reached, no more deliveries can take place until the end of the period considered. This process lets you automatically exclude a profile from a delivery if a message exceeds the set threshold, thus avoiding over-solicitation.

Threshold values can be either constant or variable. This means that for a given period, thresholds can vary from one profile to another, or even for the same profile.

In the **Weight type** field, three options are available:

The **Delivery weight** field lets you

The **Delivery mode** field..

### Capacity settings {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importance of the recipient"
>abstract="The importance of the recipient is a formula used to determine which recipients are kept when the capacity typology rules are exceeded."

In this section, you can select a capacity rule defined in the Adobe Campaign v8 Console. This rule is associated to the email channel.

The **importance of the recipient** field is a formula used to determine which recipients are kept when the capacity typology rules are exceeded.

## Audience {#audience}

In this section, you can choose a target mapping defined in the Adobe Campaign v8 console. Target mapping creation is necessary in the case you use a recipient table other than the one provided by Adobe Campaign.

## Delivery {#delivery}

Test SMTP delivery: use this option to test sending via SMTP. The delivery is processed up to connection to the SMTP server but is not sent: for every recipient of the delivery, Campaign connects to the SMTP provider server, executes the SMTP RCPT TO command, and closes the connection before the SMTP DATA command.

Email BCC: use this option to store emails on an external system through BCC by simply adding a BCC email address to your message target.

### Retries {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Maximum number of retries"
>abstract="If a message fails due to a temporary error, retries will be performed during the delivery duration."

Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. One retry per day is programmed after that and until the delivery deadline, which is defined in the Validity tab.

## Approval {#approval}

**Manual**

**Semi-Automatic**

**Automatic**

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Approval mode"
>abstract="Each step of a delivery can be subject to approval in order to ensure full monitoring and control of the various processes."

## Validity {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Delivery duration"
>abstract="The Delivery duration field lets you enter the limit for global delivery retries. This means that Adobe Campaign sends the messages beginning on the start date, and then, for messages returning an error only, regular, configurable retries are performed until the validity limit is reached."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, mainly for the mirror page and images. The resources on this page are valid for a limited time."


The Delivery duration field lets you enter the limit for global delivery retries. This means that Adobe Campaign sends the messages beginning on the start date, and then, for messages returning an error only, regular, configurable retries are performed until the validity limit is reached.

You can also choose to specify dates. To do this, select Explicitly set validity dates. In this case, the delivery and validity limit dates also let you specify the time. The current time is used by default, but you can modify this directly in the input field.

Validity limit of resources: The Validity limit field is used for uploaded resources, mainly for the mirror page and images. The resources on this page are valid for a limited time (to save disk space).

### Mirror page management {#mirror}

**Mirror page management**

### Tracking {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking will be activated on the URLs."

**Tracking validity limit**: This option defines the duration for which the tracking will be activated on the URLs.

**Substitution URL for expired URLs**: TBC


## Test Settings{#test-setttings}

**Keep double**

**Keep denylisted addresses**

**Keep quarantined addresses**

**Keep the delivery code for the proof**

**Label prefix**