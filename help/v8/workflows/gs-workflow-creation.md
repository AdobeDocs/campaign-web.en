---
audience: end-user
title: Key principles of workflow creation
description: Learn key principles of workflows with Adobe Campaign Web
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
---

# Key principles of workflow creation {#gs-workflow-creation}

With Adobe Campaign Web, you can build workflows into a visual canvas to design cross-channel processes such as segmentation, campaign execution, file processing.

## What's inside a workflow? {#gs-workflow-inside}

The workflow diagram is a representation of what is supposed to happen. It describes the various tasks to be performed and how they are linked together. 

![](assets/workflow-example.png){zoomable="yes"} {zoomable="yes"}

Each workflow contains:

* **Activities**: An activity is a task to be performed. The various activities are represented on the diagram by icons. Each activity has specific properties and other properties that are common to all activities.

    In a workflow diagram, a given activity can produce multiple tasks, in particular when there is a loop or recurrent actions.

* **Transitions**: Transitions link a source activity to a destination activity and define their sequence. 

* **Worktables**: The worktable contains all the information carried by the transition. Each workflow uses several worktables. The data conveyed in these tables can be used throughout the workflow's life cycle.

## Key steps to create a workflow {#gs-workflow-steps}


Campaigns offers two ways to create a workflow:

1. Workflows can be created as standalone workflows, from the **Workflows** menu.

    ![](assets/create-a-standalone-wf.png){zoomable="yes"}

1. Workflows can be created directly within a campaign, from the **Workflow** tab of the campaign. When included in a campaign, the workflow is executed along with all the other campaign's workflows, and the reporting metrics are all grouped at the campaign level.

    ![](assets/create-a-wf-from-a-campaign.png){zoomable="yes"}
    
Key steps to create workflows are as follows:

![](assets/workflow-creation-process.png){zoomable="yes"}

These steps are detailed in the following section:

1. [Create your workflow and define its properties](create-workflow.md)
1. [Orchestrate and configure activities](orchestrate-activities.md)
1. [Configure your workflow advanced settings](workflow-settings.md)
1. [Start your workflow and monitor its execution](start-monitor-workflows.md)
