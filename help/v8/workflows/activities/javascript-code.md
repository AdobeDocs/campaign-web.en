---
audience: end-user
title: Use the JavaScript code workflow activity
description: Learn how to use the JavaScript code workflow activity
exl-id: ca040ef8-5e0d-44e0-818d-08cfe99100be
---
# JavaScript code {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript code"
>abstract="The **JavaScript code** activity allows you to execute a JavaScript script in the context of a workflow. This enables you to perform actions or collect information from the database. Use **Simple** JavaScript code activities to execute one code snippet during workflow execution. **Advanced** JavaScript code activities allow you to perform more complex operations by executing two different code snippets sequentially. The first time the workflow starts, the first call is executed. Each time the workflow runs again, the code defined in the second call is executed."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript Snippet"
>abstract="Define the script to execute when running the activity. If you are configuring an **Advanced** JavaScript activity, edit two code snippets: the first call code to execute during the first workflow execution, and the next call code to execute during subsequent workflow executions."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript Execution"
>abstract="Configure the execution delay to stop the activity after a period of execution. By default, the execution phase cannot exceed 1 hour. After this delay, the process is aborted with an error message and the activity execution fails. To ignore this limit, set the value to 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="JavaScript Transition"
>abstract="To add one or multiple output transitions, click the **[!UICONTROL Add transitions]** button and specify a label and an internal name for each transition."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_processerrors"
>title="Process errors"
>abstract="Toggle on the **[!UICONTROL Process errors]** option to keep errors that occur during the script execution in an additional output transition."

The **JavaScript code** activity is a **Data management** activity. Use this activity to execute a JavaScript script in the context of a workflow. This enables you to collect information from the database or perform other complex operations.

## Configure the JavaScript code activity {#javascript-code-configuration}

Follow these steps to configure the **JavaScript code** activity:

1. Add a **JavaScript code** activity into your workflow.

1. Choose the type of activity to create:

    * **Simple**: Execute one code snippet.
    * **Advanced**: Perform more advanced operations by executing two different code snippets. [Learn how to configure an advanced JavaScript activity](#advanced)

    >[!NOTE]
    >
    >With the Campaign Web User Interface, two activities have been consolidated into one by merging both **Simple** and **Advanced** JavaScript code functionalities. This consolidation does not impact the activity's functionality.

1. Confirm, then click the **[!UICONTROL Edit code]** button to open the expression editor. The left-hand pane provides predefined syntaxes that you can use to build your code, including event variables. [Learn how to work with event variables and the expression editor](../event-variables.md).

    ![Expression editor interface for JavaScript code activity](../assets/javascript-editor.png)

1. In the **[!UICONTROL Execution]** section, configure the delay to stop the activity after a period of execution. By default, the execution phase cannot exceed 1 hour. After this delay, the process is aborted with an error message and the activity execution fails. To ignore this limit, set the value to 0.

    ![Configuration interface for execution delay](../assets/javascript-config.png)

1. Toggle on the **[!UICONTROL Process errors]** option to keep errors that occur during the script execution in an additional output transition.

## Advanced JavaScript code activities {#advanced}

Advanced JavaScript activities allow you to perform complex operations. These activities enable you to:

* Execute two different code snippets. The first code snippet is executed the first time the workflow starts. Each time the workflow runs again, the code snippet defined in the second call is executed.
* Add multiple output transitions that you can dynamically interact with using a script.

To configure an Advanced JavaScript code activity, follow these steps:

1. Select the **Advanced** type, then configure the code snippets to execute: 

    * Click **[!UICONTROL Edit first call code]** to define the script to execute during the first call.
    * Click **[!UICONTROL Edit next call code]** to define the script to execute during subsequent calls of the workflow. (optional)

1. To add one or multiple output transitions, click the **[!UICONTROL Add transitions]** button and specify a label and an internal name for each transition.

    In this example, two transitions are configured and activated by the script in the code snippet based on specific conditions.

    ![Example of configured transitions](../assets/javascript-transitions.png)

1. Complete the activity configuration and start the workflow.

## Example {#javascript-code-example}

### Initialize variables based on the incoming population {#example1}

This example shows how to initialize a variable based on the number of profiles targeted by a workflow. 

![Example of variable initialization based on profile count](../assets/javascript-example1.png)

In this example, VIP profiles from the database are targeted. A variable named "channel" is created with a value that depends on the number of profiles targeted by the Build audience activity:

* If more than 1000 profiles are targeted, initialize the variable with the value "email".
* Otherwise, initialize it with the value "sms". 

To achieve this, follow these steps:

1. Add a **JavaScript code** activity with the type **Simple** after the **Build audience** activity.

1. Click **Edit code** and configure the code snippet as shown below:

    ```
    if (vars.recCount > 1000)
        vars.channel = "email";
    else
        vars.channel = "sms";
    ```

1. Start the workflow. The "channel" variable is created with the "email" or "sms" value, depending on the number of profiles targeted by the **Build audience** activity.

### Trigger transitions based on a variable's value {#example2}

This example shows how to trigger a transition based on the value of a variable.

![Example of transitions triggered by variable values](../assets/javascript-example2-transitions.png)

In this example, the workflow starts with an **External signal** activity, into which a variable (`interest`) is passed from another workflow. The value of the variable is either "running" or "yoga," depending on the filtering operations performed in the initial workflow.

Different transitions in the workflow are triggered based on the variable's value.

To achieve this, follow these steps:

1. Add a **JavaScript code** activity after the External signal activity with the type **Advanced**.

1. Add two transitions: one for each possible variable value ("running," "yoga").

1. Click **Edit first call code** and configure the code snippet as shown below:

    ```
    if (vars.interest == "running")
        task.postEvent(task.transitionByName("running"));
    else
        task.postEvent(task.transitionByName("yoga"));
    ```

1. Complete the configuration of each transition to suit your needs, then start the workflow. One of the two output transitions is activated based on the value of the `interest` variable passed through the **External signal** activity.