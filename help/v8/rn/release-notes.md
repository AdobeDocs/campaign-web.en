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

Changes and improvements available with previous releases are listed [in this page](release-notes-24.md).

## October '24 release {#24-10-release}

**Release date**: Oct 29, 2024

The following features and improvements are available starting October release.

### Features

<table>
<thead>
<tr>
<th><strong>External accounts</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You now have the ability to set up and manage external accounts directly through Adobe Campaign Web User Interface. This new feature makes it simple to configure different types of external accounts, such as bounce emails (POP3) or execution instances.</p>
<p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Transactional messaging</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Transactional messaging (Message Center) is now available in the Campaign web user interface. This add-on is designed for triggering messages which are generated from events triggered from information systems, and can be: invoice, order confirmation, shipping confirmation, password change, product unavailability notification, account statement, website account creation, etc.</p>
<p>For more information, refer to the <a href="../transactional-messaging/transactional.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### Improvements

* **Workflow activities** - You can now move an activity and all its child nodes from a transition to another within a workflow. A dedicated **Move** button is available in the activity's properties pane to perform this. [Learn more](../workflows/orchestrate-activities.md#move)

* **Workflow enrichment activity**

    * You can now define an Alias and a Label when creating a new field in the **Enrichment** activity. [Learn more](../workflows/activities/enrichment.md#collection-settings)
    * You can now add offers for each profile in the **Enrichment** activity. [Learn more](../workflows/activities/enrichment.md##add-offers)

* **Distribution of values** - When accessing the list of fields for personalization, you can now check how values are distributed for each field. A dedicated popup window shows the number and percentage for each value. [Learn more](../query/build-query.md#distribution-values-query)

* **Version and system info** - You can now access details about your instance versions, both for the client console and the Web User Interface. This new section also lists all the built-in packages installed in your environment. [Learn more](../get-started/user-interface.md#user-interface-about)

* **Lists** - You can now easily reorder the values of a list. [Learn more](../get-started/work-with-folders.md)

* **Delivery** - Delivery variable are now accessible from personalisation fields. [Learn more](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)