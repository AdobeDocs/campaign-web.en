---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 51648665-8400-426c-85cf-dbf5f4f81d20
---
# Access & monitor your workflows {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Workflows"
>abstract="In this screen, you can access the full list of standalone and campaign workflows, check their current status, last/next execution dates, and create a new workflow. Browse to the 'Template' tab to access available workflow templates."

## Access & manage workflows {#access}

The **[!UICONTROL Workflows]** menu allows you to access the full list of workflows. This list includes both **standalone workflows** that have been created from this screen, and **campaign workflows**, which have been created within a campaign.

![](assets/workflow-list.png)

Each workflow in the list displays information about its current [status](#status), the last time it was executed or modified, and the next scheduled execution date and time.

You can custmize the displayed columns by clicking the **[!UICONTROL Configure column for a custom layout]** icon located in the upper-right corner of the list. This allows you to add additional information to the list, such as the last activity in error for each workflow, or the applied targeting dimension.

In addition, a search bar and filters are available to facilitate easy searching within the list. For example, you can filter the workflows to display only those belonging to a campaign, or those processed during a specific date range.

To duplicate or delete a workflow, click the ellipsis button then select **[!UICONTROL Duplicate]** or **[!UICONTROL Delete]**. 

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

Detailed information on how to start and monitor workflow execution is available in [this page](start-monitor-workflows.md).

## Workflow templates {#templates}

The **[!UICONTROL Templates]** tab lists all available workflows templates.

Workflow templates contain pre-configured activities and overall property configurations that can be reused for creating new workflows. They are created from the client console. [Learn how to work with templates](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)
