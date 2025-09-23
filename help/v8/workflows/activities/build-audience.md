---
audience: end-user
title: Use the Build audience workflow activity
description: Learn how to use the Build audience workflow activity
exl-id: c07bb025-51b7-428e-ba00-cd552f0db9d4
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
* Build a new audience with the query modeler by defining and combining filtering criteria.

>[!NOTE]
>
>Audiences loaded from a file cannot be targeted using a Build audience activity. To do this, you need to use a **Load file** activity followed by a **Reconciliation** activity. [Learn more](../../audience/about-recipients.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configure the Build audience activity {#build-audience-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_audienceselector"
>title="Audience"
>abstract="Select your audience, the same way you use an audience when designing a new delivery."

Follow these steps to configure the **Build audience** activity:

![Screenshot showing the workflow audience configuration interface.](../assets/workflow-audience.png)

1. Add a **Build audience** activity.
1. Define a label.
1. Define the audience type: **Create your own** or **Read audience**.
1. Configure your audience by following the steps detailed in the tabs below.

>[!BEGINTABS]

>[!TAB Create your own (query)]

To create your own query, follow these steps:

1. Select **Create your own (query)**.
1. Choose the **Targeting dimension**. The targeting dimension lets you define the population targeted by the operation, such as recipients, contract beneficiaries, operators, or subscribers. By default, the target is selected from the recipients. [Learn more about targeting dimensions](../../audience/targeting-dimensions.md#targeting)
1. Choose the **Filtering dimension** by clicking the icon next to the targeting dimension. The filtering dimension allows you to apply filters to the targeted population by referencing related criteria without changing the main targeting dimension. [Learn more about targeting dimensions](../../audience/targeting-dimensions.md#filtering)
1. Click **Continue**.
1. Use the query modeler to define your query, the same way you create an audience when designing a new email. [Learn how to work with the query modeler](../../query/query-modeler-overview.md)

>[!TAB Read audience]

To select an existing audience, follow these steps:

1. Select **Read audience**.
1. Click **Continue**.
1. Select your audience, the same way you use an audience when designing a new delivery. Refer to this [section](../../audience/add-audience.md).

>[!ENDTABS]

## Examples {#build-audience-examples}

Here is an example of a workflow with two **Build audience** activities. The first one targets the poker players audience, followed by an email delivery. The second one targets the VIP clients audience, followed by an SMS delivery.

![Screenshot showing an example workflow with two Build audience activities targeting different audiences.](../assets/workflow-audience-example.png)