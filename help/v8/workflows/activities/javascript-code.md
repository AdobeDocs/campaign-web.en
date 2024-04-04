---
audience: end-user
title: Use the JavaScript code workflow activity
description: Learn how to use the JavaScript code workflow activity
---
# JavaScript code {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript code"
>abstract="The **JavaScript code** activity allows you to execute a JavaScript script in the context of a workflow. This allows you to perform actions or collect information from the database. Use **Simple** JavaScript code activities to execute one code snippet at workflow execution. **Advanced** Javascript code activities allows you to perform more complex operation by executing two different code snippets in a sequential order. The first time the workflow is started, the first call is executed. Each time the workflow runs again, the code defined in the second call is executed."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript Snippet"
>abstract="1. Define the script to execute when running the activity. If you are configuring an **Advanced** JavaScript activity, you need to edit two code snippets: the first call code to execute at the first execution of the workflow, and the next call code to execute at the next calls of the workflow."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript Execution"
>abstract="Configure the execution delay to stop the activity after a period of execution. By default, the execution phase cannot exceed 1 hour. After this delay, the process is aborted with an error message and the activity execution fails. To ignore this limit, set the value to 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="JavaScript Transition"
>abstract="If you want to add multiple output transitions, click the **[!UICONTROL Add transitions]** button. This allows you, for example to trigger a specific transition based on a specific condition defined in the JavaScript code activity."

The **JavaScript code** activity is a **Data management** activity. Use this activity to execute a JavaScript script in the context of a workflow. This allows you to perform actions, collect information from the database or perform other operations such as initializing event variables.

## Configure the JavaScript code activity {#javascript-code-configuration}

Follow these steps to configure the **Load file** activity:

![](../assets/javascript-config.png)

1. Drag and drop a **JavaScript code** activity into your workflow.

1. Choose the type of JavaScript activity to configure then confirm:

    * **Simple**: Execute one code snippet.
    * **Advanced**: This option allows you to perform more complex operation by executing two different code snippets in a sequential order. The first code snippet is executed the first time the workflow is started. Each time the workflow runs again, the code snippet defined in the second call is executed.

1. In the **[!UICONTROL JavaScript snippet]** section, click the **[!UICONTROL Edit code]** button to define the script to execute.

    If you are configuring an **Advanced** JavaScript activity, you need to edit two code snippets:
    * **[!UICONTROL Edit first call code]**: define the script to execute during the first call.
    * **[!UICONTROL Edit next call code]**: define the script to execute during the next calls of the workflow.

1. The expression editor opens. Define the code snippet then click **[!UICONTROL Confirm]** once your script is ready. 

    The left hand-side pane provides predefined syntaxes that you can leverage to build your code:

    * The **[!UICONTROL Event variables]** menu allows you to use [events variable](#event-variables) from the workflow into your code.
    * The **[!UICONTROL Conditions]** menu provides functions that allow you to build conditions. [Learn how to create condtions in the expression editor](../../personalization/conditions.md#condition-perso-editor)
    * The **[!UICONTROL Add current date]** menu provides functions related to date formatting.

    ![](../assets/javascript-editor.png)

    >[!CAUTION]
    >
    >**Advanced** JavaScript is a persistent task and is periodically recalled if it has not been marked as completed. If you are configuring an **Advanced** JavaScript activity, make sure you terminate the task and prevent future recalls. To do so, use the **task.setCompleted()** method in your second code snippet (**[!UICONTROL Edit next call code]** button).
    >
    >+++**task.setCompleted()** method sample
    >```
    >task.postEvent(task.transitionByName("ok")); // to transition to Ok branch
    >task.setCompleted();
    >
    >return 0;
    >```
    >+++

1. If you want to add multiple output transitions after the JavaScript code activity, click **[!UICONTROL Add transitions]**. This allows you, for example to trigger a specific transition based on a specific condition defined in the JavaScript code activity.

1. In the **[!UICONTROL Execution]** section, configure the delay to stop the activity after a period of execution. By default, the execution phase cannot exceed 1 hour. After this delay, the process is aborted with an error message and the activity execution fails. To ignore this limit, set the value to 0.

1. Toggle on the **[!UICONTROL Process errors]** option to keep errors that occur during the script execution in an additional output transition.

## Workflows objects & variables {#event-variables}

JavaScripts executed in the context of a workflow access a series of additional global **objects** such the workflow being executed (`ìnstance`), its various tasks (`task`), or the events that activated a task (`event`).

To each type of **object** is associated a category of **variables** that can be leveraged in your JavaScript code.

* **Instance variables** (`instance.vars.xxx`) are comparable to global variables. They are shared by all activities.
* **Task variables** (`task.vars.xxx`) are comparable to local variables. They are only used by the current task. These variables are used by persistent activities to keep data and are sometimes used to exchange data between the different scripts of a same activity.
* **Event variables** (`vars.xxx`) enable the exchange of data between the elementary tasks of a workflow process. These variables are passed by the task that activated the task in progress. They are then passed to the following activities.

Event variables are the most often used variables, and they should be used in preference to instance variables. Predefined event variables are available for use in the expression editor left-hand side pane. You can also create new ones by initializing a new variable in your JavaScript code.

>[!NOTE]
>
>Additional information on JavaScript and the exposed objects and variables in Adobe Campaign is available in the Campaign v8 (client console) documentation in [this section](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Please note that while this resource offers valuable insights, discrepancies may exist as it specifically applies to the client console rather than Campaign Web User Interface.

<!--
## Example {#javascript-code-example}

Trigger transitions
Can trigger transitions based on the execution of the javascript code
Example “name” transition 1
In code, log
Command to trigger transitions
task.postEvent(task.transitionByName)
Example if value of a variable = xxx, trigger transition named “xxxx”
else: trigger another transition


Customers can use it to do more complex operations, and don’t need to use a scheduler because time depend on the execution of the workflow.
scheduler in the javascript activity and can interact with it programmatically.
example:
In first call, initialisze a variable with counter 0
In next call, increment the value.
can planify the next execution of this activity.
Get current date, execute again activity.
Everytime execute the activity, will increment the counter.


Calling an instance variable in a query
> possible ?
https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates#calling-an-instance-variable-in-a-query

Once you have specified an instance variable in an activity, you can re-use it in a workflow query.

Thus, to call a variable **instance.vars.xxx = "yyy"** in a filter, enter **$(instance/vars/xxx)**.

For example:

1. Create an instance variable that defines a delivery's internal name via the **[!UICONTROL JavaScript code]**: **instance.vars.deliveryIN = "DM42"**.

1. Create a query whose targeting and filtering dimensions are the recipients. In the conditions, specify that you would like to find all the recipients that were sent the delivery specified by the variable.

   As a reminder, this information is stored in the delivery logs.

   To reference the instance variable in the **[!UICONTROL Value]** column, enter **$(instance/vars/@deliveryIN)**.

   The workflow will return the recipients of the DM42 delivery.

-->
