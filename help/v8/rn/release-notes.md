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

Changes and improvements available with previous releases are listed in the [2024](release-notes-24.md) and [2025](release-notes-25.md).

## April '25 release {#25-4-release}

**Release date**: April 29, 2025


### New features {#25-4-features}

The following features are available to all users starting April release.

<table>
<thead>
<tr>
<th><strong>Call center channel</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The call center channel is now available in Campaign Web User interface. This channel refers to a communication method used to manage and track communications or interactions that are handled via a call center — typically phone calls made by agents to customers or prospects.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>For more information, refer to the <a href="../call-center/gs-call-center.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>New rule builder</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>A new rule builder is now available to help you define complex conditions in an improved user interface. You can switch from the old to the new rule builder as needed.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>For more information, refer to the <a href="../query/query-modeler-overview.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>External account authoring</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>As a Campaign administrator, you can now set up new connections with external systems from Campaign Web user interface.
You can also view, update and manage existing external accounts.</p>
<p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
 
### Improvements {#25-4-improvements}

**General interface improvements**

* The Field description, Add to favorites and Distribution of values options for schema attributes are now more visible in the user interface. For more information, refer to the [detailed documentation](../get-started/attributes.md).
* In the interface, the date and time is now displayed according to the primary language set in the Experience League preferences. This improvement is only available for several languages. To see the complete list of supported languages, refer to the [detailed documentation](https://experienceleague.adobe.com/en/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**Email Editor**: To enhance accessibility in Campaign Web UI, two new fields are now available in the Email Designer: they correspond to the `title` element and lang attribute in the `html` element of your email content. You can define these settings in addition to the Preheader field, in the email Body section. For more information, refer to the [detailed documentation](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Schemas**

* You can now edit the temporary schema of a list from Campaign web user interface. For more information, refer to the [detailed documentation](../audience/manage-audience.md).
* You can now preview the custom fields of a schema in a sample screen. For more information, refer to the [detailed documentation](../administration/custom-fields.md#add).
* You can now move custom fields in the list using drag and drop. For more information, refer to the [detailed documentation](../administration/custom-fields.md#add).


### New features in Limited Availability {#25-4-features-la}

>[!AVAILABILITY]
>
>The following capabilities are in Limited Availability (LA). They are restricted to customers migrating **from Adobe Campaign Standard to Adobe Campaign v8**, and cannot be deployed on any other environment. They require an upgrade of the Campaign server to v8.7.4.
>
>Refer to the following documentation pages: [Campaign Standard transition to Campaign v8](../rn/acs-migration.md) and [Features for Campaign Standard users](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interace. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. For more information, refer to the [detailed documentation](../email/edit-content.md).

* **Dynamic Reporting for Multilingual** - Dynamic reporting is now available for multilingual email deliveries. For more information, refer to the [detailed documentation](../reporting/global-reports.md). <a href=".">detailed documentation</a>.

* **SMS REST API support (LA)** - The Transactional Messaging REST API is now available for the SMS channel. When both email and mobilePhone are present in the payload, you can use the "wishedChannel" field to specify the channel. If not provided, email will be used by default unless wishedChannel explicitly requests SMS. For more information, refer to the [detailed documentation](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}.

