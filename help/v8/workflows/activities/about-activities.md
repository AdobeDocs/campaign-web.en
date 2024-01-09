---
audience: end-user
title: Work with workflows activities
description: Learn how to workflow activities
badge: label="Limited Availability" 
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
---

# About workflow activities {#workflow-activities}

Workflow activities are grouped into three categories. Depending on the context, available activities may differ. 

All activities are detailed in the sections below:

* [Targeting and data management activities](#targeting)
* [Channel activities](#channel)
* [Flow control activities](#flow-control)

![](../assets/workflow-activities.png)

## Targeting and data management activities {#targeting}

These activities are specific to targeting, manipulating and enriching population data. They let you build one or more targets by defining an audience and splitting or combining these audiences using intersection, union or exclusion operations.

* Use the [Save audience](save-audience.md) activity to update an existing audience or create a new audience from the population computed upstream in a workflow.
* Use the [Build audience](build-audience.md) activity to define your target population. You can either select an existing audience or use the rule builder to define your own query. 
* Use the [Combine](combine.md) activity to perform segmentation on your inbound population. You can use a union, an intersection or an exclusion.
* Use the [Split](split.md) activity to segment incoming population into several subsets.
* Use the [Reconciliation](reconciliation.md) activity to define the link between the data in the Adobe Campaign database and the data in a work table, for example data loaded from an external file.
* Use the [Enrichment](enrichment.md) activity to define additional data to process in your workflow. With this activity, you can leverage the inbound transition and configure the activity to complete the output transition with additional data.
* Use the [Deduplication](deduplication.md) activity to delete duplicates in the result(s) of the inbound activities.
* Use the [Change dimension](change-dimension.md) activity to change the targeting dimension as you are building your workflow.
* Use the [Load file](load-file.md) activity to work with profiles and data stored in an external file. 


## Channel activities {#channel}

Adobe Campaign Web allows you to automate and execute marketing campaigns across multiple channels. You can combine channel activities into the canvas to create cross-channel workflows that can trigger actions based on customer behavior. The following **Channel** activities are available: Email, SMS, Android and iOS Push notifications. [Learn how to set up a delivery in the context of a workflow](channels.md).

## Flow control activities {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="End activity"
>abstract="The **End** activity allows you to graphically mark the end of a workflow. This activity has no functional impact and is therefore optional."

The following activities are specific to organizing and executing workflows. Their main task is to coordinate the other activities:

* Use the [Scheduler](scheduler.md) activity to schedule when the workflow gets started.
* Use the [And-join](and-join.md) activity to synchronize multiple execution branches of a workflow.
* Add an **End** activity to graphically mark the end of a workflow. This activity has no functional impact and is therefore optional.
* Use the [Fork](fork.md) activity to create outbound transitions to start several activities at the same time.
* Add a [Wait](wait.md) activity to momentarily pause execution of a part of a workflow.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

