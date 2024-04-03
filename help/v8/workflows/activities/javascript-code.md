---
audience: end-user
title: Use the JavaScript code workflow activity
description: Learn how to use the JavaScript code workflow activity
---
# JavaScript code {#javascript-code}

<!--Javascript-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript code"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript Snippet"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript Execution"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="JavaScript Transition"
>abstract="TBC"

The **JavaScript code** activity is a **Data management** activity. Use this activity to execute a JavaScript script in the context of a workflow. This allows you to perform actions, collect information from the database or perform other operation such as initializing event variables in addition to the predefined event variables already available in the expression editor.

Often combined with a Test activity to test the 

## Configure the JavaScript code activity {#javascript-code-configuration}

Follow these steps to configure the **Load file** activity:

1. Drag and drop a **JavaScript code** activity into your workflow.

1. Choose the type of JavaScript activity to configure

    * **Simple**: Execute one code snippet.
    * **Advanced**: This option allows you to perform more complex operation by executing two different code snippets in a sequential order. The first time the workflow is started, the first call is executed. Each time the workflow runs again, the code defined in the second call is executed.

1. Click **[!UICONTROL Continue]** to confirm your selection then click the **[!UICONTROL Edit code]** button to define the script to execute.

    If you are configuring an **Advanced** JavaScript activity, you need to edit two code snippets:
    * **[!UICONTROL Edit first call code]**: define the script to execute during the first call.
    * **[!UICONTROL Edit next call code]**: define the script to execute during the next calls of the workflow.

    >[!CAUTION]
    >
    >Advanced JavaScript is a persistent task and is periodically recalled if it has not been marked as completed. To terminate the task and prevent future recalls, you must use the **task.setCompleted()** method in the **[!UICONTROL Next calls]** section:
    >
    >+++**task.setCompleted()** method sample
    >```
    >task.postEvent(task.transitionByName("ok")); // to transition to Ok branch
    >task.setCompleted();
    >
    >return 0;
    >```
    >+++

1. If you want to add multiple output transitions, click the **[!UICONTROL Add transitions]** button. This allows you, for example to trigger a specific transition based on a specific condition defined in the JavaScript code activity.

1. Configure the execution delay to stop the activity after a period of execution. By default, the execution phase cannot exceed 1 hour. After this delay, the process is aborted with an error message and the activity execution fails. To ignore this limit, set the value to 0.

1. Toggle on the **[!UICONTROL Process errors]** option to keep errors that occur during the script execution in an additional output transition.

## Example {#javascript-code-example}

Example logInfo to display information into the logs
When starting the workflow, if check the logs, will see the message defined in the code


Can trigger transitions based on the execution of the javascript code
Example “name” transition 1
In code, log
Command to trigger transitions
task.postEvent(task.transitionByName)
Example if value of a variable = xxx, trigger transition named “xxxx”
else: trigger another transition


Customers can use it to do more ocmplex operations, and don’t need to use a scehduler because time depend on the execution of the workflow.
scheduler in the javascript activity and can interact with it programmatically.
example:
In first call, initialisze a variable with counter 0
In next call, increment the value.
can planify the next execution of this activity.
Get current date, execute again activity.
Everytime execute the activity, will increment the counter.