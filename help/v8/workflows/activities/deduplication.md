---
audience: end-user
title: Use the Deduplication workflow activity
description: Learn how to use the Deduplication workflow activity
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
---
# Deduplication {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Fields to identify duplicates"
>abstract="In the **Fields to identify duplicates** section, click the **Add attribute** button to specify the fields for which identical values allow duplicates to be identified, such as email address, first name, and last name. The order of the fields specifies those to process first."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Deduplication activity"
>abstract="The **Deduplication** activity deletes duplicates in the results of inbound activities. It is mostly used after targeting activities and before activities that use targeted data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Generate a complement"
>abstract="You can generate an additional outbound transition with the remaining population excluded as duplicates. To do this, toggle on the **Generate complement** option."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Deduplication settings"
>abstract="To delete duplicates in the incoming data, define the deduplication method in the fields below. By default, only one record is kept. Select the deduplication mode based on an expression or an attribute. By default, the record to keep out of the duplicates is randomly selected."

The **Deduplication** activity is a **Targeting** activity. This activity deletes duplicates in the results of inbound activities, such as duplicated profiles in the recipient list. The **Deduplication** activity is generally used after targeting activities and before activities that use targeted data.

## Configure the Deduplication activity {#deduplication-configuration}

Follow these steps to configure the **Deduplication** activity:

![Workflow deduplication configuration process](../assets/workflow-deduplication.png) 

1. Add a **Deduplication** activity to your workflow.

1. In the **Fields to identify duplicates** section, click the **Add attribute** button to specify the fields for which identical values allow duplicates to be identified, such as email address, first name, and last name. The order of the fields specifies those to process first. [Learn how to select attributes and add them to favorites](../../get-started/attributes.md).

1. In the **Deduplication settings** section, select the number of unique **Duplicates to keep**. The default value for this field is 1. The value 0 keeps all the duplicates.

    For example, if records A and B are considered duplicates of record Y, and record C is considered a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept, and two records from A, B, and Y are kept, either by chance or depending on the deduplication method selected.

1. Select the **Deduplication method** to use:

    * **Random selection**: Randomly selects the record to keep out of the duplicates.
    * **Using an expression**: Keeps the records in which the value of the entered expression is the smallest or the largest.
    * **Non-empty values**: Keeps the records for which the expression is not empty.
    * **Following a list of values**: Defines a value priority for one or more fields. To define the values, click **Attribute** to select a field or create an expression, then add the values into the appropriate table. To define a new field, click the **Add** button located above the list of values.

1. Check the **Generate complement** option to exploit the remaining population. The complement consists of all the duplicates. An additional transition is then added to the activity.

## Example {#deduplication-example}

In the following example, use a deduplication activity to exclude duplicates from the target before sending a delivery. The identified duplicated profiles are added to a dedicated audience that can be reused if necessary. Choose the **Email** address to identify the duplicates. Keep 1 entry and select the **Random** deduplication method.

![Example of deduplication activity in a workflow](../assets/workflow-deduplication-example.png)  