---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
badge: label="Alpha" type="Positive"
---

# Orchestrate activities {#orchestrate}

Once that you have [created a workflow](create-workflow.md), wether from the workflow menu or within a campaign, you can start orchestrating the differents tasks it will perform. To do this, a visual canvas is provided, allowing you to construct a workflow diagram. Within this diagram, you can add various activities and connect them in a sequential order.

At this stage of the configuration, the diagram is displayed with a start icon, representing the beginning of your workflow. To add your first activity, click the + button connected to the start icon.

A list of activities that can be added to the diagram appears. The available activities depend on your position within the workflow diagram. For example, when adding your first activity, you can start your workflow by targeting an audience, splitting the workflow path, or setting a Wait activity to delay the workflow execution. On the other hand, after a Build audience activity, you can refine your target with targeting activites, send a delivery to your audience with channel activites, or organize the workflow process with flow control activities.

![](assets/workflow-start.png)

Once an activity has been added to the diagram, a right pane appears, allowing you to configure the newly added activity with specific settings. Detailed information on how to configure each activity is available in [this section](activities/about-activities.md).

![](assets/workflow-configure-activities.png)

Repeat this process the add as many activites as desired depending on the tasks that you want your workflow to perform. Note that you can also insert a new activity between two activites. To do this, click the + button on the transition between the activities, select the desired activity and configure it in the right pane.

To remove an activity, select it in the canvas and click the Delete icon in the activity properties.

>[!TIP]
>
>You have the option to personalize the name of the transitions between each activity. To do this, select the transition and change its label in the right pane.

Here is a workflow example designed to send an email to all customers (other than VIP customers) with an email who are interested in coffee machines.

![](assets/workflow-example.png)

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
