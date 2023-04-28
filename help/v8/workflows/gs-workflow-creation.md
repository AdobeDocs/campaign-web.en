---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
---

# Key principles of workflow creation {#gs-workflow-creation}

content TBD

A workflow is a process definition: the workflow diagram, which is a representation of what is supposed to happen. A workflow is also an instance of this process: a workflow instance, which is a representation of what is actually happening.

The workflow template describes the various tasks to be performed and how they are linked together. The task templates are called activities and are represented by icons. They are linked together by transitions.

screenshot TBD 

## What's inside a workflow?

Each workflow contains:

* **Activities**: An activity describes a task template. The various activities available are represented on the diagram by icons. Each type has common properties and specific properties.

    In a workflow diagram, a given activity can produce multiple tasks, in particular when there is a loop or recurrent actions.

* **Transitions**: Transitions enable you to link activities and define their sequence. A transition links a source activity to a destination activity. 

* **Worktables**: The worktable contains all the information carried by the transition. Each workflow uses several worktables. The data conveyed in these tables can be accelerated and used throughout the workflow’s life cycle, as long as it is not purged. Indeed, unneeded tables are purged each time the workflow is passivated, and possibly during the execution of the largest workflows to avoid overloading the server.

## Standalone and campaign workflows

Workflows can be created either as standalone workflows, or from within a campaign.

TBD: detail specificities between standalone & campaign workflows.

## Main steps to create a workflow

The main steps to create workflows are as follows:

TBD: graphic showing the whole process with explanation and ref to doc pages

create and define properties > orchestrate activities in the canvas > configure settings if needed > start the execution and monitor