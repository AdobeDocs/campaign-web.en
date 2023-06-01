---
audience: end-user
title: Use the Build audience workflow activity
description: Learn how to use the Build audience workflow activity
badge: label="Alpha" type="Positive"
---

# Build audience {#build-audience}

This activity allows you to define an audience. You can either select an existing audience or use the rule builder to define your own query. 

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuration

Follow these steps to configure the **Build audience** activity:

1. Add a Build audience activity. 
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

## Example