---
title: Campaign v8 Web User Interface previous Release Notes
description: 2024 Campaign Web User Interface releases
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
---
# 2024 release notes {#2024-release}

This page lists all changes and improvements available with **2024 releases**. Latest relese notes are available in [this page](release-notes.md).


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


### Improvements

* **Workflow activities** - You can now move an activity and all its child nodes from a transition to another within a workflow. A dedicated **Move** button is available in the activity's properties pane to perform this. [Learn more](../workflows/orchestrate-activities.md#move)

* **Workflow enrichment activity**

    * You can now define an Alias and a Label when creating a new field in the **Enrichment** activity. [Learn more](../workflows/activities/enrichment.md#collection-settings)
    * You can now add offers for each profile in the **Enrichment** activity. [Learn more](../workflows/activities/enrichment.md##add-offers)

* **Distribution of values** - When accessing the list of fields for personalization, you can now check how values are distributed for each field. A dedicated popup window shows the number and percentage for each value. [Learn more](../query/build-query.md#distribution-values-query)

* **Version and system info** - You can now access details about your instance versions, both for the client console and the Web User Interface. This new section also lists all the built-in packages installed in your environment. [Learn more](../get-started/user-interface.md#user-interface-about)

* **Lists** - You can now easily reorder the values of a list. [Learn more](../get-started/work-with-folders.md)

* **Delivery** - Delivery variable are now accessible from personalisation fields. [Learn more](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)


## September updates {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI Assistant</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Once you have crafted and tailored your message, take it to the next level with AI Assistant in Adobe Campaign Web. This powerful tool allows you to optimize the impact of your content by generating a range of engaging text, main titles and visually appealing images.</p>
<p>Immerse yourself in a hands-on experience with <a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">our live feature preview</a>, designed to let you explore its features firsthand and fully understand its capabilities.</a>.</p>
<p>For more information, refer to the <a href="../email/generative-gs.md">detailed documentation</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Availability date: Sept 12</p>
</td>
</tr>
</tbody>
</table>

## August release {#24-8-release}

**Release date**: Sept 3, 2024

The following features and improvements are available starting August release.

* **SMTP parameters** - SMTP settings are now available in the email delivery settings. [Learn more](../advanced-settings/delivery-settings.md#smtp)

* **Global variables** - You can now define global variables to define values for your deliveries. [Learn more](../advanced-settings/delivery-settings.md#variables-delivery)

### New features in Limited Availability {#acs-24-8}

>[!AVAILABILITY]
>
>The following capabilities are in Limited Availability (LA). They are restricted to customers migrating **from Adobe Campaign Standard to Adobe Campaign v8**, and cannot be deployed on any other environment.
>
>Refer to the following documentation pages: [Campaign Standard transition to Campaign v8](../rn/acs-migration.md) and [Features for Campaign Standard users](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"}.

* **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **Subscriptions with Landing pages** - You can now link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Visual fragments** - You can now archive visual content fragments. [Learn more](../content/create-fragment.md#archive)

* **Captcha in landing pages** - You can now add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->


## July release notes {#24-7-release}

**Release date**: July 30-31, 2024

The following features and improvements are available starting July release.

### Content Fragments {#24-7-1}

You can now create and use content fragments. A content fragment is a reusable component that can be referenced in one or more messages. When modifying a fragment, every content using it is updated. This functionality allows to prebuild multiple custom content blocks that can be used by marketing users to quickly assemble message contents in an improved design process.

Two types of fragments are available:

* **Expression fragments** are pre-defined expressions that are available from a dedicated entry in the expression editor.
* **Visual fragments** are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](../content/fragments.md)

    >[!AVAILABILITY]
    >
    >**Visual fragments** are in Limited Availability (LA). This capability is restricted to customers migrating **from Adobe Campaign Standard to Adobe Campaign v8**, and cannot be deployed on any other environment.

### Trap group {#24-7-2}

A  **Trap group** is a list of seed addresses. It is used to include specific addresses in your deliveries, and then target profiles who do not match the defined target criteria. This way, recipients who are out of the delivery audience can receive the delivery, as any other target recipient would. You can use seed addresses when sending proofs, or to protect your mailing list. [Learn more](../audience/trap-group.md)

### Rich push notification templates {#24-7-3}

You can now send rich push notifications. A rich push notification is an enhanced form of mobile notification that goes beyond simple text messages by incorporating multimedia elements such as images, interactive buttons, or other rich media content. With this version, a set of templates for rich push notifications are now available for your iOS and Android apps. 

[Learn more](../push/rich-push.md)

>[!AVAILABILITY]
>
>This capability requires an update to Campaign v8.6.3 <!--or v8.7.2-->. Learn more in Campaign v8 Client console [release notes](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/release-notes){target="_blank"}.

### Improvements {#improvements-24-7}

**Folders management** - You can now manage permissions and restrictions on folders.

## June release notes {#24-6-release}

**Release date**: June 18-19, 2024

The following features and improvements are available to all users starting June release.


### Plans and programs {#24-6-4}

You can now create plans and programs to organize your campaigns. By defining a folder hierarchy, you can organize your campaigns into programs, and your programs into plans. [Read more](../administration/plans-programs.md)

### Improvements {#improvements-24-6}

* **Reconciliation in Enrichment activity**: The **Enrichment** activity can now be used to reconcile data from the the Campaign database schema with data from another schema, or with data coming from a temporary schema such as data uploaded using a Load file activity. For example, you can use this option to reconcile a profile's country, specified in an uploaded file, with one of the countries available in the dedicated table of the Campaign database. [Read more](../workflows/activities/enrichment.md)


### New feature in Limited Availability {#acs-24-6}

>[!AVAILABILITY]
>
>The following capability is in Limited Availability (LA). It restricted to customers migrating **from Adobe Campaign Standard to Adobe Campaign v8**, and cannot be deployed on any other environment.

* **Delivery alerting**

The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


## May release notes {#24-5-release}

**Release date**: May 21, 2024

The following features and improvements are available to all users starting May release.

### Audit trail  {#24-5-1}

The new **Audit trail** capability provides a detailed and chronological record of all actions and events that have been made to your Adobe Campaign instance in real-time. It offers a convenient method to trace all changes to your Campaign data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance. [Read more](../reporting/audit-trail.md)

### Custom fields {#24-5-2}

**Custom fields** are additional attributes added to the out-of-the-box schemas through the Adobe Campaign console. In Campaign web user interface, these custom fields are now visible in various screens, for example the details of a profile or a test profile. In the web user interface, you cannot create custom fields, but you can now modify the way they display. [Read more](../administration/custom-fields.md)

### Create links between tables {#24-5-3}

You can now create links with another table in the **Enrichment** workflow activity. Use the new **Link definition** section in the activity parameters to create a link between the working table data and the Adobe Campaign database. For example, if you load data from a file which contains the account number, country and email of recipients, you can now create a link towards the country table in order to update this information in their profiles. [Read more](../workflows/activities/enrichment.md#create-links)

### General improvements {#improvements-24-5}

* **Direct mail** - You can now leverage the expression editor to select the attributes to display in direct mail extraction files. [Read more](../direct-mail/content-direct-mail.md)

* **Folder management** - You can now create a sub-folder of a different type than the parent folder. [Read more](../get-started/permissions.md#folders)

* **Globalization** - As part of our ongoing effort to deliver a unified user experience, we harmonize the terminology used in the Adobe Experience Cloud products and apps. This affects the German term "Titel" which is changed to "Label" when it relates to the name of an object. The changes will be progressively rolled out in the UI and documentation.


## April release notes {#april-24-4-release}

**Release date**: May 2, 2024

### New features {#new-24-4}

The following features are available to all users starting April release.

**New workflow activities**

* **Update data** - Use this activity to perform mass updates on fields in the database. Several options allow you to personalize the data update. [Read more](../workflows/activities/update-data.md)
* **Subscription services** - Use this activity to subscribe or unsubscribe multiple profiles to/from a service in a single action. [Read more](../workflows/activities/subscription-services.md)
* **Extract file** - Use this activity to export data from Adobe Campaign to another system as an external file. [Read more](../workflows/activities/extract-file.md)
* **Transfer file** - Use this activity to receive or send files, test for file presence, or list files on a server. The protocol used can be either server-to-server protocol or HTTP protocol. [Read more](../workflows/activities/transfer-file.md)
* **Test** - Use this activity to enable transitions based on specified conditions. [Read more](../workflows/activities/test.md)
* **JavaScript code** - Use this activity to execute a JavaScript code snippet in the context of a workflow. [Read more](../workflows/activities/javascript-code.md)
* **External signal** - Use this activity to trigger the execution of a workflow from another workflow, or an API call. [Read more](../workflows/activities/external-signal.md)
* **Incremental query** - Use this activity to query the database on a scheduled basis. Each time this activity is executed, the results from the previous executions are excluded. This allows you to target only new elements. [Read more](../workflows/activities/incremental-query.md)

**Rich Push Notification templates**

You can now send rich push notifications via Android. Rich push notification is an enhanced form of mobile notification that goes beyond simple text messages by incorporating multimedia elements such as images, interactive buttons, or other rich media content. [Read more](../push/rich-push.md)

Note that this feature is in **Limited Availability** (LA).


### New features in Limited Availability {#acs-24-4}

>[!AVAILABILITY]
>
>The following capabilities are in Limited Availability (LA). They are restricted to customers migrating **from Adobe Campaign Standard to Adobe Campaign v8**, and cannot be deployed on any other environment.
>
>Refer to the following documentation pages: [Campaign Standard transition to Campaign v8](../rn/acs-migration.md) and [Features for Campaign Standard users](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Branding** -  As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest APIs** - As a Campaign Standard migrated user, you can use Rest APIs to create integrations for Adobe Campaign and build your own ecosystem by interfacing Adobe Campaign with the panel of technologies that you use. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Dynamic Reporting** - As a Campaign Standard migrated user, you can access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Landing Pages** - The following improvements to landing pages are only available to users transitioning from Campaign Standard:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)

### General improvements {#improvements-24-4}

The improvements below are available to all customers starting April release.

* The **Load file** activity has been enhanced with several sections allowing you to upload a sample file, to manage errors and rejects, and delete uploaded files after the activity has been executed. [Read more](../workflows/activities/load-file.md)


* You can now **copy/paste activities** from a workflow to another workflow from a different browser tab. [Read more](../workflows/orchestrate-activities.md#copy-activities-copy)

* All workflow activities now allow you to manage their **execution options**. This lets you define the activity's execution mode and behavior in case of errors. [Read more](../workflows/orchestrate-activities.md#execution-options-execution)

* The "Do not activate the transition if the population is empty" option in the **Split activity** allows you to choose whether the workflow should transition to the next activity when the segment result is empty. [Read more](../workflows/activities/split.md)

## March release notes {#24-3-release}

>[!AVAILABILITY]
>
>This version is available to all users starting [Campaign (console) v8.6 release](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html). Learn more about Adobe Campaign client console releases and upgrades in [Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html){target="_blank"}.

**Release date**: March 19-20, 2024

### Direct Mail Channel {#24-3-dm}

**Direct mail** channel is now available for use in workflows and as standalone deliveries. Direct mail is an offline channel that allows you to create, personalize and generate an extraction files, and share it with your direct mail providers to send mail to your customers.

### New Change data source workflow activity {#24-3-change-data-source}

The **Change data source** targeting activity allows you to change the data source used by your workflow's working table. This activity provides more flexibility by allowing you to manage data across your different databases and improve performances.

### Split workflow activity improvement {#24-3-split}

You can now use the **Generate all subsets in the same table** option in the **Split** workflow activity to group all the subsets into a single output transition.

### Query modeler {#24-3-query-modeler}

* The query modeler is now available for use in the Email Designer. It allows you to build conditions when creating conditional content.
* Predefined values are now available for date-type attributes when creating a custom condition. 
* Operators can no longer be added on a new transition in the diagram. They can only be added on an existing transition before filtering components to group them together.