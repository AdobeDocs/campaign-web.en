---
title: Campaign v8 Web User Interface previous Release Notes
description: 2024 Campaign Web User Interface releases
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
---
# 2024 release notes {#2024-release}

This page lists all changes and improvements available with **2024 releases**. Latest release notes are available on [this page](release-notes.md).

## October '24 release {#24-10-release}

**Release date**: Oct 29, 2024

The following features and improvements are available starting October release.

### Features

<table>
<thead>
<tr>
<th><strong>External accounts</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now set up and manage external accounts directly through Adobe Campaign Web User Interface. This feature simplifies the configuration of different types of external accounts, such as bounce emails (POP3) or execution instances.</p>
<p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Transactional messaging</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Transactional messaging (Message Center) is now available in the Campaign web user interface. This add-on triggers messages generated from events in information systems, such as invoices, order confirmations, shipping confirmations, password changes, product unavailability notifications, account statements, and website account creations.</p>
<p>For more information, refer to the <a href="../transactional-messaging/transactional.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

### Improvements

* **Workflow activities** - Move an activity and all its child nodes from one transition to another within a workflow. Use the dedicated **Move** button in the activity's properties pane. [Learn more](../workflows/orchestrate-activities.md#move)

* **Workflow enrichment activity**
    * Define an Alias and a Label when creating a new field in the **Enrichment** activity. [Learn more](../workflows/activities/enrichment.md#collection-settings)
    * Add offers for each profile in the **Enrichment** activity. [Learn more](../workflows/activities/enrichment.md##add-offers)

* **Distribution of values** - Check how values are distributed for each field when accessing the list of fields for personalization. A popup window shows the number and percentage for each value. [Learn more](../query/build-query.md#distribution-values-query)

* **Version and system info** - Access details about your instance versions for both the client console and the Web User Interface. This section also lists all built-in packages installed in your environment. [Learn more](../get-started/user-interface.md#user-interface-about)

* **Lists** - Reorder the values of a list easily. [Learn more](../get-started/work-with-folders.md)

* **Delivery** - Delivery variables are now accessible from personalization fields. [Learn more](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)

## September updates {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI Assistant</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Optimize your crafted and tailored messages with the AI Assistant in Adobe Campaign Web. This tool generates engaging text, main titles, and visually appealing images to enhance your content.</p>
<p>Explore its features firsthand with <a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">our live feature preview</a>.</p>
<p>For more information, refer to the <a href="../email/generative-gs.md">detailed documentation</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif" alt="AI Assistant generating engaging content"/>
<p>Availability date: Sept 12</p>
</td>
</tr>
</tbody>
</table>

## August release {#24-8-release}

**Release date**: Sept 3, 2024

The following features and improvements are available starting August release.

* **SMTP parameters** - Access SMTP settings in the email delivery settings. [Learn more](../advanced-settings/delivery-settings.md#smtp)

* **Global variables** - Define global variables to set values for your deliveries. [Learn more](../advanced-settings/delivery-settings.md#variables-delivery)

### New features in Limited Availability {#acs-24-8}

>[!AVAILABILITY]
>
>The following capabilities are in Limited Availability (LA). They are restricted to customers migrating **from Adobe Campaign Standard to Adobe Campaign v8**, and cannot be deployed on any other environment.
>
>Refer to the following documentation pages: [Campaign Standard transition to Campaign v8](../rn/acs-migration.md) and [Features for Campaign Standard users](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"}.

* **Branding for Direct Mail** - Technical administrators can define one or several brands to centralize parameters affecting a brand's identity, such as the brand logo, domain of landing pages' access URL, or message tracking settings. Link these brands to messages or landing pages. [Learn more](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **Subscriptions with Landing pages** - Link a landing page to a service and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Visual fragments** - Archive visual content fragments. [Learn more](../content/create-fragment.md#archive)

* **Captcha in landing pages** - Add captcha to protect your landing page from spam and abuse caused by bots. This feature is non-intrusive for customers and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->

[Continue reading for additional release notes...]