---
audience: end-user
title: Automated delivery workflow activity
description: Learn how to use the Automated delivery workflow activity
exl-id: a9c485f1-0369-414d-9e43-bedb0390a2f5
---
# Automated delivery {#automated-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Automated delivery activity"
>abstract="The Automated delivery workflow activity is now available in the workflow palette. You can use it to create or execute delivery actions (prepare, send a proof, prepare and start, etc.) directly within your workflow."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"

>[!CONTEXTUALHELP]
>id="acw_orchestration_automated-delivery"
>title="Automated delivery activity"
>abstract="The **Automated delivery** activity is used for automation: create or reuse a delivery in your workflow, then choose the action to perform (prepare, prepare and start, send proof, etc.). You can select an existing explicit delivery created outside the workflow, or create a new delivery from a template each time the activity runs."

The **Automated delivery** activity lets you create, configure, and execute delivery actions directly within your workflow. Use it when you want to run a predefined delivery on a schedule or as part of an automated flow, or when you want to generate a new delivery from a template each time the activity runs.

<!--
**[Continuous delivery](continuous-delivery.md)** always uses a template. The first run creates one delivery; later runs send to new recipients through that same delivery. **Automated delivery** is different: you either reuse one existing delivery every run, or you create a new delivery from a template each time—so each run can be its own delivery if you want. 
-->

To configure this activity, follow these steps:

1. Define the delivery settings, [read more](#delivery-settings)
1. Select the action to perform, [read more](#action-to-execute)
1. Set up the transition, [read more](#transition-to-execute)
1. Define a modification script, [read more](#script)

## Define the delivery settings {#delivery-settings}

When you configure the activity, you choose where the delivery comes from. Two options are available in this section:

![Screenshot showing the automated delivery](../assets/automated-delivery.png){zoomable="yes"}

* Select **Explicit delivery** when you want to act on an existing delivery, for example a stand-alone delivery or a delivery created from a campaign. Pick the delivery using the **Select delivery** button. Each time the workflow runs and reaches this activity, it acts on **the same** delivery. No new delivery is created per execution. The activity reuses the same delivery. This is useful when you have a single delivery that you want to prepare or send repeatedly, for example on a schedule or after an approval step.

<!-- by default, the list shows unfinished deliveries in the Deliveries folder. You can browse other folders to select a delivery from another campaign. You choose the action to perform (prepare, prepare and start, send a proof, and so on).-->

* Select **New, created from a template** when you want a **new** delivery to be created every time the activity runs. Pick the delivery template using the **Select template** button. Each execution generates a new delivery based on that template. Use this when each workflow execution should result in its own distinct delivery (for example one email per run).

<!-- Unlike the Continuous delivery activity, there is no “append” to a previous execution—each run produces a separate delivery. -->

>[!NOTE]
>
>The **Specified in the transition** and **Computed by script** options, used for advanced use cases, can only be configured in the Client Console. See the [Campaign v8 documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/wf-activities/action-activities/delivery){target="_blank"}.

## Select the action to perform {#action-to-execute}

In this section, choose what the activity does with the delivery. The following options are available:

![Screenshot showing the actions to execute in the automated delivery](../assets/automated-delivery2.png){zoomable="yes"}

* **Save**: Creates and saves the delivery without analyzing or sending it.
* **Estimate the target**: Calculates the delivery target to assess its potential (first analysis phase).
* **Prepare**: Runs the full analysis (target calculation and content preparation). The delivery is not sent.
* **Send a proof**: Sends a proof of the delivery.
* **Prepare and start**: Runs the full analysis (target calculation and content preparation) and sends the delivery.

## Set up the transition {#transition-to-execute}

This section allows you to choose if you want to generate transitions after the activity. The following options are available:

![Screenshot showing the transitions in the automated delivery](../assets/automated-delivery3.png){zoomable="yes"}

* **Generate an outbound transition**: Generates an outbound transition when the activity finishes.
* **Transition label**: Allows you to customize the label displayed on the transition in the canvas.
* **Process errors**: Adds an additional transition for handling errors.

## Define a modification script {#script}

You can use a script to change the activity's behavior, for example, delivery parameters such as the activity label. Use this when you need custom logic for this activity.

Click **Create script** and write your modification logic in the editor.

## Related topics {#related}

* [About workflow activities](about-activities.md)
* [Continuous delivery](continuous-delivery.md)
* [Email, SMS, Push, Direct mail activities](channels.md)
* [Delivery templates](../../msg/delivery-template.md)
