---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
---

# Create a workflow {#create}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Workflow properties"
>abstract="TBD"

## Create the workflow {#create-workflow}

The first step to create your workflow in Campaign v8 Web is to create it either as a standalone workflow or directly within a campaign and to define its general properties. To do so, follow these steps:

1. Start by deciding whether you want to create a standalone workflow or integrate it directly within a campaign:

    * **Standalone workflow**: Navigate to the Worklows menu and click the Create workflow button in the upper-right corner.
    * **Campaign workflow:** Navigate to the Campaigns menu and open the campaign where you want to create a new workflow. Click the Create workflow button in the upper-right corner of the Workflows tab.

    The workflow Properties dialog box appears.

    ![](assets/workflow-create.png)

1. Select the template to use to create the workflow and provide a label for the workflow.

    Workflow templates contain pre-configured activities and overall property configurations that can be reused for creating new workflows. They are created from the client console. [Learn how to work with templates](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

1. Expand the Additional options section if you want to configure specific settings for the workflow, such as the storing folder and timezone. [Learn how to configure worklow properties](workflow-settings.md)

1. Click the Create workflow button to confirm the creation of your workflow.

With your workflow created, you can now start orchestrating the various tasks it will perform using a dedicated visual canvas. [Learn how to orchestrate workflow activities](#build)

## Orchestrate workflow activities {#build}

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

Once you have completed the workflow, add en End activity at the end of the diagram. This activity allow you to visually mark the end of a workflow and has no functional impact.

After successfully designing the workflow diagram, you can execute the workflow and track the progress of its various tasks. [Learn how to start a workflow and monitor its execution](start-monitor-workflows.md)
