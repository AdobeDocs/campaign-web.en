---
audience: end-user
title: Work with workflows activities
description: Learn how to workflow activities
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
---

# About workflow activities {#workflow-activities}

Workflow activities are grouped into three categories. Depending on the context, available activities may differ. 

All activities are detailed in the sections below:

* [Targeting and data management activities](#targeting)
* [Channel activities](#channel)
* [Flow control activities](#flow-control)

![](../assets/workflow-activities.png)

## Targeting activities {#targeting}

These activities are specific to targeting. They let you build one or more targets by defining an audience and splitting or combining these audiences using intersection, union or exclusion operations.

* [Build audience](build-audience.md): Define your target population. You can either select an existing audience or use the query modeler to define your own query.
* [Change data source](change-data-source.md): Change the data source for the Working table of your workflow."
* [Change dimension](change-dimension.md): Change the targeting dimension as you are building your workflow.
* [Combine](combine.md): Perform segmentation on your inbound population. You can use a union, an intersection or an exclusion.
* [Deduplication](deduplication.md): Delete duplicates in the result(s) of the inbound activities.
* [Enrichment](enrichment.md): Define additional data to process in your workflow. With this activity, you can leverage the inbound transition and configure the activity to complete the output transition with additional data.
* [Incremental query](incremental-query.md): Query the database on a scheduled basis. Each time this activity is executed, the results from the previous executions are excluded. This allows you to target only new elements. 
* [Reconciliation](reconciliation.md): Define the link between the data in the Adobe Campaign database and the data in a work table, for example data loaded from an external file.
* [Save audience](save-audience.md): Update an existing audience or create a new audience from the population computed upstream in a workflow.
* [Split](split.md): Segment incoming population into several subsets.

## Data management activities {#data}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Extract and Load File activities"
>abstract="New data management activities are available in workflows. Use the Extract File activity to export data from Adobe Campaign to another system as an external file. Use the Load File activity to work with profiles and data stored in an external file."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"

These activities are specific to manipulating and enriching population data.

* [Extract file](extract-file.md): Export data from Adobe Campaign to another system as an external file.
* [Load file](load-file.md): Work with profiles and data stored in an external file. 
* [Transfer file](transfer-file.md): Receive or send files, test for file presence, or list files on a server. The protocol used can be either server-to-server protocol or HTTP protocol.
* [JavaScript code](javascript-code.md): Execute a JavaScript code snippet in the context of a workflow.
* [Subscription services](subscription-services.md): Subscribe or unsubscribe multiple profiles to/from a service in a single action.
* [Update data](update-data.md): Perform mass updates on fields in the database. Several options allow you to personalize the data update.

## Channel activities {#channel}

Adobe Campaign Web allows you to automate and execute marketing campaigns across multiple channels. You can combine channel activities into the canvas to create cross-channel workflows that can trigger actions based on customer behavior. The following **Channel** activities are available: Email, SMS, Android and iOS Push notifications. [Learn how to set up a delivery in the context of a workflow](channels.md).

## Flow control activities {#flow-control}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Advanced workflow activities"
>abstract="You can now configure Test, JavaScript Code, and External Signal activities in a workflow. Use the Test activity to enable workflow transitions based on conditions. Add a JavaScript Code activity to execute a JS code snippet in the context of your workflow. Configure an External Signal activity to trigger the execution of your workflow from an API, or another workflow."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"



>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="End activity"
>abstract="The **End** activity allows you to graphically mark the end of a workflow. This activity has no functional impact and is therefore optional."

The following activities are specific to organizing and executing workflows. Their main task is to coordinate the other activities:

* [And-join](and-join.md): Synchronize multiple execution branches of a workflow.
* **End**: Graphically mark the end of a workflow. This activity has no functional impact and is therefore optional
* [External signal](external-signal.md): Trigger the execution of a workflow from another workflow, or an API call. 
* [Fork](fork.md): Create outbound transitions to start several activities at the same time.
* [Scheduler](scheduler.md): Schedule when the workflow gets started.
* [Test](test.md): Enable transitions based on specified conditions.
* [Wait](wait.md): Momentarily pause execution of a part of a workflow.
