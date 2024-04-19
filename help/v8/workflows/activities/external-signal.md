---
audience: end-user
title: Use the External signal activity
description: Learn how to use the External signal workflow activity
---
# External signal {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="External Signal"
>abstract="The **External signal** activity lets you trigger the execution of a workflow deom another workflow or an API call."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="External Signal Parameters"
>abstract="External Signal Parameters"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="End triggers"
>abstract="End triggers"

The **External signal** activity is a **Flow control** activity. It allows you to trigger the execution of a workflow from another workflow or from an API call.

>[!NOTE]
>
>This page presents the main steps to configure an **[!UICONTROL External Signal]** activity in Campaign Web User Interface and trigger it from another workflow or an API call. Detailed information on how to trigger a workflow and its best practices, and how to work with Campaign APIs is available in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

Follow these steps to configure the **External signal** activity and trigger its execution:

1. Add an **External signal** activity into your workflow.

1. Complete the configuration of your workflow and start its execution. The **[!UICONTROL External Signal]** activity displays as "Pending", waiting to be triggered.

    ![](../assets/external-signal-pending.png)

1. Retrieve the information below:

    * The **workflow's internal name**, which displays next to its label.

        +++View example

        ![](../assets/external-signal-workflow-name.png)

        +++

    * The **External signal activity's name**, which displays in the workflow's **[!UICONTROL Execution options]**.

        +++View example

        ![](../assets/external-signal-name.png)

        +++

1. To trigger the workflow, you need to execute the `PostEvent` JavaScript function. This function allows you to pass variables with the values of your choice and leverage them in the triggered workflow.

    The `PostEvent` function can be executed either from another workflow, or from an API call.

    * To trigger an **[!UICONTROL External signal]** activity from a workflow, execute the PostEvent function from the **[!UICONTROL Initialization script]** pane, which is accessible from the activity's **[!UICONTROL Execution options]**. For the **[!UICONTROL JavaScript code]** activity, execute the function from the activity's script.

        The syntax is as follows:

        ```

        xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);

        ```

    +++View example

    In this example, we are triggering the "signal1" External signal activity that has been added to the workflow whose internal name is "WKF12345". We are also passing a variable named "customID", with the value "123456".

    ![](../assets/external-signal-sample.png)

    +++

    * To trigger an **[!UICONTROL External signal]** activity from an API call, follow the steps detailed in the Campaign API documentation. [Learn how to use the static `PostEvent` method](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html)
