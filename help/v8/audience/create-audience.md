---
audience: end-user
title: Create audiences
description: Learn how to create audiences in Adobe Campaign Web
badge: label="Beta"
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
---
# Create audiences {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="From this screen, you can access the list of all audiences that can be targeted in your deliveries. Click **Create** to create new audiences into a visual canvas using various workflow activities such as **Split** or **Exclude**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."

Campaign Web allows you to create new audiences into a visual workflow canvas. Beyond starting from scratch to create a simple audience, you can also leverage workflow activities to refine your audience. For instance, you can combine multiple audiences into a single one, enrich your audience with external attributes, or divide a it into multiple audiences based on rules of your choice.

Once you've crafted your workflow, the resulting audiences are automatically stored within Campaign database alongside your existing ones. These audiences can then be targeted in workflows or standalone deliveries.

## Create your first audience {#create}

To create an audience, follow these steps:

1. Navigate to the **[!UICONTROL Audiences]** menu and click the **[!UICONTROL Create Audience]** button located in the top-right corner.
1. Provide a label for your audience.
1. Expand the **[!UICONTROL Additional options]** section to configure advanced audience parameters.

    By default, audiences are created into the **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Lists]** explorer menu. You can change the default storage location using the **[!UICONTROL Folder]** field.

    ![](assets/audiences-settings.png)

1. Once you have configured the audience settings, click the **[!UICONTROL Create Audience]** button. A workflow canvas appears, featuring two default activites:

    * **[!UICONTROL Build audience]**: This is the starting point of your workflow, allowing you to create an audience and use it as a foundation for your workflow.

    * **[!UICONTROL Save audience]**: This represents the final step in your workflow, enabling you to save the workflow results as a new audience.

1. Open the **[!UICONTROL Build audience]** activity and use the rule builder to define the population to include into your audience by filtering data contained in the database. [Learn how to configure a Build audience activity](../workflows/activities/build-audience.md)

1. If you want to perform additional operations on the population targeted into the workflow, add as many activities as required and connect them together. For more information on how the configure workflow activities, refer to the [workflows documentation](../workflows/activities/about-activities.md). 

    >[!NOTE]
    >
    >Channel activities are not available for use in audience workflows.

    ![](assets/audience-creation-canvas.png)

1. Configure the **[!UICONTROL Save audience]** activity to specify how you want to save the population computed upstream in the workflow. [Learn how to configure a Save audience activity](../workflows/activities/save-audience.md)

1. When your workflow is ready, click **[!UICONTROL Start]** to execute it.

The workflow is saved in the **[!UICONTROL Workflows]** list, while the resulting audience(s) are accessible in the **[!UICONTROL Audiences]** list. [Learn how to monitor & manages audiences](manage-audience.md)

You can now use this audience as the main target of a delivery. [Learn more](add-audience.md)

## Audience workflow example {#example}

The example below shows an audience workflow configured to target female customers living in New York and create two new audiences depending on their latest purchase (Yoga or Running gear).

![](assets/audiences-example.png)

1. The **[!UICONTROL Build audience]** activity targets all female profiles living in New York.
1. The **[!UICONTROL Enrichment]** activity enriches the audience with information from the Purchases table to identify which type of product the customers purchased.
1. The **[!UICONTROL Split]** activity divides the workflow into two paths based on the customers' latest purchase.
1. The **[!UICONTROL Save audience]** activities at the end of each path  create two new audiences into the database including the population computed in each path.
