---
audience: end-user
title: Use the Reconciliation workflow activity
description: Learn how to use the Reconciliation workflow activity
badge: label="Limited Availability"
---
# Reconciliation {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Reconciliation activity"
>abstract="The **Reconciliation** activity is a **Targeting** activity. It allows you to link unidentified data to existing resources. For example, the **Reconciliation** activity can be placed after a **Load audience** activity to import non-standard data into the database. In this case, the **Reconciliation** activity lets you define the link between the data in the Adobe Campaign database and the data in the work table." 


>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Reconciliation select field"
>abstract="Reconciliation select field" 


>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Reconciliation create condition"
>abstract="Reconciliation create condition" 

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Reconciliation generate complement"
>abstract="Reconciliation generate complement" 

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Reconciliation keep unreconciled data option"
>abstract="Reconciliation keep unreconciled data option" 


The **Reconciliation** activity is a **Targeting** activity. It allows you to link unidentified data to existing resources. For example, the **Reconciliation** activity can be placed after a **Load audience** activity to import non-standard data into the database. In this case, the **Reconciliation** activity lets you define the link between the data in the Adobe Campaign database and the data in the work table.


## Best practices {#reconciliation-best-practices}

While the **Enrichment** activity allows you to define additional data to process in your workflow (you can use an **Enrichment** activity to combine data coming from multiple sets, or to create links to a temporary resource), the **Reconciliation** activity allows you to link unidentified data to existing resources. 

>[!NOTE]
>Reconciliation operation implies that the data of the linked dimensions are already in the database.  For example, if you import a file of purchases showing which product was purchased, at what time, by which client, etc., the product as well as the client must already exist in the database.
>

## Configure the Reconciliation activity {#reconciliation-configuration}


>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Targeting dimension"
>abstract="Select the new targeting dimension. A dimension lets you define the targeted population: recipients, app subscribers, operators, subscribers, etc. By default, the current targeting dimension is selected." 

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Reconciliation rules"
>abstract="Select the reconciliation field(s) to use for the deduplication. You can use one or more reconciliation criteria." 

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Select the targeting dimension"
>abstract="Select the targeting dimension for your inbound data to reconcile with." 
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/about-recipients.html?lang=en#targeting-dimensions" text="Targeting dimensions"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Keep unreconciled data"
>abstract="By default, non reconciled data are kept in the outbound transition and available in the worktable for future use. To remove unreconciled data, desactivate the **Keep unreconciled data** option." 


>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Reconciliation attribute"
>abstract="Select the attribute to use to reconciliate data, and click Confirm." 

Follow these steps to configure the **Reconciliation** activity:

1. Drag and drop a **Reconciliation** activity into your workflow. This activity should be added following a transition containing a population whose targeting dimension does not directly come from Adobe Campaign. 

1. Select the new targeting dimension. A dimension lets you define the targeted population: recipients, app subscribers, operators, subscribers, etc. Learn more about targeting dimensions in [this page](../../audience/about-recipients.md#targeting-dimensions).

1. Select the reconciliation field(s) to use for the deduplication. You can use one or more reconciliation criteria.

    1. To use attributes to reconcile data, select the **Simple attributes** option. For example, select the **Email** fields to deduplicate profiles based on their email address. The **Source** field lists the fields available in the input transition, which are to be reconcilied. The **Destination** field corresponds to the fields of the selected targeting dimension. Data are reconcilied when source and destination are equal.
        
        To add another reconciliation criteria, click the **Add rule** button. If several join conditions are specified, they must ALL be verified so that the data can be linked together.    

        ![](../assets/workflow-reconciliation-criteria.png)

    1. To use other attributes to reconcile data, select the **Advanced reconciliation conditions** option. You can then create your own reconciliation condition using the query modeler. Learn how to use the query modeler in [this section](../../query/query-modeler-overview.md).

1. You can filter data to reconciliate using the **Create filter** button. This lets you create a custom condition using the [query modeler](../../query/query-modeler-overview.md).

By default, non reconcilied data are kept in the outbound transition and available in the worktable for future use. To remove unreconciled data, desactivate the **Keep unreconciled data** option.

## Example {#reconciliation-example}

In the following example, the activity is configured so that the workflow 


## Compatibility {#reconciliation-compat}

The **Reconciliation** activity does not exist in the Client console. All **Enrichments** activities created in the Client console with the reconciliation options enabled are displayed as **Reconciliation** activities in Campaign Web UI.
