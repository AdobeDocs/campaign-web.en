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

## March '26 release {#26-3-release}

### New features {#26-3-features}

<table>
<thead>
<tr>
<th><strong>Schema authoring (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The schema authoring feature is now available to all customers (GA). This capability allows you to create and manage schemas directly from the Campaign Web User Interface. You can create new tables, extend existing schemas and create custom forms. You can define custom data structures to support your specific business needs without requiring access to the Client Console.</p>
<p>For more information, refer to the <a href="../administration/schemas.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the <a href="../email/apply-email-themes.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integration of custom Firefly models and third-party image generation models</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Enable seamless integration of standard and custom Firefly models, along with approved third-party image models, to provide greater flexibility, control, and brand alignment when generating images.</p>
<p>Choose the right model for your needs:</p>
<ul><li> <strong>Adobe model</strong> (powered by Firefly Image Model 4) for immediate image generation without additional setup</li><li> <strong>Partner model</strong> (powered by Gemini 2.5 Flash) for specialized capabilities</li><li><strong>Custom models</strong> (brand-specific models trained on your own assets) for on-brand generation that aligns precisely with your brand identity, style, and visual guidelines.</li></ul>
<p>For more information, refer to the <a href="../content/generative-models.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Automated delivery activity</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The <strong>Automated delivery</strong> workflow activity is now available in the workflow palette. You can use it to create or execute delivery actions (prepare, send a proof, prepare and start, etc.) directly within your workflow. Select an existing delivery created outside the workflow to reuse it on every run, or create a new delivery from a template each time the activity executes.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>For more information, refer to <a href="../workflows/activities/automated-delivery.md">detailed documentation.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Multiple workflow branches and Join activity</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p><strong>Multiple branches</strong> are now supported. Instead of using a <strong>Fork</strong>, you can click <strong>Add branch</strong> on the toolbar. The <strong>AND-join</strong> activity has also been improved. It is now a generic <strong>Join</strong> activity that lets you choose between AND and OR join options.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>For more information, refer to <a href="../workflows/orchestrate-activities.md#toolbar">Orchestrate activities</a> and <a href="../workflows/activities/join.md">Join</a> documentation pages.</p>
</td>
</tr>
</tbody>
</table>

### Improvements {#26-3-improvements}

* The **Start** workflow activity has been added to improve compatibility with the Client Console. This activity is optional and is not inserted by default in new workflows. However, it is added automatically to existing workflows.
[Learn more](../workflows/activities/about-activities.md#flow-control)
* The time zone selection field in the **Schedule** settings of a delivery has been moved below the **Contact date** field. [Learn more](../msg/create-deliveries.md#gs-schedule)