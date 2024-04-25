---
title: Latest release notes
description: Discover new feature coming with Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
---
# Release notes {#latest-release}

<!--Last update: **March 19, 2024**-->

Adobe Campaign Web user interface releases operate on a continuous delivery model which allows for a more scalable, phased approach to feature deployment. Accordingly, these release notes get updated several times a month. Please check them regularly.

## April release notes {#24-4-release}

**Release date**: April 30, 2024

### New features {#new-24-4}

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->
**Update data activity** 

This new activity allows you to perform a mass update on fields in the database. Several options allow you to personalize the data update.

**Subscription services activity**

This new activity allows you to subscribe to or unsubscribe multiple profiles from a service in a single action.

**File management activities**

* **Extract file**: Export data from Adobe Campaign in the form of an external file.
* **Transfer file**: Receive or send files, test for file presence, or list files on a server. The protocol used can be either server-to-server protocol or HTTP protocol.

**Advanced activities**

* **Test**: Enable transitions based on specified conditions.
* **JavaScript code**: Execute a JavaScript code snippet in the context of a workflow.
* **External signal**: Trigger the execution of a workflow from another workflow or an API call.

**Incremental query**

This new activity allows you to query the database on a scheduled basis. Each time this activity is executed, the results from the previous executions are excluded. This allows you to target only new elements.

**Features for Campaign Standard users**

>[!AVAILABILITY]
>
>These features are released in Limited Availability are available only for Adobe Campaign Standard users.

* **Branding**: Technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates.
* **Dynamic Reporting**: The Dynamic report feature provides fully customizable and real-time reports to measure the impact of your marketing activities within your Adobe Campaign Web Interface instance.
* **Rest APIs**: As a Campaign Stardard migrated user, you can use Rest APIs to create integrations for Adobe Campaign and build your own ecosystem by interfacing Adobe Campaign with the panel of technologies that you use.

### General improvements {#improvements-24-4}

**Landing pages**

<!--**Autorize Unidentified Visitor in Landing Pages**: -->

* A new option in the landing page configuration allows any visitor to access the landing page. If you unselect this option, only identified users can access and submit the form.

<!--Landing pages - Storing additional data on submission-->

* A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted.

<!--**Landing pages - Referencing landing page while configuring a service**: It is now possible to-->

* You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service.

<!--**Landing Pages: Linking Landing page to subscription service**: It is now possible to * **Branding + Landing Pages**: TBD-->

* You can now link a landing page to a service so that profiles can subscribe to or unsubscribe from a specific service upon submitting the landing page.

<!--**Landing Page - Option to call different services on a user action**: -->

* A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one).

<!--Landing Pages - Support conditional content-->

* Conditional content is now supported in landing pages.

**Workflows**

<!--**Workflow - Copy/Paste into another tab**: -->

* You can now copy paste activities to another workflow from a different browser tab.

<!--**Workflow - Execution options**: -->

* All workflow activities now allow you to manage their execution options. This lets you define the activity’s execution mode and behavior in case of errors.

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* The "Do not activate the transition if the population is empty" option in the Split activity allows you to choose whether the workflow should transition to the next activity when the segment result is empty.

<!--* **Workflow - Load file activity improvements**-->

* The Load file activity has been enhanced with several sections allowing you to upload a sample file, to manage errors and rejects and delete uploaded files after the activity has been executed.

<!--* **Support of custom fields**-->

* Custom fields are additional attributes added to the out-of-the-box schemas through the Adobe Campaign console. In Campaign web, These custom fields are displayed in various screens, for example the details of a profile or a test profile. In the web user interface, you cannot create custom fields, but you can now modify the way they display. 

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
