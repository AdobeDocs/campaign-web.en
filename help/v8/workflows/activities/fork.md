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

The **Fork** activity is a **Flow control** activity. It allows you to create outbound transitions to start several activities at the same time.

## Configure the Fork activity{#fork-configuration}

Follow these steps to configure the **Fork** activity:

![](../assets/workflow-fork.png)

1. Add a **Fork** activity to your workflow.
1. Click **Add transition** to add a new outbound transition. By default two transitions are defined.
1. Add a label to each of your transitions. 

## Example{#fork-example}

In the following example, we're using two **Fork** activities:

* One before the two queries, to execute them at the same time.
* One after the intersection, to send an email and an SMS simultaneously to the targeted population.

![](../assets/workflow-fork-example.png)
