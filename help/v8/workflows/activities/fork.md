---
audience: end-user
title: Use the Fork workflow activity
description: Learn how to use the Fork workflow activity
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
---

# Fork {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Fork activity"
>abstract="The **Fork** activity allows you to create outbound transitions to start several activities at the same time."

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Fork activity transitions"
>abstract="By default, two transitions are created with a **Fork** activity. Click the **Add transition** button to define an additional outbound transition, and enter its label."

The **Fork** activity is a **Flow control** activity. It enables you to create outbound transitions to start several activities simultaneously.

## Configure the Fork activity {#fork-configuration}

Follow these steps to configure the **Fork** activity:

![Workflow fork activity configuration screenshot](../assets/workflow-fork.png)

1. Add a **Fork** activity to your workflow.
1. Click **Add transition** to add a new outbound transition. By default, two transitions are defined.
1. Add a label to each transition.

## Example {#fork-example}

In the following example, two **Fork** activities are used:

* One before the two queries, to execute them simultaneously.
* One after the intersection, to send an email and an SMS at the same time to the targeted population.

![Workflow fork example screenshot](../assets/workflow-fork-example.png)
```