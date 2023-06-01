---
audience: end-user
title: Use the Combine workflow activity
description: Learn how to use the Combine workflow activity
badge: label="Alpha" type="Positive"
---

# Combine {#combine}

This activity allows you to process sets on inbound data. You can thus combine several populations, exclude part of it or only keep data common to several targets. Here are the available segmentation types:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

   * The **Union** allows you to regroup the result of multiple activities into a single target.
   * The **Intersection** allows you to keep only the elements common to the different inbound populations in the activity.
   * The **Exclusion** allows you to exclude elements from one population according to certain criteria. 

## Configuration

Follow these steps to configure the **Combine** activity:

1. Add multiple activities such as **Build audience** activities to form at least two different execution branches.
1. Add a **Combine** activity to any of the previous segmentation transitions.
1. Select the segmentation type: union, intersection or exclusion.
1. Click **Continue**.
1. In the **Sets to join** section, check all the previous activities you wish you join. 

For the **Union** and **Intersection**, you need to select the **Reconciliation type** to define how duplicates are handled:

    * Keys only: this is the default mode. The activity only keeps one element when elements from the different inbound transitions have the same key. This option can only be used if the inbound populations are homogeneous.
    * A selection of columns: select this option to define the list of columns on which the data reconciliation will be applied. You must first select the primary set (that which contains the source data), then the columns to use for the join.

For the **Intersection** and **Exclusion**, you can check the **Generate completement** option if you wish to process the remaining population. The complement will contain the union of the results of all inbound activities minus the intersection. An additional outbound transition will then be added to the activity.

For the **Exclusion**, select the **Primary set** from the inbound transitions, in the **Sets to join** section. This is the set from which elements are excluded. The other sets match elements before being excluded from the primary set.

## Examples

In the following example, we added a **union** that retrieves all the profiles of the two queries: persons between 18 and 27 years old and persons between 34 and 40 years old.

![](../assets/workflow-union-example.png)

The following example shows the **intersection** between two query activities. It is being used here to retrieve profiles who are between 18 to 27 years old and whose email address has been provided.

![](../assets/workflow-intersection-example.png)

The following **exclusion** example shows two queries configured to filter profiles who are between 18 and 27 years old and have an adobe email email domain. The profiles with an adobe email domain are then excluded from the first set. 

![](../assets/workflow-exclusion-example.png)





