---
audience: end-user
title: Use the Deduplication workflow activity
description: Learn how to use the Deduplication workflow activity
badge: label="Beta" 
---

# Deduplication {#deduplication}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Fork activity"
>abstract="The Deduplication activity allows you to..."
-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Deduplication complement"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Deduplication settings"
>abstract="TBD"

The **Deduplication** activity is a **Targeting** activity. This activity allows you to delete duplicates in the result(s) of the inbound activities. The **Deduplication** activity is generally used following targeting activities and before activities that allow the use of targeted data.

## Configuration

Follow these steps to configure the **Scheduler** activity:

1. Add a **Deduplication** activity to your workflow.

      ![](../assets/workflow-deduplication.png)

1. In the **Fields to identify duplicates** section, click the **Add attribute** button to specify the fields for which the identical values allow the duplicates to be identified: email address, first name, last name, etc. The order of the fields allows you to specify those to process first.

1. Select the number of unique **Duplicates to keep**. The default value for this field is 1. The value 0 allows you to keep all the duplicates.

<!--
    For example, if records A and B are considered duplicates of record Y, and a record C is considered as a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept and two records from A, B, and Y are kept, by chance or depending on the deduplication method selected thereafter.

-->

1. Select the **Deduplication method** to use:

    * **Random selection**: randomly selects the record to be kept out of the duplicates.
    * **Using an expression**: this lets you keep the records in which the value of the expression entered is the smallest or the biggest. ++ Expression ++ Sort
    * **Following a list of values**: lets you define a value priority for one or more fields. To define the values, click **Attribute** to select a field or create an expression, then add the value(s) into the appropriate table. To define a new field, click the Add button located above the list of values. ++ Sort

1. Check the **Generate complement** option if you wish to exploit the remaining population. The complement consists of all the duplicates. An additional transition will then be added to the activity.

## Example
