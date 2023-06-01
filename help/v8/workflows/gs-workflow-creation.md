---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
---

# Key principles of workflow creation {#gs-workflow-creation}

With Campaign v8 Web, you can build workflows into a visual canvas to design cross-channel processes such as segmentation, campaign execution, file processing.

Workflows can be created either as standalone workflows, from the Workflows menu, or directly within a campaign, in which case the workflow will be linked to the campaign and executed along with all the other campaign's workflows.

## What's inside a workflow?

The workflow diagram is a representation of what is supposed to happen. It describes the various tasks to be performed and how they are linked together. 

![](assets/workflow-example.png)

Each workflow contains:

* **Activities**: An activity is a task to be performed. The various activities are represented on the diagram by icons. Each activity has specific properties and other properties that are common to all activities.

    In a workflow diagram, a given activity can produce multiple tasks, in particular when there is a loop or recurrent actions.

* **Transitions**: Transitions link a source activity to a destination activity and define their sequence. 

* **Worktables**: The worktable contains all the information carried by the transition. Each workflow uses several worktables. The data conveyed in these tables can be used throughout the workflow’s life cycle.

## Main steps to create a workflow

The main steps to create workflows are as follows:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="create-workflow.md#create">
<img alt="Lead" src="assets/do-not-localize/workflow-process-1.jpeg">
</a>
<div><a href="create-workflow.md#create"><strong>Create the workflow</strong>
</div>
<p>
</td>
<td>
<a href="create-workflow.md#build">
<img alt="Infrequent" src="assets/do-not-localize/workflow-process-2.jpeg">
</a>
<div>
<a href="create-workflow.md#build"><strong>Orchestrate activities</strong></a>
</div>
<p></td>
<td>
<a href="workflow-settings.md">
<img alt="Validation" src="assets/do-not-localize/workflow-process-3.jpeg">
</a>
<div>
<a href="workflow-settings.md"><strong>Configure advanced settings (optional)</strong></a>
</div>
<p>
</td>
<td>
<a href="start-monitor-workflows.md">
<img alt="start and monitor workflows" src="assets/do-not-localize/workflow-process-4.jpeg">
</a>
<div>
<a href="start-monitor-workflows.md"><strong>Start & monitor the workflow execution</strong></a>
</div>
<p>
</td>
</tr></table>