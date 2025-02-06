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
<p>Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. This feature is now available to all customers running on server build 8.6.4 and above.</p>
<img src="assets/do-not-localize/visual-fragment.gif">
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
<img src="assets/do-not-localize/external-delivery.gif">
<p>For more information, refer to the <a href="../msg/send-external-deliveries.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--
<table>
<thead>
<tr>
<th><strong>Create business rules (typology rules)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create typologies and typology rules in the Adobe Campaign web interface. A typology is a collection of typology rules that help control, filter, and prioritize deliveries. Typologies ensure that your deliveries always contain required elements (such as an unsubscribe link or subject line) and apply filtering rules to exclude specific groups from your target audience (such as unsubscribers, competitors, or non-loyalty customers).</p>
<img src="assets/do-not-localize/typology.gif">
<p>For more information, refer to the <a href="../administration/typologies.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
-->

<table>
<thead>
<tr>
<th><strong>Manage your enumerations</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create enumerations directly through Adobe Campaign Web User Interface. An enumeration is a list of values suggested by the system to populate fields. Use enumerations to standardize the values of these fields, help with data input or use within queries.</p>
<img src="assets/do-not-localize/enumerations.gif">
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
<img src="assets/do-not-localize/options.gif">
<p>For more information, refer to the <a href="../administration/options.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Define and call Javascript codes</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create JavaScript codes in Adobe Campaign Web User Interface. This allows you to create reusable functions that can be utilized across workflows, similar to a library.</p>
<img src="assets/do-not-localize/javascript.gif">
<p>For more information, refer to the <a href="../administration/javascript-codes.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Landing page generation with the AI Assistant Content Accelerator</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The AI Assistant Content Accelerator is now available with your landing page deliveries, enabling you to generate text, images, or complete page layouts.</p>
<p>For more information on AI Assistant Content Accelerator, refer to the <a href="../email/generative-lp.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>




### Improvements {#25-1-improvements}

* Customize the display of custom fields in the interface:
    
    * You can now select additional custom fields to display in the interface
    * You can now set rules for displaying link-type custom fields, such as restricting list values based on another field's input
    * You can now arrange fields in the interface with more flexibly: fields can span a single column, or be grouped into subsections for better organization
    * You can now set specific fields as read-only

* Recent and Favorites filters: To quickly reuse attributes that are frequently used, you can now add them to favorites. This ensures they are readily accessible for future tasks. In addition to favorites, you can also view and use the most recently selected attributes.

* External accounts: The new **[!UICONTROL Routing]** type is available for selection when creating a new external account. It allows you to configure a specific external account for use in your external deliveries. [Learn more](../administration/external-account.md#routing)