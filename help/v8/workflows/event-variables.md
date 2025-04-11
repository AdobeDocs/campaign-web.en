---
audience: end-user
title: Workflow event variables
description: Learn how to leverage event variables in your workflows.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
---
# Workflow event variables {#event-variables}

Some workflow activities allow you to edit scripts in the expression editor to perform specific actions, such as retrieving data from previous activities, building conditions, or computing file names based on event variables.

## What are event variables {#scripting}

Scripts executed in the context of a workflow access a series of additional global **objects**, such as the workflow itself that is being executed (`instance`), its various tasks (`task`), or the events that activated a given task (`event`).

Each type of **object** is associated with a category of **variables** that can be used in the expression editor when editing scripts in activities, such as **[!UICONTROL JavaScript code]** or **[!UICONTROL Test]**.

* **Instance variables** (`instance.vars.xxx`) are comparable to global variables. They are shared by all activities.
* **Task variables** (`task.vars.xxx`) are comparable to local variables. They are only used by the current task. These variables are used by persistent activities to keep data and are sometimes used to exchange data between the different scripts of the same activity.
* **Event variables** (`vars.xxx`) enable the exchange of data between the elementary tasks of a workflow process. These variables are passed by the task that activated the task in progress. They are then passed to the following activities. **Event variables** are the most commonly used variables, and they should be used in preference to instance variables.

>[!NOTE]
>
>Additional information on scripting and the exposed objects and variables in Adobe Campaign is available in the Campaign v8 (client console) documentation in [this section](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Please note that while this resource offers valuable insights, discrepancies may exist as it specifically applies to the client console rather than Campaign Web User Interface.

## Leverage event variables in the expression editor {#expression-editor}

Predefined event variables are available for use in the expression editor's left-hand side pane. You can also create new ones by initializing a new variable in your code.

![Screenshot showing predefined event variables in the expression editor's left-hand side pane](assets/event-variables.png)

In addition to these event variables, you can also use the **[!UICONTROL Conditions]** menu in the left pane to build conditions and the **[!UICONTROL Add current date]** menu to apply functions related to date formatting.