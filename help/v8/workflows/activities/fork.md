---
audience: end-user
title: Use the Fork workflow activity
description: Learn how to use the Fork workflow activity
badge: label="Alpha" type="Positive"
---

# Fork {#fork}

The **Fork** activity allows you to create outbound transitions to start several activities at the same time.

The **Fork** activity allows you to carry out several different activities independently within the same workflow.

## Configuration

Follow these steps to configure the **Fork** activity:

1. Add a **Fork** activity to your workflow.
1. Click **Add transition** to add a new outbound transition. By default two transitions are defined.
1. Add a label to each of your transitions. 

## Example

The following example, we're using two **Fork** activities:

* One before the two queries, to execute them at the same time.
* One after the intersection, to send an email and an SMS simultaneously to the targeted population.

![](../assets/workflow-fork-example.png)

