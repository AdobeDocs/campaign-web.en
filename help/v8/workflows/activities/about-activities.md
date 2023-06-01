---
audience: end-user
title: Work with workflows activities
description: Learn how to workflow activities
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
---

# About workflow activities {#workflow-activities}

Workflow activities are grouped into three categories. Depending on the context, available activities may differ. 

All activities are detailed in the sections below:

* [Targeting activities](#targeting)
* [Channel activities](#channel)
* [Flow control activities](#flow-control)

![](../assets/workflow-activities.png)

## Targeting activities {#targeting}

These activities are specific to targeting, manipulating and enriching population data. They let you build one or more targets by defining an audience and splitting or combining these audiences using intersection, union or exclusion operations.

* The [Build audience](build-audience.md) activity allows you define your target population. You can either select an existing audience or use the rule builder to define your own query. 
* The [Combine](combine.md) activity allows to perform segmentation on your inbound population. You can use a union, an intersection or an exclusion.
* The [Enrichment](enrichment.md) activity allows you to define additional data to process in your workflow. With this activity, you can leverage the inbound transition and configure the activity to complete the output transition with additional data.

## Channel activities {#channel}

Adobe Campaign Web enables you to automate and execute marketing campaigns across multiple channels, such as email, SMS, or push. With Adobe Campaign workflows, you can combine channel activities into the canvas to create cross-channel workflows that can trigger actions based on customer behavior. 

For example, you can create a welcome email campaign that includes a series of messages across different channels, such as email, SMS, and push. You can also send a follow-up email after a customer has completed a purchase or send a personalized birthday message to a customer via SMS. 

By using channel activities, you can create comprehensive, personalized campaigns that engage customers across multiple touchpoints and drive conversions.

* [Email](email.md)
* [Push](push.md)
* [SMS](sms.md)

## Flow control activities {#flow-control}

The following activities are specific to organizing and executing workflows. Their main task is to coordinate the other activities:

* The [And-join](and-join.md) activity allows you to synchronize multiple execution branches of a workflow.
* The [End](end.md) activity allows you to graphically mark the end of a workflow. This activities have no functional impact and is therefore optional.
* The [Fork](fork.md) activity allows you to create outbound transitions to start several activities at the same time.
* The [Wait](wait.md) activity momentarily suspends executing a part of a workflow.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

