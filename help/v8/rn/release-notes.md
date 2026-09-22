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

## September '26 release {#26-9-release}

_September 22, 2026_

### New features {#26-9-features}

<table>
<thead>
<tr>
<th><strong>LINE channel</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign now supports the <strong>LINE</strong> channel, a popular instant messaging application. Create and send LINE messages using text, image, or video content, in standalone deliveries or in workflows, alongside your other channels. <a href="../line/get-started-line.md">Read more</a></p>
</td>
</tr>
</tbody>
</table>

### Improvements {#26-9-improvements}

* **Side navigation access**: Administrators can now hide specific menu entries from the side navigation. [Read more](../administration/schemas-browse-access.md#customize-screen-display-screen-def)
* **Additional approval types**: You can now require budget and delivery-start approvals for Campaign deliveries, in addition to content and target approvals. [Read more](../campaigns/campaign-approvals.md#configure-approval-settings-configure-approvals)
* **Visitor-based SMS targeting**: The visitor target mapping is now available for SMS deliveries. [Read more](../sms/create-sms.md)
* **Workflow cancel button**: A new **Cancel** button lets you revert unsaved changes in a workflow. [Read more](../workflows/orchestrate-activities.md#save-or-discard-your-changes-save-cancel)
* **Deduplication with multiple values**: The **Following a list of values** option now supports multiple attributes. [Read more](../workflows/activities/deduplication.md#configure-the-deduplication-activity-deduplication-configuration)
* **Mobile target mapping**: You can now create target mappings for mobile application targets. [Read more](../administration/target-mappings.md#create-a-target-mapping-create-mapping)
* **External database enrichment**: You can now enrich data from an external database in the **Enrichment** or **Build audience** activity. [Read more](../workflows/activities/enrichment.md#external-data)
* **File audience reconciliation**: You can now configure whether to import recipients into the database when targeting an audience from a file. [Read more](../audience/file-audience.md#select-and-configure-the-input-file-upload)
* **Direct joins on collections**: When selecting an attribute directly from a collection, you can now choose how the condition is built: using the recommended default option, an aggregate function, or an advanced direct join. [Read more](../query/build-query.md#custom-conditions-on-linked-tables-1-1-and-1-n-links-links)

