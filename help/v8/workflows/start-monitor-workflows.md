---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
exl-id: c9c41189-0150-49a4-bdb3-317fe543eb2c
---
# Start and monitor your workflows {#start-monitor}

Once you create your workflow and design the tasks to perform in the canvas, you can launch it and monitor how it is executed.

## Start the workflow {#start}

To start the workflow, navigate to the **[!UICONTROL Workflows]** menu or the associated campaign, and click the **[!UICONTROL Start]** button in the upper-right corner of the canvas.

Once the workflow is running, each activity in the canvas executes sequentially until the end of the workflow is reached.

You can track the progress of targeted profiles in real time using a visual flow. This allows you to quickly identify the status of each activity and the number of profiles transitioning between them.

![Visual representation of workflow execution in progress.](assets/workflow-execution.png){zoomable="yes"}

## Workflow transitions {#transitions}

In workflows, data transported from one activity to another through transitions is stored in a temporary work table. This data can be displayed for each transition. To display the data, select a transition to open its properties in the right-hand side of the screen.

* Click **[!UICONTROL Preview schema]** to display the schema of the work table.
* Click **[!UICONTROL Preview results]** to view the data transported in the selected transition.

![Example of transition properties and data preview.](assets/transition.png){zoomable="yes"}

## Monitor activity execution {#activities}

Visual indicators in the upper-right corner of each activity box allow you to check their execution status:

| Visual indicator | Description | 
|------------------|-------------|
| ![](assets/activity-status-pending.png){zoomable="yes"}{width="70%"} | The activity is currently being executed. |
| ![](assets/activity-status-orange.png){zoomable="yes"}{width="70%"} | The activity requires your attention. This may involve confirming the sending of a delivery or taking a necessary action. |
| ![](assets/activity-status-red.png){zoomable="yes"}{width="70%"} | The activity has encountered an error. To resolve the issue, open the workflow logs for more information. |
| ![](assets/activity-status-green.png){zoomable="yes"}{width="70%"} | The activity has been successfully executed. |

## Monitor logs and tasks {#logs-tasks}

Monitoring workflow logs and tasks is a key step to analyze your workflows and ensure they are running properly. Logs and tasks are accessible from the **[!UICONTROL Logs]** icon, which is available in the action toolbar and in each activity's properties pane.

The **[!UICONTROL Logs and tasks]** menu provides a history of the workflow execution, recording all user actions and encountered errors. This history is saved for the duration specified in the workflow [execution options](workflow-settings.md). During this duration, all messages are saved, even after a workflow restart. If you do not want to save messages from a previous execution, click the **[!UICONTROL Purge history]** button.

![Example of workflow logs and tasks interface.](assets/workflow-logs.png){zoomable="yes"}

Two types of information are available:

* The **[!UICONTROL Log]** tab contains the execution history of all workflow activities. It indexes the operations carried out and execution errors in chronological order.
* The **[!UICONTROL Tasks]** tab details the execution sequencing of the activities.

In both tabs, you can choose the displayed columns and their order, apply filters, and use the search field to quickly find the desired information.

## Workflow execution commands {#execution-commands}

The action bar in the upper-right corner provides commands to manage the workflow execution. You can:

* **[!UICONTROL Start]** / **[!UICONTROL Resume]** the execution of the workflow. If the workflow was paused, it resumes. Otherwise, it starts, and the initial activities are activated.
* **[!UICONTROL Pause]** the execution of the workflow. The workflow then takes on the Paused status. No new activities are activated until it resumes, but operations in progress are not suspended.
* **[!UICONTROL Stop]** a workflow that is being executed. The workflow then takes on the Finished status. Operations in progress are interrupted if possible. You cannot resume the workflow from the same point where it was stopped.