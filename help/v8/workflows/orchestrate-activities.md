---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
exl-id: 0c8e2158-518c-4620-9971-00ed2eccdd4f
---
# Orchestrate activities {#orchestrate}

Once that you have [created a workflow](create-workflow.md), wether from the workflow menu or within a campaign, you can start orchestrating the differents tasks it will perform. To do this, a visual canvas is provided, allowing you to construct a workflow diagram. Within this diagram, you can add various activities and connect them in a sequential order.

## Add activities {#add}

At this stage of the configuration, the diagram is displayed with a start icon, representing the beginning of your workflow. To add your first activity, click the **+** button connected to the start icon.

A list of activities that can be added to the diagram appears. The available activities depend on your position within the workflow diagram. For example, when adding your first activity, you can start your workflow by targeting an audience, splitting the workflow path, or setting a **Wait** activity to delay the workflow execution. On the other hand, after a **Build audience** activity, you can refine your target with targeting activities, send a delivery to your audience with channel activities, or organize the workflow process with flow control activities.

![](assets/workflow-start.png){zoomable="yes"}

Once an activity has been added to the diagram, a right pane appears, allowing you to configure the newly added activity with specific settings. Detailed information on how to configure each activity is available in [this section](activities/about-activities.md).

![](assets/workflow-configure-activities.png){zoomable="yes"}

Repeat this process to add as many activities as desired depending on the tasks that you want your workflow to perform. Note that you can also insert a new activity between two activities. To do this, click the **+** button on the transition between the activities, select the desired activity and configure it in the right pane.

To remove an activity, select it in the canvas and click the **Delete** icon in the activity properties.

>[!TIP]
>
>You have the option to personalize the name of the transitions between each activity. To do this, select the transition and change its label in the right pane.

## Manage activities {#manage}

When adding activities, action buttons are available in the properties pane, allowing you to perform multiple operations. You can:

* **Delete** the activity from the canvas.
* **Disable/Enable** the activity. When the workflow is executed, disabled activities and the following activities on the same path are not executed and the workflow is stopped.
* **Copy** the activity. You can then paste it in any workflow by cliking the **+** button on a transition and selecting "Paste 1 activity".
* Access the activity's **Logs and tasks**.
* **Pause/Resume** the activity. When the workflow is executed, it pauses at the paused activity. The corresponding task as well as all those that follow it in the same path are not executed.

![](assets/activity-action.png){zoomable="yes"}{width="50%"}

Several **Targeting** activities, such as **Combine** or **Deduplication**, allow you to process the remaining population and include it into an additional outbound transition. For example, if you're using a **Split** activity, the complement consists of the population that did not match any of the previously defined subsets. To use this capability, activate the **Generate complement** option. 

![](assets/workflow-split-complement.png)

## Example {#example}

Here is a workflow example designed to send an email to all customers (other than VIP customers) with an email who are interested in coffee machines.

![](assets/workflow-example.png){zoomable="yes"}{zoomable="yes"}

To achieve this, activities below have been added:

* A **[!UICONTROL Fork]** activity that divides the workflow into three paths (one for each set of customer),
* **[!UICONTROL Build audience]** activities to target the three sets of customers:

    * Customers with an email,
    * Customers belonging to the pre-existing "Interrested in Coffee Machine(s)" audience,
    * Customers belonging to the pre-existing "VIP ro reward" audience.

* A **[!UICONTROL Combine]** activity that groups together customers with an email and those interested in coffee machines,
* A **[!UICONTROL Combine]** activity that excludes VIP customers,
* An **[!UICONTROL Email delivery]** activity that sends an email to the resulting customers. 

Once you have completed the workflow, add en **[!UICONTROL End]** activity at the end of the diagram. This activity allow you to visually mark the end of a workflow and has no functional impact.

After successfully designing the workflow diagram, you can execute the workflow and track the progress of its various tasks. [Learn how to start a workflow and monitor its execution](start-monitor-workflows.md)
