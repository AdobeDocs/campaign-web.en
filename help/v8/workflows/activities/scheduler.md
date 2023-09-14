---
audience: end-user
title: Use the Scheduler workflow activity
description: Learn how to use the Scheduler workflow activity
badge: label="Beta" 
---

# Scheduler {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Scheduler activity"
>abstract="The Scheduler activity allows you..."

The **Scheduler** activity is a **Flow control** activity. It allows you to schedule when the workflow gets started. This activity should be considered as a scheduled start. It can only be used as the first activity of the workflow. 

## Best pratctices

Do not schedule a workflow to run more than every 15 minutes as it may impede overall system performance and create blocks in the database.

## Configuration

Follow these steps to configure the **Scheduler** activity:

1. Add a **Scheduler** activity to your workflow.

   ![](../assets/workflow-scheduler.png)

1. Configure the **Execution frequency**:

   * **Once**: the workflow is executed a single time.

   * **Daily**: the workflow is executed at a specific time, once a day.

   * **Several times a day:** the workflow is regularly executed several times a day. You can set up executions at specific times or periodically.

   * **Weekly**: the workflow is executed at a specified moment, once or several times a week.

   * **Monthly**: the workflow is executed at a specified moment, once or several times a month. You can select months, when you need the workflow to be executed. You can also set up executions on specified week days of the month, such as the second Tuesday of the month.

1. Define the execution details according to the frequency selected. The detail fields may vary depending on the frequency used (time, repetition frequency, specified days, etc.).

1. Click **Preview launch times** to check the schedule of the next ten executions of your workflow.

1. Define the validity period of the scheduler:

   * **Permanent (never expires)**: the workflow is executed, according to the frequency specified, without any limits to the time frame or number of iterations.

   * **Validity period**: the workflow is executed according to the frequency specified, up until a specific date. You need to specify start and end dates. 

## Example

In the following example, the activity is configured so that starts the workflow several times a day at 9 and 12 AM, every day of the week from October 1st, 2023 to January 1st, 2024.

   ![](../assets/workflow-scheduler2.png)



