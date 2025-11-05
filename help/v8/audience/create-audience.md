---
audience: end-user
title: Create audiences
description: Learn how to create audiences in Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
---
# Create audiences {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="From this screen, you can access the list of all audiences that can be targeted in workflows or standalone deliveries. Click **Create** to create a new audience into a visual canvas.<br/><br/>Beyond starting from scratch to create a simple audience, you can also leverage workflow activities to refine your audience. For instance, you can combine multiple audiences into a single one, enrich your audience with external attributes, or divide it into multiple audiences based on rules of your choice."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

## About audience creation

Campaign Web allows you to create new audiences in a visual workflow canvas. Beyond starting from scratch to create a simple audience, you can also leverage workflow activities to refine your audience. For instance, you can combine multiple audiences into a single one, enrich your audience with external attributes, or divide it into multiple audiences based on rules of your choice.

Once you craft your workflow, the resulting audiences are automatically stored within the Campaign database alongside your existing ones. These audiences can then be targeted in workflows or standalone deliveries.

The **[!UICONTROL Origin]** column indicates audiences' origins: **[!UICONTROL Adobe Campaign]** audiences are created in the Adobe Campaign v8 console or Web User Interface, while **[!UICONTROL Adobe Experience Platform:]** audiences are created within Adobe Experience Platform and integrated into Campaign using the Adobe Sources and Destinations integration.

➡️ [Discover this feature in video](#video) 

## Permissions for custom operator groups

When creating a new audience, a workflow is automatically created and stored in the **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Jobs]** / **[!UICONTROL Targeting workflows]** folder.

If you are assigned to a custom operator group and encounter a "You do not have rights" error when creating audiences, you need to ensure your operator group has the necessary permissions to this folder.

To resolve this, an administrator must add your custom operator group to the folder security section in the Campaign console. [Learn how to manage permissions on folders](../get-started/permissions.md#folder-permissions)

## Create your first audience {#create}

To create an audience, follow these steps:

1. Navigate to the **[!UICONTROL Audiences]** menu, and click the **[!UICONTROL Create Audience]** button located in the top-right corner.

1. A new workflow is automatically created, allowing you to combine activities to generate your audience. By default, the canvas contains two main activities:

    * The "Query" **[!UICONTROL Build audience]** activity is the starting point of your workflow. It allows you to create an audience and use it as a foundation for your workflow.

    * The "New audience" **[!UICONTROL Save audience]** activity represents the final step in your workflow. It enables you to save the results as a new audience.

    ![A blank audience creation canvas with two default activities: Build audience and Save audience.](assets/create-audience-blank.png){zoomable="yes"}

    >[!IMPORTANT]
    >
    >Audience workflows are stored in the **Workflows** menu, alongside your other Campaign workflows. They are specifically designed to build audiences and are identifiable by their vertical canvas.
  
1. For better readability, change the name of the workflow in the workflow settings' **Label** field. [Learn how to configure workflow settings](../workflows/workflow-settings.md)

1. Open the **[!UICONTROL Build audience]** activity, and use the query modeler to define the population to include in your audience by filtering data contained in the database. [Learn how to configure a Build audience activity](../workflows/activities/build-audience.md)

1. If you want to perform additional operations on the population targeted in the workflow, add as many activities as required and connect them together. For more information on how to configure workflow activities, refer to the [workflows documentation](../workflows/activities/about-activities.md). 

    >[!NOTE]
    >
    >Channel activities are not available for use in audience workflows.

    ![An audience creation canvas with multiple activities connected to refine the audience.](assets/audience-creation-canvas.png){zoomable="yes"}

1. Configure the **[!UICONTROL Save audience]** activity to specify how you want to save the population computed upstream in the workflow. [Learn how to configure a Save audience activity](../workflows/activities/save-audience.md)

1. When your workflow is ready, click **[!UICONTROL Start]** to execute it.

The workflow is saved in the **[!UICONTROL Workflows]** list, while the resulting audience(s) are accessible in the **[!UICONTROL Audiences]** list with the label defined in the **Save audience** activity. Learn how to monitor and manage audiences in [this section](manage-audience.md)

You can now use this audience as the main target of a delivery. [Learn more](add-audience.md)

## Audience workflow example {#example}

The example below shows an audience workflow configured to target female customers living in New York and create two new audiences depending on their latest purchase (Yoga or Running gear).

![An audience workflow example targeting female customers in New York and splitting them based on their latest purchase.](assets/audiences-example.png){zoomable="yes"}

1. The **[!UICONTROL Build audience]** activity targets all female profiles living in New York.
1. The **[!UICONTROL Enrichment]** activity enriches the audience with information from the Purchases table to identify which type of product the customers purchased.
1. The **[!UICONTROL Split]** activity divides the workflow into two paths based on the customers' latest purchase.
1. The **[!UICONTROL Save audience]** activities at the end of each path create two new audiences in the database, including the population computed in each path.

## Edit an audience {#edit}

You can modify an audience generated from a workflow whenever necessary by re-executing its corresponding workflow. This allows you to refresh audience data or refine the audience by adjusting the query to suit your needs.

1. Navigate to the **Audiences** menu, and open the audience you want to edit.
1. In the **Overview** tab, the **Last workflow** section provides a link to the workflow used to generate the audience. Click on it to access the workflow.
1. Make the desired changes, and click the **Start** button to rerun the workflow. Upon completion, the audience resulting from the workflow is automatically updated with the latest workflow results.
 
By default, rerunning an audience workflow replaces the entire content of the audience with new data, causing the loss of previous data.

If you prefer not to replace the existing audience results, configure the **Save audience** activities to align with your requirements. For example, you can change the **Audience label** field to store the new results in a new audience or add the new results to the existing audience content without erasing previous data. [Learn how to configure a Save audience activity](../workflows/activities/save-audience.md)

![The Save audience activity configuration screen with options to adjust audience saving behavior.](assets/edit-audience-save.png){zoomable="yes"}

## How-to video {#video}

Learn how to build and manage audiences, how to select audiences for a delivery, and define control groups.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)