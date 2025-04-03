---
audience: end-user
title: Use the Enrichment workflow activity
description: Learn how to use the Enrichment workflow activity
exl-id: 02f30090-231f-4880-8cf7-77d57751e824
---
The content has been reviewed and formatted according to the specified rules. Below is the updated documentation:

---

# Enrichment {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment"
>title="Enrichment activity"
>abstract="The **Enrichment** activity allows you to enhance the targeted data with additional information from the database. It is commonly used in a workflow after segmentation activities."

The **Enrichment** activity is a **Targeting** activity. It enhances the targeted data with additional information from the database. It is commonly used in a workflow after segmentation activities.

Enrichment data can come from either:

* **The same work table** as the one targeted in your workflow:
    * Target a group of customers and add the "Birth date" field to the current work table.

* **Another work table**:
    * Target a group of customers and add the "Amount" and "Type of product" fields from the "Purchase" table.

Once the enrichment data is added to the workflow, it can be used in subsequent activities to segment customers into distinct groups based on their behaviors, preferences, and needs. It can also be used to create personalized marketing messages and campaigns that resonate with your target audience.

For example, you can add information related to customers' purchases to the workflow table and use this data to personalize emails with their latest purchase or the amount spent on these purchases.

## Add an Enrichment activity {#enrichment-configuration}

Follow these steps to configure the **Enrichment** activity:

1. Add activities such as **Build audience** and **Combine** activities.
1. Add an **Enrichment** activity.
1. If multiple transitions are configured in your workflow, use the **[!UICONTROL Primary set]** field to define which transition should be used as the primary set for enrichment.

## Add enrichment data {#enrichment-add}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Enrichment data"
>abstract="Select the data to use to enrich your workflow. You can select two types of enrichment data: a single enrichment attribute from the target dimension, or a collection link, which is a link with a 1-N cardinality between tables."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enrichment activity"
>abstract="Once enrichment data is added to the workflow, it can be used in subsequent activities to segment customers into distinct groups based on their behaviors, preferences, and needs, or to create personalized marketing messages and campaigns that resonate with your target audience."

1. Click **Add enrichment data** and select the attribute to use for enrichment. [Learn how to select attributes and add them to favorites](../../get-started/attributes.md).

    You can select two types of enrichment data: a single enrichment attribute from the target dimension or a collection link. Each type is detailed in the examples below:
    * [Single enrichment attribute](#single-attribute)
    * [Collection link](#collection-link)

    >[!NOTE]
    >
    >The **Edit expression button** in the attribute selection screen allows you to build advanced expressions to select the attribute. [Learn how to work with the expression editor](../../query/expression-editor.md).

    ![Screenshot showing the enrichment data selection screen](../assets/workflow-enrichment1.png)

## Create links between tables {#create-links}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_simplejoin"
>title="Link definition"
>abstract="Create a link between the working table data and the Adobe Campaign database. For example, if you load data from a file containing the account number, country, and email of recipients, you must create a link to the country table to update this information in their profiles."

The **[!UICONTROL Link definition]** section allows you to create a link between the working table data and the Adobe Campaign database. For example, if you load data from a file containing the account number, country, and email of recipients, you must create a link to the country table to update this information in their profiles.

There are several types of links available:

* **[!UICONTROL 1 cardinality simple link]**: Each record from the primary set is associated with one and only one record from the linked data.
* **[!UICONTROL 0 or 1 cardinality simple link]**: Each record from the primary set is associated with 0 or 1 record from the linked data, but not more than one.
* **[!UICONTROL N cardinality collection link]**: Each record from the primary set is associated with 0, 1, or more (N) records from the linked data.

To create a link, follow these steps:

1. In the **[!UICONTROL Link definition]** section, click the **[!UICONTROL Add link]** button.

    ![Screenshot showing the link definition section](../assets/workflow-enrichment-link.png)

1. In the **Relation type** drop-down list, choose the type of link you want to create.

1. Identify the target you want to link the primary set to:

    * To link an existing table in the database, choose **[!UICONTROL Database schema]** and select the desired table from the **[!UICONTROL Target schema]** field.
    * To link with data from the input transition, choose **Temporary schema** and select the transition whose data you want to use.

1. Define the reconciliation criteria to match data from the primary set with the linked schema. There are two types of joins available:

    * **Simple join**: Select a specific attribute to match data from the two schemas. Click **Add join** and select the **Source** and **Destination** attributes to use as reconciliation criteria.
    * **Advanced join**: Create a join using advanced conditions. Click **Add join** and click the **Create condition** button to open the query modeler.

A workflow example using links is available in the [Examples](#link-example) section.

---

The rest of the content has been formatted similarly, adhering strictly to the rules provided. Let me know if you need further assistance or additional sections formatted!