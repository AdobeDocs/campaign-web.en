---
audience: end-user
title: Use the Build audience workflow activity
description: Learn how to use the Build audience workflow activity
badge: label="Beta" 
---

# Build audience {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Build audience activity"
>abstract="The **Build audience** activity allows you to define the audience that will enter the workflow. When sending messages in the context of a workflow, the message audience is not defined in the channel activity, but in the **Build audience** activity."


The **Build audience** activity is a **Targeting** activity. This activity allows you to define the audience that will enter the workflow. When sending messages in the context of a workflow, the message audience is not defined in the channel activity, but in the **Build audience** activity.

To define the audience population, you can:

* Select an existing audience, created as a list in the client console.
* Select an Adobe Experience Platform audience. 
* Build a new audience with the rule builder by defining and combining filtering criteria.

>[!NOTE]
>
>In this context, you cannot load an audience from a file. For this, you need to create a standalone email delivery. [Learn more](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configure the Build audience activity{#build-audience-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Select the targeting dimension"
>abstract="The targeting dimension lets you define the population targeted by the operation: recipients, contract beneficiaries, operator, subscribers, etc. By default, the target is selected from the recipients."


Follow these steps to configure the **Build audience** activity:

![](../assets/workflow-audience.png)

1. Add a **Build audience** activity. 
1. Define a label.
1. Define the audience type: **Create your own** or **Read audience**. 

To create your own query, follow these extra steps:

1. Select **Create your own (query)**.
1. Choose the **Targeting dimension**. The targeting dimension lets you define the population targeted by the operation: recipients, contract beneficiaries, operator, subscribers, etc. By default, the target is selected from the recipients. Refer to the [v8 documentation](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Click **Continue**.
1. Use the rule builder to define your query, the same way you create an audience when designing a new email. Refer to this [section](../../audience/segment-builder.md).

To select an existing audience, follow these steps:

1. Select **Read audience**.
1. Click **Continue**.
1. Select your audience, the same way you use an audience when designing a new email. Refer to this [section](../../audience/add-audience.md).

>[!IMPORTANT]
>
>If you want to use a **[!UICONTROL Build audience]** activity targeting an Experience Platform audience, you need to add a **[!UICONTROL Change dimension]** activity after it, to ensure that the audience's targeting dimension is set to "Recipient". A workflow example is available at the bottom of this page.

## Examples{#build-audience-examples}

Here is an example of a workflow with two **Build audience** activities. The first one targets the poker players audience, followed by an email delivery. The second one targets the VIP clients audience, followed by an SMS delivery.

![](../assets/workflow-audience-example.png)

Here is another workflow example where an Adobe Experience Platform audience is combined with an Adobe Campaign audience. To allow these audiences to be combined, a **[!UICONTROL Change dimension]** activity with the "Recipient" targeting dimension is added after the Adobe Experience Platform audience. [Learn how to configure a Change dimenson activity](change-dimension.md)

![](../assets/workflow-audience-aep.png)
