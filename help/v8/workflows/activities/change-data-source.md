---
audience: end-user
title: Use the Change Data Source workflow activity
description: Learn how to use the Change Data Source workflow activity
---
# Change Data Source {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="Change Data Source"
>abstract="The **Change Data Source** activity allows you to select a different data source for the Working table of your workflow."

The **Change Data Source** activity is a **targeting** activity. This activity allows you to change the data source used by your workflow Working table. This provides more flexibility by allowing you to manage data across your different databases.

>[!AVAILABILITY]
>
>The **[!UICONTROL Change Data Source]** activity is available with the "Access to external data (Federated Data Access)" package only. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html){target="_blank"}

## What is a Working table {#working-table}

In workflows, data is transported from one activity to another is stored in a temporary **Working table**. By default, Working tables are created in the same database as the source of the data we query on. For example, when querying the "Profiles" table, stored on the Cloud database, a Working table is automatically created on the same Cloud database.

To change this, you can add a **Change Data Source **activity to choose a different data source for your Working table. This allows you to leverage data from external databases to perform operations such as enrichment or querying. 

Note that, after changing the data source of your Working table, you need to switch it back to the Cloud database to continue the workflow execution by adding another **Change Data Source** activity.

## Configure the Change Data Source activity {#configure}

Follow these steps to configure the **Change dimension** activity:

1. Add a **Change Data Source** activity to your workflow.

   ![](../assets/workflow-change-dimension.png)

1. Define the data source where you want to move the worklow Working table:

   * **[!UICONTROL Default Campaign database (PostgreSQL)]**: Use the default Campaign database.
   * **[!UICONTROL FDA external account]**: Use external databases connected to Adobe Campaign through Federated Data Access capability.

      >[!AVAILABILITY]
      >
      >Campaign configuration and connection to external systems are restricted to advanced users and only available from the client console. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html){target="_blank"}

1. Configure your workflow to perform the desired operations using the new data source.

   Once done, switch back the Working table data sourcev to the Campaign Cloud database to continue the workflow execution. To do this, add a new **[!UICONTROL Change Data Source]** activity to the workflow and select the **FDA external account** data source.

<!--## Example {#example}

In this example, we want to-->
