---
title: Campaign v8 Web User Interface Release Notes
description: Discover new features coming with the latest Campaign Web User Interface release
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
---
# Release notes {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Release notes"
>abstract="Adobe Campaign Web user interface releases operate on a continuous delivery model which allows for a more scalable, phased approach to feature deployment. Accordingly, Campaign release notes get updated several times a month, with latest features, improvements, and fixes. We recommend you to check them regularly."

Adobe Campaign Web user interface releases operate on a continuous delivery model which allows for a more scalable, phased approach to feature deployment. Accordingly, these release notes get updated several times a month. Please check them regularly.

## July '26 release {#26-7-release}

_July 28, 2026_

### New features {#26-7-features}

<table>
<thead>
<tr>
<th><strong>Offer management</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now manage offers end-to-end directly from the Campaign Web User Interface, without using the Client Console. Configure offer environments and offer spaces, build your offer catalog and categories, create offers with eligibility rules and priority weights, and approve and deploy them for use in your deliveries.</p>
<!--p>For more information, refer to the <a href="../offers/gs-offer-management.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Brand configuration</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdomain and protocols, email header parameters, and URL tracking parameters, are now available in the Web UI.</p>
<!--p>For more information, refer to the <a href="../administration/branding/branding-configure.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Public resources in the Email Designer</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>When adding images to your emails, you can now select <strong>public resources</strong>. This allows you to choose an image already available on your Adobe Campaign instance, such as a file previously imported in the Email Designer or a public resource uploaded from the Client Console.</p>
<!--p>For more information, refer to the <a href="../email/content-components.md#image">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Data loading (RDBMS) workflow activity</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The <strong>Data loading (RDBMS)</strong> activity is now available in the Campaign Web User Interface. Use this activity to load data directly from an external relational database into your workflow. The extracted data is available throughout the workflow and can be used for targeting, enrichment, or further data processing.</p>
<!--p>For more information, refer to the <a href="../workflows/activities/data-loading-rdbms.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Dynamic JavaScript pages</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Dynamic JavaScript pages (JSSP) let you build server-side pages that generate dynamic content when accessed through a URL, such as custom APIs, exports, or web application logic. You can now create, modify, duplicate, and delete these pages directly from the Campaign Web User Interface.</p>
<!--p>For more information, refer to the <a href="../administration/dynamic-javascript-pages.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

### Improvements {#26-7-improvements}

* The following improvements have been made to **custom schema configuration**:
    * The new **Action data** section allows you to restrict the actions available on a custom schema's records, regardless of the security rules configured on individual folders. <!--[Read more](../administration/schemas-action-data.md)-->
    * **Custom filters** have been added in the **Inventory list configuration** section. They allow you to choose which attributes are displayed as quick-access fields in the filters pane of the list view. <!--[Read more](../administration/schemas-custom-filters.md)-->

* The following improvements have been made to **workflows**:
    * Deleting a workflow activity is now more flexible: when the activity has subsequent activities, you can choose to delete them all, delete only the selected activity, or delete it while keeping its subsequent activities in a new branch. <!--[Read more](../workflows/orchestrate-activities.md#delete-activity)-->
    * You can now disconnect a transition between two workflow activities without deleting either of them. This lets you reorganize a workflow diagram, for example to temporarily set aside a group of activities you want to keep, without having to delete and recreate them. <!--[Read more](../workflows/orchestrate-activities.md#disconnect-transition)-->
    * Horizontal and vertical scroll bars are now displayed around the workflow canvas, letting you navigate large workflows by dragging directly to the area you want to view. <!--[Read more](../workflows/orchestrate-activities.md)-->
    * When savind or starting/restarting a workflow, a warning is now displayed if another user modified the workflow in the Web UI or the Client Console since you opened it. You can choose to override the other changes with yours, reload the workflow to get the latest version, or cancel.

* **Sender email address**: You can now restrict the **From email** field of your deliveries to a predefined list of addresses, using the **NmsDelivery_senderAddressMask** option. <!--[Read more](../administration/options.md#restrict-sender-address)-->
* **Login error messages** have been improved: When a login attempt fails, the Web UI now displays a more specific error message for several scenarios (for example, when the user has no security zone assigned or their IP address is restricted).
