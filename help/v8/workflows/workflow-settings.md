---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
badge: label="Alpha" type="Positive"
---
# Configure the workflow settings {#workflow-settings}

content TBD

define settings available from the button in the workflow canvas
<!--à reformuler-->

## Workflow properties {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workflow properties"
>abstract="TBD"

(= same as when creating the workflow ? to check)

* Label
* Additional options
* Internal name
* Folder
* Linked campaign > can change it. If so, workflow will disappear from the current campaign and appear in the new linked one
* Timezone: define a specific time zone to use by default in all the workflow's activities. By default, the workflow's time zone is the one defined for the current Campaign operator.
* Supervisor: When a workflow is in error, the operator(s) belonging to the workflow supervision group are notified by email, as long as their email address is listed in their profile. This group is selected in the **[!UICONTROL Supervisor(s)]** field of the workflow properties.
* description 

## Segmentation settings

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmentation settings"
>abstract="TBD"

* targeting dimension: 

    During data segmentation operations, the targeting key is mapped to a filtering dimension. The targeting dimension lets you define the population targeted by the operation: recipients, contract beneficiaries, operator, subscribers, etc. The filtering dimension lets you select the population based on certain criteria: contract holders, newsletter subscribers, etc.

* keep results: The **Keep the result of interim populations between two executions** option keeps temporary tables between two executions of a workflow.  It is available in the workflow properties' **[!UICONTROL General]** tab, and can be used for development and test purpose to monitor data and check results. You can use this option in development environments, but never use it on production environments. Keeping temporary tables could result in the size of the database increasing significantly and eventually the size limit being reached. Moreover, it will slow down the backup.

    Only the working tables of the last execution of the workflow are kept. Working tables from previous executions are purged by the **[!UICONTROL cleanup]** workflow, which runs on a daily basis.

    >[!CAUTION]
    >
    >This option must **never** be checked in a **production** workflow. This option is used to analyze the results and is designed only for testing purposes and hence must be used only on development or staging environments.

## Workflow execution settings

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Execution settings"
>abstract="TBD"

* History in days: The work tables of the database keep a history of executions (tasks, events, log). Here you can define the number of days to be archived for this workflow: the cleanup process will delete the oldest archives once a day. If the value in this field is zero, the archive will never be deleted. 

    specifies the number of days after which the history must be purged. The history contains elements related to the workflow: logs, tasks, events (technical objects linked to the workflow operation), as well as files downloaded by the **[!UICONTROL Transfer file]** activity. Default value is 30 days for out-of-the-box workflow templates.

    Purge of the history is performed by the Database cleanup technical workflow, which is executed by default everyday

    >[!IMPORTANT]
    >
    >If the **[!UICONTROL History in days]** field is left blank, its value will be considered as "1", meaning that the history will purged after 1 day.

* default affinity: this field allows you to force a workflow or a workflow activity to execute on a particular machine.   If your installation includes several workflow servers, use this field to choose the machine which the workflow will be executed on. If the value defined in this field doesn't exist on any server, the workflow will remain pending.
    
* save sql queriesi in log: allows you to save the SQL queries from the workflow into the logs. (where to access sql logs?)

    This functionality is reserved for advanced users. It concerns workflows that contain targeting activities (query, union, intersection, etc.). When this option is checked, the SQL queries sent to the database during workflow execution are displayed in Adobe Campaign: this means you can analyze them to optimize queries or diagnose issues.

    Queries are displayed in an **[!UICONTROL SQL logs]** tab which is added to the workflow (except campaign workflows) and to the **[!UICONTROL Properties]** activity when the option is enabled. The **[!UICONTROL Audit]** tab also includes SQL queries. 

## Error management settings

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Error management settings"
>abstract="TBD"

* This field lets you define the actions to be taken if a workflow task has errors. There are two possible options:
    
    Stop the process: the workflow is automatically paused. the workflow status changes to Failed. Once the issue is solved, restart the workflow using the Start or Restart buttons.
    
    Ignore: the status of the task that triggered the error changes to Failed, but the workflow keeps the Started status. This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.
    
* Consecutive errors: This field becomes available when the Ignore value is selected in the In case of errors field. You can specify the number of errors that can be ignored before the process is stopped. Once this number is reached, the workflow status changes to Failed. If the value of this field is 0, the workflow will never be stopped regardless of the number of errors.
