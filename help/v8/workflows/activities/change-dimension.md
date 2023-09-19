---
audience: end-user
title: Use the Change dimension workflow activity
description: Learn how to use the Change dimension workflow activity
badge: label="Beta" 
---

# Change dimension {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generate a complement"
>abstract="You can generate an additional outbound transition with the remaining population, which was excluded as a duplicate. To do this, toggle on the **Generate complement** option"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Change dimension activity"
>abstract="This activity allows you to change the targeting dimension as you are building an audience. It shifts the axis depending on the data template and the input dimension. For example, you can switch from the "contracts" dimension to the "clients" dimension."

The **Change dimension** activity is a **Targeting** activity. This activity allows you to change the targeting dimension as you are building an audience. This activity shifts the axis depending on the data template and the input dimension. For example, you can switch from the "contracts" dimension to the "clients" dimension.

## Configuration

Follow these steps to configure the **Change dimension** activity:

1. Add a **Change dimension** activity to your workflow.

   ![](../assets/workflow-change-dimension.png)

1. Define the **New target dimension**. During dimension change, all records are kept. Other options are not available yet. 

1. Execute the workflow to view the result. Compare the data in the tables before and after the change dimension activity, and compare the structure of the workflow tables.



