---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
---

# Key principles of workflow creation {#gs-workflow-creation}

With Campaign v8 Web, you can build workflows into a visual canvas to design cross-channel processes such as segmentation, campaign execution, file processing.

Workflows can be created either as standalone workflows, from the Workflows menu, or from within a campaign, form the Campaigns menu.

TBD: detail specificities between standalone & campaign workflows.

## What's inside a workflow?

The workflow diagram is a representation of what is supposed to happen. It describes the various tasks to be performed and how they are linked together. 

Each workflow contains:

* **Activities**: An activity is a task to be performed. The various activities are represented on the diagram by icons. Each activity has specific properties and other properties that are common to all activities.

    In a workflow diagram, a given activity can produce multiple tasks, in particular when there is a loop or recurrent actions.

* **Transitions**: Transitions link a source activity to a destination activity and define their sequence. 

* **Worktables**: The worktable contains all the information carried by the transition. Each workflow uses several worktables. The data conveyed in these tables can be accelerated and used throughout the workflow’s life cycle, as long as it is not purged. Indeed, unneeded tables are purged each time the workflow is passivated, and possibly during the execution of the largest workflows to avoid overloading the server.

## Main steps to create a workflow

The main steps to create workflows are as follows:

TBD: graphic showing the whole process with explanation and ref to doc pages

create and define properties > orchestrate activities in the canvas > configure settings if needed > start the execution and monitor