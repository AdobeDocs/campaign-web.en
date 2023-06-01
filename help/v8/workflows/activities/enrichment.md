---
audience: end-user
title: Use the Enrichment workflow activity
description: Learn how to use the Enrichment workflow activity
badge: label="Alpha" type="Positive"
---

# Enrichment {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enrichment activity"
>abstract="The Enrichment activity allows you to enhance the targeted data with additional information from the database. It is commonly used in a workflow after targeting activities.<br/>Once enrichment data has been added to the workflow, it can be used in the activities added after the Enrichment activity to segment customers into distinct groups based on their behaviors, preferences, and needs, or to create personalized marketing messages and campaigns that are more likely to resonate with your target audience."

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

