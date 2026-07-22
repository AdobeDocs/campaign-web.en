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

_July 20, 2026_

### New features {#26-7-features}

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
<p>For more information, refer to the <a href="../administration/branding/branding-configure.md">detailed documentation</a>.</p>
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
<p>You can now reuse public resources when adding images to your emails. In addition to browsing your Adobe Experience Manager Assets library or importing a new file from your computer, you can select an image already available on your Adobe Campaign instance, such as a file previously imported or a public resource uploaded from the Client Console. This option is available for both content images and background images.</p>
<p>For more information, refer to the <a href="../email/content-components.md#image">detailed documentation</a>.</p>
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
<p>For more information, refer to the <a href="../workflows/activities/data-loading-rdbms.md">detailed documentation</a>.</p>
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
<p>For more information, refer to the <a href="../administration/dynamic-javascript-pages.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Offer management in the Web UI</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><em>Description coming soon.</em></p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Custom schema configuration improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The screen definition of a custom schema now includes an <strong>Action data</strong> section, letting you restrict create, update, and delete actions for its records. Enable <strong>Read-only</strong> to make the detail screen read-only and hide list actions, or <strong>Do not allow deletion</strong> to remove the delete action. These restrictions apply at the schema level, across every folder and for every user, including administrators.</p>
<p>It also includes a <strong>Custom filters</strong> section, inside <strong>Inventory list configuration</strong>, letting you choose which attributes are displayed as quick-access fields in the filters pane of the list view, above the <strong>Advanced filters</strong> rule builder. You can select direct attributes, link attributes, or sub-attributes of a link.</p>
<p>For more information, refer to the <a href="../administration/schemas-action-data.md">Action data</a> and <a href="../administration/schemas-custom-filters.md">Custom filters</a> documentation pages.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Workflow improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Horizontal and vertical scroll bars are now displayed around the workflow canvas, giving you another way to navigate large workflows by dragging directly to the area you want to view.</p>
<p>You can now disconnect a transition between two workflow activities without deleting them. If the source activity has a single outbound transition, disconnecting it creates a new branch containing the activities that were connected; if the source activity has multiple outbound transitions, only the selected transition is removed.</p>
<p>When a workflow is already open for edition by another user, Adobe Campaign now warns you before you save, helping you avoid overwriting that user's changes.</p>
<p>For more information, refer to the <a href="../workflows/orchestrate-activities.md#toolbar">Orchestrate activities</a> and <a href="../workflows/orchestrate-activities.md#disconnect-transition">Delete and disconnect activities</a> documentation pages.</p>
</td>
</tr>
</tbody>
</table>

### Improvements {#26-7-improvements}

* **More descriptive login error messages**: _Description coming soon._
* **Restrict edition of the sender email address**: _Description coming soon._
