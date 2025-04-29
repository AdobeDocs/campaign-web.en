---
audience: end-user
title: Use the Save audience workflow activity
description: Learn how to use the Fork workflow activity
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
---
# Save audience {#save-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Save an audience"
>abstract="Use this activity to update an existing audience or create a new audience from the population computed upstream in the workflow. The audiences created are added to the list of audiences, and available via the **Audiences** menu."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Generate outbound transition"
>abstract="Use this option if you want to add a transition after the **Save audience** activity."

The **Save audience** activity is a **Targeting** activity. This activity allows you to update an existing audience or create a new audience from the population computed upstream in a workflow. The audiences created are added to the list of application audiences, and are made available via the **Audiences** menu.

This activity is primarily used to retain population groups computed in the same workflow by converting them into reusable audiences. Connect it to other targeting activities such as a **Build audience** or a **Combine** activity.

## Configure the Save audience activity {#save-audience-configuration}

Follow these steps to configure the **Save audience** activity:

![Description: Workflow configuration for Save audience activity](../assets/workflow-save-audience.png)

1. Add a **Save audience** activity to your workflow.

1. In the **Mode** drop-down, select the action you want to perform:

    * **Create or update an existing audience**: Define an **Audience label**. If the audience already exists, it is updated; otherwise, a new audience is created.

    * **Update an existing audience**: Choose the **Audience** you want to update from the list of existing audiences.

1. Select the **Update mode** that applies to existing audiences:

    * **Replace audience content with new data**: All audience content is replaced, and old data is lost. Only the data from the inbound transition of the **Save audience** activity is retained. This option erases the audience type and the targeting dimension of the updated audience.

    * **Complete audience with new data**: The old audience content is retained, and the data from the inbound transition of the **Save audience** activity is added to it.

1. Check the **Generate an outbound transition** option if you want to add a transition after the **Save audience** activity.

The content of the saved audience is then available in the detail view of the audience, which can be accessed from the **Audiences** menu. The columns available in this view correspond to the columns of the inbound transition of the workflow's **Save audience** activity.

## Example {#save-audience-example}

The following example illustrates a simple audience update from targeting. A scheduler runs the workflow once a month. A query retrieves all profiles subscribed to the different applications available. The **Save audience** activity updates the audience by removing profiles that have unsubscribed from the service since the last workflow execution and adding newly subscribed profiles.