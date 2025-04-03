---
audience: end-user
title: Use the Test workflow activity
description: Learn how to use the Test workflow activity
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
---
```markdown
# Test {#test}

>[!CONTEXTUALHELP]
>id="acw_orchestration_test"
>title="Test activity"
>abstract="The **Test** activity is a **Flow control** activity. It allows you to enable transitions based on specified conditions."

>[!CONTEXTUALHELP]
>id="acw_orchestration_test_conditions"
>title="Conditions"
>abstract="The **Test** activity can have multiple output transitions. During workflow execution, each condition is tested sequentially until one of them is met. If none of the conditions are met, the workflow continues along the path of the **[!UICONTROL Default condition]**. If no default condition is activated, the workflow stops at this point."

The **Test** activity is a **Flow control** activity. It allows you to enable transitions based on specified conditions.

## Configure the Test activity {#test-configuration}

Follow these steps to configure the **Test** activity:

1. Add a **Test** activity to your workflow.

1. By default, the **[!UICONTROL Test]** activity presents a simple boolean test. If the condition defined in the "True" transition is met, this transition activates. Otherwise, a default "False" transition activates.

1. To configure the condition associated with a transition, click the **[!UICONTROL Open personalization dialog]** icon. Use the expression editor to define the rules required to activate this transition. You can also use event variables, conditions, and date/time functions. [Learn how to work with event variables and the expression editor](../event-variables.md).

    Additionally, modify the **[!UICONTROL Label]** field to personalize the transition's name on the workflow canvas.

    ![Default configuration of the Test activity](../assets/workflow-test-default.png)

1. Add multiple output transitions to a **[!UICONTROL Test]** activity. To do this, click the **[!UICONTROL Add condition]** button and configure the label and associated condition for each transition.

1. During workflow execution, each condition is tested sequentially until one of them is met. If none of the conditions are met, the workflow continues along the path of the **[!UICONTROL Default condition]**. If no default condition is activated, the workflow stops at this point.

## Example {#example}

In this example, different transitions activate based on the number of profiles targeted by a **[!UICONTROL Build audience]** activity:
* If more than 10,000 profiles are targeted, an email message is sent.
* For 1,000 to 10,000 profiles, an SMS is sent.
* If the targeted profiles fall below 1,000, they are directed to a "do not contact" transition.

![Example of Test activity transitions](../assets/workflow-test-example.png)

To achieve this, the `vars.recCount` event variable is used in the "email" and "sms" conditions to count the number of targeted profiles and activate the appropriate transition.

![Configuration of Test activity example](../assets/workflow-test-example-config.png)
```