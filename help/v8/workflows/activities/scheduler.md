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

The Scheduler activity allows you to schedule when a workflow or an activity is started.

The Scheduler activity should be considered as a scheduled start. This activity can only be used as the first activity of the workflow. 

## Best pratctices

* Do not schedule a workflow to run more than every 15 minutes as it may impede overall system performance and create blocks in the database.

## Configuration

Follow these steps to configure the **Scheduler** activity:

1. Add a **Scheduler** activity to your workflow.

1. Configure the **Execution frequency**:

   * Once: the workflow is executed a single time.

   * Daily: the workflow is executed at a specific time, once a day.

   * Several times a day: the workflow is regularly executed several times a day. You can set up executions at specific times or periodically.

   * Weekly: the workflow is executed at a specified moment, once or several times a week.

   * Monthly: the workflow is executed at a specified moment, once or several times a month. You can select months, when you need the workflow to be executed. You can also set up executions on specified weekday of the month, such as the second Tuesday of the month.
1. Define the execution details according to the frequency selected. The detail fields may vary depending on the frequency used (time, repetition frequency, specified days, etc.).

1. Click **Preview launch times** to check the schedule of the next ten executions of your workflow.

1. Define the validity period of the scheduler:

   * Permanent (never expires): the workflow will be executed, according to the frequency specified, without any limits to the time frame or number of iterations.
   
   * Validity period: the workflow will be executed according to the frequency specified, up until a specific date. The execution deadline will therefore need to be specified.

## Example


