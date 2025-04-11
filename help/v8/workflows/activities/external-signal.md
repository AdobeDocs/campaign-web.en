---
audience: end-user
title: Use the External signal activity
description: Learn how to use the External signal workflow activity
exl-id: e4244ecc-5e37-41a6-a4dd-6e32da6d5512
---
# External signal {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="External Signal"
>abstract="The **External signal** activity lets you trigger the execution of a workflow from another workflow or an API call."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="External Signal Parameters"
>abstract="External Signal Parameters"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="End triggers"
>abstract="End triggers"

The **External signal** activity is a **Flow control** activity. It lets you trigger the execution of a workflow from another workflow or an API call.

>[!NOTE]
>
>This page explains the main steps to configure an **[!UICONTROL External Signal]** activity in Campaign Web User Interface and trigger it from another workflow or an API call. Detailed information on how to trigger a workflow, best practices, and how to work with Campaign APIs is available in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example).

Follow these steps to configure the **External signal** activity and trigger its execution:

1. Add an **External signal** activity into your workflow.

1. Complete the configuration of your workflow, and start its execution. The **[!UICONTROL External Signal]** activity displays as "Pending," waiting to be triggered.
 
    ![The screenshot shows the External Signal activity in a pending state.](../assets/external-signal-pending.png)

1. Retrieve the following information:

    * The **workflow's internal name**, which displays next to its label.

        +++View example

        ![The screenshot shows the workflow's internal name next to its label.](../assets/external-signal-workflow-name.png)

        +++

    * The **External signal activity's name**, which displays in the workflow's **[!UICONTROL Execution options]**.

        +++View example
  
        ![The screenshot shows the External Signal activity's name in the Execution options.](../assets/external-signal-name.png)

        +++

1. To trigger the workflow, execute the `PostEvent` JavaScript function. This function lets you pass variables with the values of your choice and use them in the triggered workflow.

    The `PostEvent` function can be executed either from another workflow or from an API call.

    * To trigger an **[!UICONTROL External signal]** activity from a workflow, execute the PostEvent function from the **[!UICONTROL Initialization script]** pane, accessible from the activity's **[!UICONTROL Execution options]**. For the **[!UICONTROL JavaScript code]** activity, execute the function from the activity's script.

        The syntax is as follows:

        ```

        xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);

        ```

    +++View example

    In this example, the "signal1" External signal activity is triggered. It has been added to the workflow whose internal name is "WKF12345." A variable named "customID" is passed with the value "123456."
 
    ![The screenshot shows an example of triggering the External Signal activity using the PostEvent function.](../assets/external-signal-sample.png)

    +++

    * To trigger an **[!UICONTROL External signal]** activity from an API call, follow the steps detailed in the Campaign API documentation. [Learn how to use the static `PostEvent` method](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html).