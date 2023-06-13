---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
badge: label="Alpha" 
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
---
# Configure workflow settings {#workflow-settings}

When orchestrating workflow activities in the canvas, you can access advanced settings related to the workflow. For example, you can set a specific timezone for the workflow, manage how the workflow should behave in case of error, or manage the delay after which the workflow history should be purged.

These settings are pre-configured in the template selected when creating the workflow, but can be edited as needed for this specific workflow.

To do this, click the **[!UICONTROL Workflow settings]** icon  in the upper-left corner of the canvas, next to the workflow label.

![](assets/workflow-settings.png)

## Workflow properties {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workflow properties"
>abstract="This section provides generic workflow properties that are also accessible when creating the workflow. You can choose the template to use to create the workflow and specify a label. Expand the Additional options section to configure specific settings such as the workflow storing folder or timezone."

The **[!UICONTROL Properties]** section provides generic settings that are also accessible when creating the workflow.

* **[!UICONTROL Label]**: The label of the workflow that displays in the list.
* **[!UICONTROL Name]**: The internal name of the workflow.
* **[!UICONTROL Folder]**: The folder where the workflow should be saved.
* **[!UICONTROL Linked campaign]**: This field display if the workflow has been created within a campaign. It allows you to open the associated campaign.
* **[!UICONTROL Timezone]**: Define a specific time zone to use by default in all the workflow's activities. By default, the workflow's time zone is the one defined for the current Campaign operator.
* **[!UICONTROL Supervisor(s)]**: When a workflow is in error, the operator(s) belonging to the workflow supervision group are notified by email, as long as their email address is listed in their profile.
* **[!UICONTROL Description]**: Use this field to provide a description of your workflow.

## Segmentation settings

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmentation settings"
>abstract="In this section, you can select the targeting dimension to target profiles in the workflow, and choose to keep the worklow results between two executions. This option should be used for testing purposes only and must never be enabled in a production workflow."

* **[!UICONTROL Targeting dimension]**: Select the targeting dimension to use to target profiles: recipients, contract beneficiaries, operator, subscribers, etc.
* **[!UICONTROL Keep the result of interim populations between two executions]**: By default, only the working tables of the last execution of the workflow are kept. Working tables from previous executions are purged by a technical workflow, which runs on a daily basis.

    If this option is enabled, working tables will be kept even after the workflow has been executed. You can use it for testing purposes and hence must be used only on development or staging environments. It must never be checked in a production workflow.

## Execution settings

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Execution settings"
>abstract="In this section, you can configure settings related to the execution of the worklow, such the number of days the workflow history is kept."

* **[!UICONTROL History in days]**: Specifies the number of days after which the history must be purged. The history contains elements related to the workflow: logs, tasks, events (technical objects linked to the workflow operation). Default value is 30 days for out-of-the-box workflow templates. Purge of the history is performed by the Database cleanup technical workflow, which is executed by default everyday

    >[!IMPORTANT]
    >
    >If the **[!UICONTROL History in days]** field is left blank, its value will be considered as "1", meaning that the history will purged after 1 day.

* **[!UICONTROL Default affinity]**: If your installation includes several workflow servers, use this field to choose the machine which the workflow will be executed on. If the value defined in this field does not exist on any server, the workflow will remain pending.
    
* **[!UICONTROL Save SQL queries in log]**: allows you to save the SQL queries from the workflow into the logs. This functionality is reserved for advanced users. It applies to workflows that contain targeting activities like **[!UICONTROL Build audience]**. When this option is enabled, the SQL queries sent to the database during workflow execution are displayed in the workflow's logs, allowing you to analyze them to optimize queries or diagnose issues.

## Error management settings

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Error management settings"
>abstract="In this section, you can manage how the workflow should behave when an error occurs during its execution (pause/stop its execution or ignore errors)."

* **[!UICONTROL Error management]**: This field lets you define the actions to be taken if a workflow task has errors. There are two possible options:
    
    * **[!UICONTROL Suspend the process]**: The workflow is automatically paused and its status changes to **[!UICONTROL Failed]**. Once the issue is solved, resume the workflow using the **[!UICONTROL Resume]** buttons.
    * **[!UICONTROL Ignore]**: The status of the task that triggered the error changes to **[!UICONTROL Failed]**, but the workflow keeps the **[!UICONTROL Started]** status. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
    * **[!UICONTROL Abord the process]**: The workflow is automically stopped and its status changes to **[!UICONTROL Failed]**. Once the issue is solved, restart the workflow using the **[!UICONTROL Start]** buttons.

* **[!UICONTROL Consecutive errors]**: This field becomes available when the **[!UICONTROL Ignore]** value is selected in the **[!UICONTROL In case of errors]** field. You can specify the number of errors that can be ignored before the process is stopped. Once this number is reached, the workflow status changes to **[!UICONTROL Failed]**. If the value of this field is 0, the workflow will never be stopped regardless of the number of errors.
