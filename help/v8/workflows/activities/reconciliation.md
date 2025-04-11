---
audience: end-user
title: Use the Reconciliation workflow activity
description: Learn how to use the Reconciliation workflow activity
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
---
# Reconciliation {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Reconciliation activity"
>abstract="The **Reconciliation** activity is a **Targeting** activity that defines the link between the data in the Adobe Campaign database and the data in a work table. For example, the **Reconciliation** activity can be placed after a **Load file** activity to import non-standard data into the database. In this case, the **Reconciliation** activity defines the link between the data in the Adobe Campaign database and the data in the external table."

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

The **Reconciliation** activity is a **Targeting** activity that defines the link between the data in the Adobe Campaign database and the data in a work table, such as data loaded from an external file.

For example, the **Reconciliation** activity can be placed after a **Load file** activity to import non-standard data into the database. In this case, the **Reconciliation** activity defines the link between the data in the Adobe Campaign database and the data in the work table.

## Best practices {#reconciliation-best-practices}

While the **Enrichment** activity defines additional data to process in your workflow (for example, combining data from multiple sets or creating links to a temporary resource), the **Reconciliation** activity links unidentified data to existing resources.

>[!NOTE]
>Reconciliation operations require that the data of the linked dimensions already exist in the database. For example, if you import a file of purchases showing which product was purchased, at what time, and by which client, the product and the client must already exist in the database.

## Configure the Reconciliation activity {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Targeting dimension"
>abstract="Select the new targeting dimension. A dimension defines the targeted population: recipients, app subscribers, operators, subscribers, and more. By default, the current targeting dimension is selected."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Reconciliation rules"
>abstract="Select reconciliation rules for deduplication. To use attributes, select the **Simple attributes** option and choose the source and destination fields. To create your own reconciliation condition using the query modeler, select the **Advanced reconciliation conditions** option."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview" text="Work with the query modeler"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Select the targeting dimension"
>abstract="Select the targeting dimension for your inbound data to reconcile with."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html#targeting-dimensions" text="Targeting dimensions"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Keep unreconciled data"
>abstract="By default, non-reconciled data are kept in the outbound transition and available in the worktable for future use. To remove unreconciled data, deactivate the **Keep unreconciled data** option."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Reconciliation attribute"
>abstract="Select the attribute to use to reconcile data, and click Confirm."

Follow these steps to configure the **Reconciliation** activity:

1. Add a **Reconciliation** activity to your workflow. This activity should follow a transition containing a population whose targeting dimension does not directly come from Adobe Campaign.

1. Select the new targeting dimension. A dimension defines the targeted population: recipients, app subscribers, operators, subscribers, and more. [Learn more about targeting dimensions](../../audience/about-recipients.md#targeting-dimensions).

1. Select the field(s) to use for the reconciliation. You can use one or more reconciliation criteria.

    1. To use attributes to reconcile data, select the **Simple attributes** option. The **Source** field lists the fields available in the input transition, which are to be reconciled. The **Destination** field corresponds to the fields of the selected targeting dimension. Data are reconciled when the source and destination are equal. For example, select the **Email** fields to deduplicate profiles based on their email address.

        To add another reconciliation criterion, click the **Add rule** button. If several join conditions are specified, they must all be verified for the data to be linked together.

        ![Reconciliation criteria example](../assets/workflow-reconciliation-criteria.png)

    1. To use other attributes to reconcile data, select the **Advanced reconciliation conditions** option. You can then create your own reconciliation condition using the query modeler. [Learn how to work with the query modeler](../../query/query-modeler-overview.md).

1. Filter data to reconcile using the **Create filter** button. This lets you create a custom condition using the query modeler. [Learn how to work with the query modeler](../../query/query-modeler-overview.md).

By default, non-reconciled data are kept in the outbound transition and available in the worktable for future use. To remove unreconciled data, deactivate the **Keep unreconciled data** option.

## Example {#reconciliation-example}

The following example demonstrates a workflow that creates an audience of profiles directly from an imported file containing new clients. It includes the following activities:

The workflow is designed as follows:

![Workflow example](../assets/workflow-reconciliation-sample-1.0.png)

It is built with the following activities:

* A [Load file](load-file.md) activity uploads a file containing profile data extracted from an external tool.

    For example:

    ```
    lastname;firstname;email;birthdate;
    JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
    PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
    WEAVER;Justin;justin_w@testmail.com;11/15/1990;
    MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
    REESE;Richard;rreese@testmail.com;02/08/1987;
    ```

* A **Reconciliation** activity identifies the incoming data as profiles by using the **Email** and **Date of birth** fields as reconciliation criteria.

    ![Reconciliation activity example](../assets/workflow-reconciliation-sample-1.1.png)

* A [Save audience](save-audience.md) activity creates a new audience based on these updates. You can also replace the **Save audience** activity with an **End** activity if no specific audience needs to be created or updated. Recipient profiles are updated in any case when you run the workflow.

## Compatibility {#reconciliation-compat}

The **Reconciliation** activity does not exist in the Client console. All **Enrichment** activities created in the Client console with the reconciliation options enabled are displayed as **Reconciliation** activities in the Campaign Web user interface.