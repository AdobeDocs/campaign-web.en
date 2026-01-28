---
title: Campaign v8 Web User Interface Release Notes
description: Discover new features coming with the latest Campaign Web User Interface release
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
---
# Release notes {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Release notes"
>abstract="Adobe Campaign Web user interface releases operate on a continuous delivery model which allows for a more scalable, phased approach to feature deployment. Accordingly, Campaign release notes get updated several times a month, with latest features, improvements, and fixes. We recommend you to check them regularly."

Adobe Campaign Web user interface releases operate on a continuous delivery model which allows for a more scalable, phased approach to feature deployment. Accordingly, these release notes get updated several times a month. Please check them regularly.

Changes and improvements available with previous releases are listed in the [2024](release-notes-24.md) and [2025](release-notes-25.md) pages.

## January '26 release {#26-1-release}

_Jan 27, 2026_

### New features {#26-1-features}

<table>
<thead>
<tr>
<th><strong>Multilingual delivery capabilities (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Multilingual delivery feature is now available to all customers (GA). This feature allows you to send multiple messages in different languages in Adobe Campaign Web User Interface. You can choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. 
<p>For more information, refer to the <a href="../msg/multilingual.md">detailed documentation</a>.</p>
<p>The following improvements have been made to multilingual push notifications:</p>
<ul>
<li>You can now quickly populate all language variants by uploading a CSV file containing your multilingual content. <a href="../msg/multilingual.md#csv-upload">Read more</a>
</li>
<li>Rich push notifications are now supported.</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Profile enrichment in Transactional Messages capability is now available to all customers (GA). In addition to emails, SMS and push notifications are now also supported. This feature allows you to personalize transactional messages by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>For more information, refer to the <a href="../transactional-messaging/profile-enrichment.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager live and langage copies</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Adobe Experience Manager content integration allows you to access all language and live copies created in Adobe Experience Manager directly within Campaign when building deliveries. You can refresh content in real-time to fetch the latest Adobe Experience Manager versions. This integration eliminates manual content synchronization between Adobe Experience Manager and Campaign, streamlining your multi-language campaign workflow.</p>
<p>For more information, refer to the <a href="../integrations/aem-multilingual.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Content experiments - A/B testing</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Content experiments in Adobe Campaign Web allow you to define multiple A/B testing delivery variants in order to measure which performs best for your target audience. You can vary the delivery content, subject, or sender to test different versions and determine which variant produces the best results. You can conduct A/B tests on various email elements such as subject line, sender name and email body content.</p>
<p>For more information, refer to the <a href="../email/ab-testing.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Continuous delivery activity allows you to add new recipients to an existing delivery. This delivery type avoids having to create a new delivery each time, making it more efficient for low-volume alerts or notifications sent as needed. A continuous delivery creates a single delivery instance. All delivery logs (broadLog) and tracking logs reference this one delivery, simplifying monitoring and reporting.</p>
<p>For more information, refer to the <a href="../workflows/activities/continuous-delivery.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Campaign approval management</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The approval process helps coordinate multiple stakeholders and ensures quality control before deliveries are sent. Use approvals when your organization requires validation from different teams, such as marketing managers reviewing content or data analysts validating target audiences.</p>
<p>For more information, refer to the <a href="../campaigns/campaign-approvals.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

### Improvements {#26-1-improvements}

* Dynamic reporting now supports push notifications and SMS. [Learn more](../reporting/dynamic-reporting/get-started-reporting.md)
* Pre-defined filters - A new "Shared filter" option lets you make a predefined filter available to other users in your organization. [Learn more](../get-started/predefined-filters.md#share-filter)
* Personalization fields created in Adobe Experience Manager, such as Name, Email, Date, and Address, are now included and available when using content template.
* Content quality evaluation now checks for readability, cohesiveness, and effectiveness issues independent of brand guidelines, identifying unclear messaging, inconsistent tone, or structural gaps. [Learn more](../content/brands-score.md)
