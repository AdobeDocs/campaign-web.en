---
audience: end-user
title: Use the Join workflow activity
description: Learn how to use the Join workflow activity
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
---
# Join {#join}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Multiple workflow branches and Join activity"
>abstract="Multiple branches are now supported. Instead of using a Fork, you can click Add branch on the toolbar. The AND-join activity has also been improved. It is now a generic Join activity that lets you choose between AND and OR join options."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="AND-join activity"
>abstract="The **And-join** activity allows you to synchronize multiple execution branches of a workflow. It is triggered once all of the preceding activities have finished. This ensures that certain activities are completed before continuing to execute the workflow."


>[!CONTEXTUALHELP]
>id="acw_orchestration_join"
>title="Join activity"
>abstract="The **Join** activity lets you merge multiple inbound transitions. Choose whether to continue when all inbound transitions are complete (AND) or when any inbound transition is complete (OR)."

The **Join** activity is a **Flow control** activity. It synchronizes multiple execution branches of a workflow. 
You can choose how inbound transitions are evaluated:

* **AND**: Continues only after all selected inbound transitions are activated.
* **OR**: Continues as soon as one selected inbound transition is activated.

When **AND** is selected, this activity triggers its outbound transition only after all the inbound transitions are activated. In other words, it activates once all preceding activities are completed. This ensures that certain activities are finished before continuing to execute the workflow.

When **OR** is selected, execution continues as soon as one of the selected inbound transitions is activated. It does not wait for every branch.

## Configure the Join activity {#join-configuration}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Merging options"
>abstract="Select which activities you want to join. In the **Primary set** drop-down, choose which inbound transition population you want to keep."

Follow these steps to configure the **Join** activity:

1. Add multiple activities, such as channel activities, to form at least two different execution branches. You can use a **Fork** or add a separate branch using the **Add branch** (+) toolbar button. See [Orchestrate activities](../orchestrate-activities.md#toolbar).

   ![Screenshot showing two branches.](../assets/workflow-join.png)

1. Add a **Join** activity to any of the branches.

   ![Screenshot showing the Join activity added.](../assets/workflow-join2.png)

1. In the join options, choose **AND** or **OR** and click **Continue**.
1. In the **Merging options** section, check all the previous activities you want to join.
1. In the **Primary set** drop-down, choose which inbound transition population to keep. The outbound transition can only contain one of the inbound transition populations.

   >[!NOTE]
   >
   >The **Primary set** field is only available for the **AND** join option.

   ![Screenshot showing join configured.](../assets/workflow-join3.png)

## Example {#join-example}

The following example shows two workflow branches with an email and SMS delivery. The **Join** activity, set to **AND**, triggers when both inbound transitions are enabled. Push notifications are sent only after both deliveries are completed. If you set the join option to **OR**, the push messages are sent as soon as the first inbound delivery activity is completed.

![Example of a workflow with two branches, showing email and SMS delivery followed by push notifications.](../assets/workflow-join4.png){zoomable="yes"}