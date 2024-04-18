---
audience: end-user
title: Configure workflow settings
description: Learn how to configure workflow settings with Adobe Campaign Web
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
---

# Configure workflow settings {#workflow-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Workflow properties"
>abstract="In this screen, choose the template to use to create the workflow and specify a label. Expand the **Additional options** section to configure more settings such as the workflow internal name, its folder, timezone, and supervisor group. It is highly recommended to select a supervisor group so that operators are alerted if an error occurs."

When creating a workflow or orchestrating workflow activities in the canvas, you can access advanced settings related to the workflow. For example, you can set a specific timezone for the workflow, manage how the workflow should behave in case of error, or manage the delay after which the workflow history should be purged.

These settings are pre-configured in the template selected when creating the workflow, but can be edited as needed for this specific workflow.

![](assets/workflow-settings-button.png){zoomable="yes"}{width="70%" align="left"}

## Workflow properties {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workflow properties"
>abstract="This section provides generic workflow properties that are also accessible when creating the workflow. You can choose the template to use to create the workflow and specify a label. Expand the Additional options section to configure specific settings such as the workflow storing folder or timezone."

The **[!UICONTROL Properties]** section provides generic settings which can be configured when creating a workflow. To access the properties of an existing workflow, click the **[!UICONTROL Settings]** button available in the actions bar above the workflow canvas.


![](assets/workflow-settings.png){zoomable="yes"}{width="70%" align="left"}


These properties are:

* The **[!UICONTROL Label]** of the workflow that displays in the list.
* The **[!UICONTROL Internal name]** of the workflow.
* The **[!UICONTROL Folder]** where the workflow should be saved.
* The default **[!UICONTROL Timezone]** to use in all the workflow's activities. By default, the workflow's time zone is the one defined for the current Campaign operator.
    Possible values are:
    * **Server time zone** to use the time zone of the Adobe Campaign application server
    * **Operator time zone** to uses the time zone of the Adobe Campaign operator who executes the workflow, as defined in the operator's profile, in the client console
    * **Time zone of the database** to use the time zone of the database server
    * A specific time zone
* When a workflow fails, the operators belonging to the operators group selected in the **[!UICONTROL Supervisor(s)]** field are notified by email.
* You can also enter a **[!UICONTROL Description]** of your workflow.

When the workflow is [associated to a campaign](create-workflow.md), it is displayed in the **[!UICONTROL Linked campaign]** field. You can open the associated campaign from that field.


## Segmentation settings  {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmentation settings"
>abstract="In this section, you can select the targeting dimension to target profiles in the workflow, and choose to keep the worklow results between two executions. This option should be used for testing purposes only and must never be enabled in a production workflow."

* **[!UICONTROL Targeting dimension]**: Select the targeting dimension to use to target profiles: recipients, contract beneficiaries, operator, subscribers, etc. [Learn more about targeting dimensions](../audience/targeting-dimensions.md)

* **[!UICONTROL Keep the result of interim populations between two executions]**: By default, only the working tables of the last execution of the workflow are kept. Working tables from previous executions are purged by a technical workflow, which runs on a daily basis.

    If this option is enabled, working tables will be kept even after the workflow has been executed. You can use it for testing purposes and hence must be used **only** on development or staging environments. It must never be checked in a production workflow.

## Execution settings  {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Execution settings"
>abstract="In this section, you can configure settings related to the execution of the worklow, such the number of days the workflow history is kept."

* **[!UICONTROL History in days]**: Specifies the number of days after which the history must be purged. The history contains elements related to the workflow: logs, tasks, events (technical objects linked to the workflow operation). Default value is 30 days for out-of-the-box workflow templates. Purge of the history is performed by the Database cleanup technical workflow, which is executed by default everyday

    >[!IMPORTANT]
    >
    >If the **[!UICONTROL History in days]** field is left blank, its value will be considered as "1", meaning that the history will purged after 1 day.

* **[!UICONTROL Default affinity]**: If your installation includes several workflow servers, use this field to specify the server which the workflow will be executed on. This forces the execution of that workflow on a particular server. You can choose any existing affinity name, but make sure you do not use spaces or punctuation marks. If you use different servers, specify different names, separated by commas.

    >[!IMPORTANT]
    >
    >If the value defined in this field does not exist on any server, the workflow will remain pending.

    
* **[!UICONTROL Save SQL queries in log]**: Check this option to you to save the SQL queries from the workflow into the logs. This functionality is reserved for advanced users. It applies to workflows that contain targeting activities like **[!UICONTROL Build audience]**. When this option is enabled, the SQL queries sent to the database during workflow execution are displayed in the workflow's logs, allowing you to analyze them to optimize queries or diagnose issues.

## Error management settings  {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Error management settings"
>abstract="In this section, you can define how the workflow should manage errors during its execution. You can choose to pause the process, ignore a certain number of errors, or stop the workflow execution."

* **[!UICONTROL Error management]**: This field lets you define the actions to be taken if a workflow task has errors. There are three possible options:
    
    * **[!UICONTROL Suspend the process]**: The workflow is automatically paused and its status changes to **[!UICONTROL Failed]**. Once the issue is solved, resume the workflow using the **[!UICONTROL Resume]** buttons.
    * **[!UICONTROL Ignore]**: The status of the task that triggered the error changes to **[!UICONTROL Failed]**, but the workflow keeps the **[!UICONTROL Started]** status. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
    * **[!UICONTROL Abord the process]**: The workflow is automically stopped and its status changes to **[!UICONTROL Failed]**. Once the issue is solved, restart the workflow using the **[!UICONTROL Start]** buttons.

* **[!UICONTROL Consecutive errors]**: This field becomes available when the **[!UICONTROL Ignore]** value is selected in the **[!UICONTROL In case of errors]** field. You can specify the number of errors that can be ignored before the process is stopped. Once this number is reached, the workflow status changes to **[!UICONTROL Failed]**. If the value of this field is 0, the workflow will never be stopped regardless of the number of errors.

## Initialization script {#initialization-script}

The **Initialization script** lets you initialize variables or modify activity properties. Click the **Edit code** button and type the snippet of code to execute. The script is called when the workflow executes. Refer to the section related to [event variables](../workflows/event-variables.md).

