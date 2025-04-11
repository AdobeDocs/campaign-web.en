---
audience: end-user
title: Use the Combine workflow activity
description: Learn how to use the Combine workflow activity
exl-id: 7e821678-e6a2-4613-b05e-6ccbe4df41c3
---
# Combine {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="Combine activity"
>abstract="The **Combine** activity allows you to perform segmentation on your inbound population. You can combine several populations, exclude part of it, or only keep data common to several targets."

The **Combine** activity is a **Targeting** activity. This activity allows you to perform segmentation on your inbound population. You can combine several populations, exclude part of it, or only keep data common to several targets. Here are the available segmentation types:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* The **Union** regroups the result of multiple activities into a single target.
* The **Intersection** keeps only the elements common to the different inbound populations in the activity.
* The **Exclusion** excludes elements from one population according to certain criteria.

## Configure the Combine activity {#combine-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Intersection merging options"
>abstract="The intersection keeps only the elements common to the different inbound populations in the activity. In the Sets to join section, check all the previous activities you wish to join."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Exclusion merging options"
>abstract="The exclusion excludes elements from one population according to certain criteria. In the Sets to join section, check all the previous activities you wish to join."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="Select the segmentation type"
>abstract="Select how to combine audiences. The **Union** regroups the result of multiple activities into a single target. The **Intersection** keeps only the elements common to the different inbound populations in the activity. The **Exclusion** excludes elements from one population according to certain criteria."

Follow these common steps to configure the **Combine** activity:

![](../assets/workflow-combine.png)

1. Add multiple activities, such as **Build audience** activities, to form at least two different execution branches.
1. Add a **Combine** activity to any of the previous branches.
1. Select the segmentation type: [union](#union), [intersection](#intersection), or [exclusion](#exclusion).
1. Click **Continue**.
1. In the **Sets to join** section, check all the previous activities you wish to join.

## Union {#combine-union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="Reconciliation options"
>abstract="Select the **Reconciliation type** to define how to handle duplicates. By default, the **Keys** option is activated, meaning that the activity keeps only one element when elements from the different inbound transitions have the same key. Use the **A selection of columns** option to define the list of columns on which the data reconciliation is applied."

In the **Combine** activity, configure a **Union** by selecting the **Reconciliation type** to define how duplicates are handled:

* **Keys only**: This is the default mode. The activity keeps only one element when elements from the different inbound transitions have the same key. This option can only be used if the inbound populations are homogeneous.
* **A selection of columns**: Select this option to define the list of columns on which the data reconciliation is applied. First, select the primary set (the source data), then the columns to use for the join.

## Intersection {#combine-intersection}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Intersection reconciliation options"
>abstract="Select the **Reconciliation type** to define how to handle duplicates. By default, the **Keys** option is activated, meaning that the activity keeps only one element when elements from the different inbound transitions have the same key. Use the **A selection of columns** option to define the list of columns on which the data reconciliation is applied."

In the **Combine** activity, configure an **Intersection** by following these extra steps:

1. Select the **Reconciliation type** to define how duplicates are handled. See the [Union](#union) section.
1. Check the **Generate complement** option if you wish to process the remaining population. The complement contains the union of the results of all inbound activities minus the intersection. An additional outbound transition is then added to the activity.

## Exclusion {#combine-exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Exclusion rules"
>abstract="When necessary, manipulate inbound tables. To exclude a target from another dimension, return this target to the same targeting dimension as the main target. Click Add a rule in the Exclusion rules section and specify the dimension change conditions. Data reconciliation is carried out either via an attribute or a join."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="Select sets to combine"
>abstract="In the **Sets to join** section, select the **Primary set** from the inbound transitions. This is the set from which elements are excluded. The other sets match elements before being excluded from the primary set."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_exclusion"
>title="Exclusion rules"
>abstract="When necessary, manipulate inbound tables. To exclude a target from another dimension, return this target to the same targeting dimension as the main target. Click Add a rule in the Exclusion rules section and specify the dimension change conditions. Data reconciliation is carried out either via an attribute or a join."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="Combine generate complement"
>abstract="Toggle on the Generate complement option to process the remaining population in an additional transition."

In the **Combine** activity, configure an **Exclusion** by following these extra steps:

1. In the **Sets to join** section, select the **Primary set** from the inbound transitions. This is the set from which elements are excluded. The other sets match elements before being excluded from the primary set.
1. When necessary, manipulate inbound tables. To exclude a target from another dimension, return this target to the same targeting dimension as the main target. Click **Add a rule** in the **Exclusion rules** section and specify the dimension change conditions. Data reconciliation is carried out either via an attribute or a join.
1. Check the **Generate complement** option if you wish to process the remaining population. See the [Intersection](#intersection) section.

## Examples {#combine-examples}

In the following example, a **Combine** activity uses a **Union** to retrieve all the profiles of the two queries: persons between 18 and 27 years old and persons between 34 and 40 years old.

![](../assets/workflow-union-example.png)

The following example shows the **Intersection** between two query activities. It retrieves profiles who are between 18 and 27 years old and whose email address has been provided.

![](../assets/workflow-intersection-example.png)

The following **Exclusion** example shows two queries configured to filter profiles who are between 18 and 27 years old and have an Adobe email domain. The profiles with an Adobe email domain are excluded from the first set.

![](../assets/workflow-exclusion-example.png)