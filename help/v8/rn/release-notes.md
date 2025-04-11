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

Adobe Campaign Web user interface releases operate on a continuous delivery model, which allows for a scalable, phased approach to feature deployment. Accordingly, these release notes are updated several times a month. Check them regularly.

Changes and improvements available with previous releases are listed [on this page](release-notes-24.md).

## February '25 release {#25-2-release}

**Release date**: Feb 18, 2025

The following features and improvements are available starting February release.

### Features {#25-2-features}

<table>
<thead>
<tr>
<th><strong>Create business rules (typology rules)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create typologies and typology rules in Adobe Campaign Web User Interface. Typologies control, filter, and prioritize the sending of deliveries. Typologies validate that deliveries always contain mandatory components (such as an unsubscription link or a subject line) or filtering rules to exclude groups from your audience (like unsubscribers, competitors, or non-loyalty customers).</p>
<img src="assets/do-not-localize/typology.gif" alt="Illustration of typology rules creation in Adobe Campaign Web User Interface">
<p>For more information, refer to the <a href="../administration/typologies.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Target mappings</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create target mappings in Campaign Web User Interface. Target mappings define how different delivery channels (email, SMS, push notifications) link to the data fields of a schema. The target mapping defines the targeted audience: profiles, contract beneficiaries, operators, subscribers, prospects, and others.</p>
<img src="assets/do-not-localize/target-mapping.gif" alt="Illustration of target mappings creation in Adobe Campaign Web User Interface">
<p>For more information, refer to the <a href="../administration/target-mappings.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Schema details</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now access the details of a schema by selecting its name in the list. Custom fields editing is now accessible from the <b>Edit custom fields</b> button available in the schema details.</p>
<img src="assets/do-not-localize/schemas.gif" alt="Illustration of schema details and custom fields editing in Adobe Campaign Web User Interface">
<p>For more information, refer to the <a href="../administration/schemas.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

## January '25 release {#25-1-release}

**Release date**: Feb 5, 2025

The following features and improvements are available starting January release.

### Features {#25-1-features}

<table>
<thead>
<tr>
<th><strong>Create and use visual fragments</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries or in content templates. This feature is now available to all customers running on server build 8.6.4 and above.</p>
<img src="assets/do-not-localize/visual-fragment.gif" alt="Illustration of visual fragments creation and usage in Adobe Campaign Web User Interface">
<p>For more information, refer to the <a href="../content/use-visual-fragments.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Use a third-party system to send deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define external deliveries and external delivery templates in the Campaign web interface. In this mode, messages are compiled into an output file, which can be shared with your external provider. By default, the external delivery mode is used for the direct mail channel.</p>
<img src="assets/do-not-localize/external-delivery.gif" alt="Illustration of external delivery setup in Adobe Campaign Web User Interface">
<p>For more information, refer to the <a href="../msg/send-external-deliveries.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Manage your enumerations</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create enumerations directly through Adobe Campaign Web User Interface. An enumeration is a list of values suggested by the system to populate fields. Use enumerations to standardize the values of these fields, assist with data input, or use within queries.</p>
<img src="assets/do-not-localize/enumerations.gif" alt="Illustration of enumeration management in Adobe Campaign Web User Interface">
<p>For more information, refer to the <a href="../administration/enumerations.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Create custom options</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now access technical options within Adobe Campaign Web User Interface and create your own custom options to suit your needs. This is particularly useful when working with JavaScript code workflow activities to store intermediate data.</p>
<img src="assets/do-not-localize/options.gif" alt="Illustration of custom options creation in Adobe Campaign Web User Interface">
<p>For more information, refer to the <a href="../administration/options.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Define and call JavaScript codes</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create JavaScript codes in Adobe Campaign Web User Interface. This allows you to create reusable functions that can be used across workflows, similar to a library.</p>
<img src="assets/do-not-localize/javascript.gif" alt="Illustration of JavaScript code creation in Adobe Campaign Web User Interface">
<p>For more information, refer to the <a href="../administration/javascript-codes.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Landing page generation with the AI Assistant</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The AI Assistant is now available with your landing page deliveries, enabling you to generate text, images, or complete page layouts.</p>
<img src="assets/do-not-localize/ai-lp.gif" alt="Illustration of AI Assistant usage for landing page generation in Adobe Campaign Web User Interface">
<p>For more information on AI Assistant, refer to the <a href="../email/generative-lp.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

### Improvements {#25-1-improvements}

* Customize the display of custom fields in the interface:
    * Select additional custom fields to display in the interface.
    * Set rules for displaying link-type custom fields, such as restricting list values based on another field's input.
    * Arrange fields in the interface more flexibly: fields can span a single column or be grouped into subsections for better organization.
    * Set specific fields as read-only.

* Recent and Favorites filters: Add frequently used attributes to favorites for quick access. In addition to favorites, view and use the most recently selected attributes.

* External accounts: The new **[!UICONTROL Routing]** type is available for selection when creating a new external account. It allows you to configure a specific external account for use in your external deliveries. [Learn more](../administration/external-account.md#routing).