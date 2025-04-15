---
audience: end-user
title: Use the Update data workflow activity
description: Learn how to use the Update data workflow activity
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
---
# Update data {#update-data}

The **Update data** activity is a **Data Management** activity. It enables you to perform a mass update on fields in the database. Several options allow you to customize the data update.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update it if it has already been added. You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely.

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or directly use reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section lets you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example, if there is a duplicate). The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.
-->

## Configure the Update data activity {#update-data-configuration}

To configure the **Update data** activity, add the activity to your workflow and define a label.

![Workflow Update Data Activity](../assets/workflow-update-data.png)

### Operation type

The **Operation type** field lets you choose the process to be carried out on the data in the database:

* **Insert or update**: Insert data or update it if the records already exist in the database.
* **Insert**: Insert data only. Records that already exist are not updated. If reconciliation criteria are defined, only the non-reconciled records will be added.
* **Update**: Update data of the records that already exist in the database only.
* **Delete**: Delete data.

The **Batch size** field lets you select the number of inbound transition elements to be updated. For example, if you specify 500, the first 500 records processed will be updated.

### Record identification

This section allows you to specify how to identify the records in the database:

* If data entries relate to an existing targeting dimension, select the **Using the targeting dimension** option, and choose it in the **Targeting dimension to update** field.
* You can also select **Using custom links** and specify one or more links that will enable identification of the data in the database.
* If the operation type selected requires an update, use the **Using reconciliation rules** option.

### Fields to update

In the **Fields to update** section, add the fields on which the update will be applied. If necessary, add conditions so that this update is carried out. Use the **Taken into account if** field to define conditions. Conditions are applied sequentially in list order. Use the arrows on the right to change the order of the updates. You can use the same destination field multiple times.

Automatically link fields using the **Auto-mapping** button. Automatic linking detects fields with the same name.

During an **Insert or update** operation type, individually select the operation to apply for each field. Use the **Operation type** field to specify the desired value.

### Advanced options

The **Advanced options** section lets you specify additional options to handle updating data and managing duplicates.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

The last two options allow you to perform specific actions:

* **Generate an outbound transition**: Creates an outbound transition that will be activated at the end of execution. Updating usually signals the end of a targeting workflow, and the option is therefore not activated by default.

* **Generate an outbound transition for the rejects**: Creates an outbound transition containing records that have not been correctly processed after the update (for example, if there is a duplicate). The update generally marks the end of a targeting workflow, and the option is not activated by default.