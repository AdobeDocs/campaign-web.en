---
audience: end-user
title: Use the AND-join workflow activity
description: Learn how to use the AND-join workflow activity
badge: label="Alpha" type="Positive"
---

# AND-join {#join}

The **And-join** activity allows you to synchronize multiple execution branches of a workflow.

The AND-join activity only triggers its outbound transition once all the inbound transitions are activated, in other words, once all of the preceding activities have finished.

## Configuration

Follow these steps to configure the **AND-join** activity:

1. Add multiple activities such as **Combine** activities to form at least two different execution branches.
1. Add an **AND-join** activity to any of the branches.
1. In the **Merging options** section, check all the previous activities you wish you join. 
1. Select the **Primary set** to be kept in the outbound transition. 

## Example

The following example shows two workflow branches with an email and SMS delivery. The AND-join will trigger when both inbound transitions are enabled. The push notifications will then be sent only after both deliveries are finished. 

![](../assets/workflow-andjoin-example.png)