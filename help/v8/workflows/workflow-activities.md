---
audience: end-user
title: Work with workflows activities
description: Learn how to workflow activities
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
---

# Workflow activities {#workflow-activities}

## Targeting activities {#targeting}

These activities let you build one or more targets by defining sets and splitting or combining these sets using intersection, union, or exclusion operations.

### Build audience {#build-audience}

This activity allows you to define an audience. You can either select an existing Campaign andience or use the rule builder to define your own query. 

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

Follow these steps to configure the **Build audience** activity:

1. Add a Build audience activity. 
1. Define a label.
1. Define the audience type: **Create your own** or **Read audience**. 

To create your own query, follow these extra steps:

1. Select **Create your own (query)**.
1. Choose the **Targeting dimension**. The targeting dimension lets you define the population targeted by the operation: recipients, contract beneficiaries, operator, subscribers, etc. By default, the target is selected from the recipients. Refer to the [v8 documentation](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Click **Continue**.
1. Use the rule builder to define your query, the same way you create an audience when designing a new email. Refer to this [section](../audience/segment-builder.md).

To select an existing audience, follow these steps:

1. Select **Read audience**.
1. Click **Continue**.
1. Select your audience, the same way you use an audience when designing a new email. Refer to this [section](../audience/add-audience.md).

### Combine {#combine}

This activity allows you to process sets on inbound data. You can thus combine several populations, exclude part of it or only keep data common to several targets. Here are the available segmentation types:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* The **Union** allows you to regroup the result of multiple activities into a single target.
* The **Intersection** allows you to keep only the elements common to the different inbound populations in the activity.
* The **Exclusion** allows you to exclude elements from one population according to certain criteria. 

Follow these steps to configure the **Combine** activity:

1. Add your **Combine** activity to any of the previous segmentation transitions.
1. Select the segmentation type: union, intersection or exclusion.
1. Click **Continue**.
1. In the **Sets to join** section, check all the previous activities you wish you join. 

For the **Union** and **Intersection**, you need to select the **Reconciliation type** to define how duplicates are handled:

    * Keys only: this is the default mode. The activity only keeps one element when elements from the different inbound transitions have the same key. This option can only be used if the inbound populations are homogeneous.
    * A selection of columns: select this option to define the list of columns on which the data reconciliation will be applied. You must first select the primary set (that which contains the source data), then the columns to use for the join.

For the **Intersection** and **Exclusion**, you can check the **Generate completement** option if you wish to process the remaining population. The complement will contain the union of the results of all inbound activities minus the intersection. An additional outbound transition will then be added to the activity.

For the **Exclusion**, select the **Primary set** from the inbound transitions, in the **Sets to join** section. This is the set from which elements are excluded. The other sets match elements before being excluded from the primary set.

### Enrichment {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enrichment activity"
>abstract="The Enrichment activity allows you to enhance the targeted data with additional information from the database. Itis commonly used in a workflow after targeting activities.<br/>Once enrichment data has been added to the workflow, it can be used in the activities added after the Enrichment activity to segment customers into distinct groups based on their behaviors, preferences, and needs, or to create personalized marketing messages and campaigns that are more likely to resonate with your target audience."

The Enrichment activity allows you to enhance the targeted data with additional information from the database. Itis commonly used in a workflow after targeting activities.

Enrichment data can come either:

* **From the same work table** as the one targeted into your workflow:

    *Target a group of customers and add the "Birth date" field to the current work table*

* **From another work table**:

    *Target a group of customers and add the "Amount" and "Type of product" fields coming from the "Purchase" table*.

Once the enrichment data has been added to the workflow, it can then be used in the activities added after the Enrichment activity to segment customers into distinct groups based on their behaviors, preferences, and needs,or to create personalized marketing messages and campaigns that are more likely to resonate with your target audience.

For instance, you can add to the workflow working table information related to customers' purchases and use this data to personalize emails with their latest purchase or the amount spent on these purchases.

To add an Enrichement activity into your workflow, follow these steps:

1. add activity
1. select attribute to use as enrichment data

    display advanced fields option
    i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    select an existing filter
    save the filter for reuse
    view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?

## Channel activities {#channel}

Adobe Campaign Web enables you to automate and execute marketing campaigns across multiple channels, such as email, SMS, or push. With Adobe Campaign  workflows, you can combine channel activities into the canvas to create cross-channel workflows that can trigger actions based on customer behavior. 

For example, you can create a welcome email campaign that includes a series of messages across different channels, such as email, SMS, and push. You can also send a follow-up email after a customer has completed a purchase or send a personalized birthday message to a customer via SMS. 

By using channel activities, you can create comprehensive, personalized campaigns that engage customers across multiple touchpoints and drive conversions.

Channel activities are available from the palette, on the left-hand side of the screen, in the Channels section.

### Email {#email}

description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow


The Email delivery activity allows you to configure the sending an email in a workflow. 

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### SMS {#sms}

### Push notification (Android) {#push-android}

### Push notification (iOS) {#push-ios}

## Flow control activities {#flow-control}

content TBD

<!--à reformuler-->These activities let you build one or more targets by defining sets and splitting or combining these sets using intersection, union, or exclusion operations.

Flow control activities are used to coordinate the workflow activities.

### Fork {#fork}

### AND-join {#join}


### Wait {#wait}

### End {#end}

## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section

