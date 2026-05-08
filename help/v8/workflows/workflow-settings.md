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
>abstract="In this screen, choose the template to use to create the workflow and specify a label. Expand the **Additional options** section to configure more settings, such as the workflow internal name, its folder, timezone, and supervisor group. It is highly recommended to select a supervisor group so that operators are alerted if an error occurs."

When creating a workflow or orchestrating workflow activities in the canvas, access advanced settings related to the workflow. For example, set a specific timezone for the workflow, manage how the workflow should behave in case of error, or manage the delay after which the workflow history is purged.

These settings are pre-configured in the template selected when creating the workflow, but can be edited as needed for this specific workflow.

![Workflow settings button interface](assets/workflow-settings-button.png){zoomable="yes"}{width="70%" align="left"}

## Workflow properties {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workflow properties"
>abstract="This section provides generic workflow properties that are also accessible when creating the workflow. You can choose the template to use to create the workflow and specify a label. Expand the Additional options section to configure specific settings, such as the workflow storing folder or timezone."

The **[!UICONTROL Properties]** section provides generic settings that can be configured when creating a workflow. To access the properties of an existing workflow, click the **[!UICONTROL Settings]** button available in the actions bar above the workflow canvas.

![Workflow settings interface](assets/workflow-settings.png){zoomable="yes"}{width="70%" align="left"}

These properties include:

* The **[!UICONTROL Label]** of the workflow that displays in the list.
* The **[!UICONTROL Internal name]** of the workflow.
* The **[!UICONTROL Folder]** where the workflow should be saved.
* The default **[!UICONTROL Timezone]** to use in all the workflow's activities. By default, the workflow's timezone is the one defined for the current Campaign operator.
    Possible values are:
    * **Server timezone** to use the timezone of the Adobe Campaign application server.
    * **Operator timezone** to use the timezone of the Adobe Campaign operator who executes the workflow, as defined in the operator's profile in the client console.
    * **Timezone of the database** to use the timezone of the database server.
    * A specific timezone.
* When a workflow fails, the operators belonging to the operator group selected in the **[!UICONTROL Supervisor(s)]** field are notified by email.
* Enter a **[!UICONTROL Description]** of your workflow.

When the workflow is [associated with a campaign](create-workflow.md), it is displayed in the **[!UICONTROL Linked campaign]** field. Open the associated campaign from that field.

## Segmentation settings {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmentation settings"
>abstract="In this section, you can select the targeting dimension to target profiles in the workflow and choose to keep the workflow results between two executions. This option should be used for testing purposes only and must never be enabled in a production workflow."

* **[!UICONTROL Targeting dimension]**: Select the targeting dimension to use to target profiles, such as recipients, contract beneficiaries, operators, subscribers, and others. [Learn more about targeting dimensions](../audience/targeting-dimensions.md).

* **[!UICONTROL Keep the result of interim populations between two executions]**: By default, only the working tables of the last execution of the workflow are kept. Working tables from previous executions are purged by a technical workflow, which runs daily.

    If this option is enabled, working tables will be kept even after the workflow has been executed. Use it for testing purposes, and ensure it is used **only** on development or staging environments. It must never be checked in a production workflow.

## Execution settings {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Execution settings"
>abstract="In this section, you can configure settings related to the execution of the workflow, such as the number of days the workflow history is kept."

* **[!UICONTROL History in days]**: Specifies the number of days after which the history must be purged. The history contains elements related to the workflow, such as logs, tasks, and events (technical objects linked to the workflow operation). The default value is 30 days for out-of-the-box workflow templates. Purge of the history is performed by the Database cleanup technical workflow, which is executed daily.

    >[!IMPORTANT]
    >
    >If the **[!UICONTROL History in days]** field is left blank, its value will be considered as "1," meaning that the history will be purged after 1 day.

* **[!UICONTROL Default affinity]**: If your installation includes several workflow servers, use this field to specify the server on which the workflow will be executed. This forces the execution of that workflow on a particular server. Choose any existing affinity name, but ensure you do not use spaces or punctuation marks. If you use different servers, specify different names separated by commas.

    >[!IMPORTANT]
    >
    >If the value defined in this field does not exist on any server, the workflow will remain pending.

* **[!UICONTROL Save SQL queries in log]**: Check this option to save the SQL queries from the workflow into the logs. This functionality is reserved for advanced users. It applies to workflows that contain targeting activities, such as **[!UICONTROL Build audience]**. When this option is enabled, the SQL queries sent to the database during workflow execution are displayed in the workflow's logs, allowing you to analyze them to optimize queries or diagnose issues.

## Error management settings {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Error management settings"
>abstract="In this section, you can define how the workflow should manage errors during its execution. You can choose to pause the process, ignore a certain number of errors, or stop the workflow execution."

* **[!UICONTROL Error management]**: This field lets you define the actions to be taken if a workflow task has errors. There are three possible options:
    
    * **[!UICONTROL Suspend the process]**: The workflow is automatically paused, and its status changes to **[!UICONTROL Failed]**. Once the issue is solved, resume the workflow using the **[!UICONTROL Resume]** buttons.
    * **[!UICONTROL Ignore]**: The status of the task that triggered the error changes to **[!UICONTROL Failed]**, but the workflow keeps the **[!UICONTROL Started]** status. <!-- TO ADD ONCE SCHEDULER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
    * **[!UICONTROL Abort the process]**: The workflow is automatically stopped, and its status changes to **[!UICONTROL Failed]**. Once the issue is solved, restart the workflow using the **[!UICONTROL Start]** buttons.

* **[!UICONTROL Consecutive errors]**: This field becomes available when the **[!UICONTROL Ignore]** value is selected in the **[!UICONTROL In case of errors]** field. Specify the number of errors that can be ignored before the process is stopped. Once this number is reached, the workflow status changes to **[!UICONTROL Failed]**. If the value of this field is 0, the workflow will never be stopped regardless of the number of errors.

## Initialization script {#initialization-script}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_initialization"
>title="Initialization script"
>abstract="This section lets you define JavaScript code that runs at the start of the workflow. It can be used to initialize variables, set parameters, or prepare data before any workflow activities are executed."

The **Initialization script** lets you initialize variables or modify activity properties. Click the **Edit code** button and type the snippet of code to execute. The script is called when the workflow executes. Refer to the section related to [event variables](../workflows/event-variables.md).