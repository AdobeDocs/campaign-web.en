---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
---
# Access and manage workflows {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Workflows"
>abstract="In this screen, you can access the full list of standalone and campaign workflows, check their current status, last/next execution dates, and create a new workflow. Browse to the 'Templates' tab to access available workflow templates."

The **[!UICONTROL Workflows]** menu provides access to the full list of workflows. This list includes both **standalone workflows**, created from this screen, and **campaign workflows**, created within a campaign.

![Workflow list screen showing standalone and campaign workflows](assets/workflow-list.png){zoomable="yes"}

Each workflow in the list displays information about its current [status](#status), the last time it was executed or modified, and the next scheduled execution date and time.

Customize the displayed columns by clicking the **[!UICONTROL Configure column for a custom layout]** icon located in the upper-right corner of the list. This allows you to add additional information to the list, such as the last activity in error for each workflow or the applied targeting dimension.

Additionally, a search bar and filters are available to simplify searching within the list. For example, filter workflows to display only those belonging to a campaign or those processed during a specific date range.

To duplicate or delete a workflow, click the ellipsis button, then select **[!UICONTROL Duplicate]** or **[!UICONTROL Delete]**. 

>[!NOTE]
>
>You can duplicate a workflow that is in progress, but you cannot delete it.

## Workflows' statuses {#status}

Workflows can have multiple statuses:

* **[!UICONTROL Draft]**: The workflow has been created and saved.
* **[!UICONTROL In progress]**: The workflow is currently running.
* **[!UICONTROL Finished]**: The workflow execution is complete.
* **[!UICONTROL Paused]**: The workflow has been paused.
* **[!UICONTROL Erroneous]**: The workflow encountered an error. Open the workflow and access the logs and tasks to identify the error and resolve it. [Learn how to monitor logs and tasks](start-monitor-workflows.md#logs-tasks)

Detailed information on how to start and monitor workflow execution is available on [this page](start-monitor-workflows.md).

## Workflow templates {#templates}

The **[!UICONTROL Templates]** tab lists all available workflow templates.

Workflow templates contain pre-configured activities and overall property configurations that can be reused for creating new workflows.

Create workflow templates from an existing workflow or from scratch. [Learn how to create workflow templates](create-workflow.md#workflow-templates)