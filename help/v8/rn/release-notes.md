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

## August '26 release {#26-8-release}

_August 18, 2026_

### New features {#26-8-features}

<table>
<thead>
<tr>
<th><strong>Approval workflow activity</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The <strong>Approval</strong> workflow activity, previously only available in the Client Console, is now available in the Campaign Web User Interface. Assign the task to a group or an individual operator, customize the notification title and message, and define the possible answers (for example Yes/No) as output branches.</p>
<p>For more information, refer to the <a href="../workflows/activities/approval.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

### Improvements {#26-8-improvements}

* **Opens tracking**: You can now enable or disable open tracking directly from the Campaign Web User Interface. This helps you comply with data protection regulations. [Read more](../advanced-settings/delivery-settings.md#tracking-tab)
* **Program list view**: Programs are now listed in a dedicated view, similar to campaigns, deliveries, and workflows. You can browse existing programs and create new ones directly from this view. [Read more](../administration/plans-programs.md#create-program)
* **Custom schema configuration**: In the **Action data** section, you can now disallow the **Duplicate** action on a custom schema's records. [Read more](../administration/schemas-action-data.md#action-data)
* **Custom filters**: In the schema editor, you can now restrict the values available in the picker for a link-type custom filter, using the new **Link settings** dialog. [Read more](../administration/schemas-custom-filters.md#settings)
* **Schema validation**: You can now validate the structure of a schema directly from the schema editor, using the new **Check** button. [Read more](../administration/schemas-create-publish.md#create-new)
* **Folder security**: Actions available on a folder are now consistently governed by the operator's rights, matching the behavior of the Client Console. [Learn more](../get-started/work-with-folders.md#about-folders).
<!--* **Enrichment activity**: You can now enrich data from an external database directly from the **Enrichment** workflow activity. This matches the capability already available in the Client Console.-->
<!--* **Workflow and delivery templates (only msf???)**: When creating a new workflow or delivery, you must now explicitly select a template. A default template is no longer applied automatically.-->

