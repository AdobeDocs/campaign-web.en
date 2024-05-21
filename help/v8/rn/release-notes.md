---
title: Latest release notes
description: Discover new feature coming with Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
---
# Release notes {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Release notes"
>abstract="Adobe Campaign Web user interface releases operate on a continuous delivery model which allows for a more scalable, phased approach to feature deployment. Accordingly, Campaign release notes get updated several times a month, with latest features, improvements, and fixes. We recommend you to check them regularly."

Adobe Campaign Web user interface releases operate on a continuous delivery model which allows for a more scalable, phased approach to feature deployment. Accordingly, these release notes get updated several times a month. Please check them regularly.

## May release notes {#24-5-release}

**Release date**: May 21, 2024

The following features and improvements are available to all users starting May release.

### Audit trail  {#24-5-1}

The new **Audit trail** capability provides a detailed and chronological record of all actions and events that have been made to your Adobe Campaign instance in real-time. It offers a convenient method to trace all changes to your Campaign data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.

### Custom fields {#24-5-2}

**Custom fields** are additional attributes added to the out-of-the-box schemas through the Adobe Campaign console. In Campaign web user interface, these custom fields are now visible in various screens, for example the details of a profile or a test profile. In the web user interface, you cannot create custom fields, but you can now modify the way they display. [Read more](../administration/custom-fields.md)

### Create links between tables {#24-5-3}

You can now create links with another table in the **Enrichment** workflow activity. Use the new **Link definition** section in the activity parameters to create a link between the working table data and the Adobe Campaign database. For example, if you load data from a file which contains the account number, country and email of recipients, you can now create a link towards the country table in order to update this information in their profiles.


### Content fragments {#24-5-4}

* You can now author, use, and save **visual fragments** to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process. [Learn more](../email/fragments.md)

* You can now author, use, and manage **expression fragments** to quickly build personalized content. A fragment is a prebuilt reusable component that can be referenced in multiple contents across Adobe Campaign for an improved and accelerated design process.


### General improvements {#improvements-24-5}

* **Direct mail** - You can now leverage the expression editor to select the attributes to display in direct mail extraction files.

* **Folder management** - You can now create a sub-folder of a different type than the parent folder.


<!--* **Execution options for workflows** - You can now define execution options for your workflows, such as the maximum duration, the affinity, or the time zone.-->

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
<!--**Workflow - Copy/Paste into another tab**: -->

* The **Load file** activity has been enhanced with several sections allowing you to upload a sample file, to manage errors and rejects, and delete uploaded files after the activity has been executed. [Read more](../workflows/activities/load-file.md)


* You can now **copy/paste activities** from a workflow to another workflow from a different browser tab. [Read more](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* All workflow activities now allow you to manage their **execution options**. This lets you define the activity's execution mode and behavior in case of errors. [Read more](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

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
