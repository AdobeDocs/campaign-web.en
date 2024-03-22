---
audience: end-user
title: Create audiences
description: Learn how to create audiences in Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
---
# Create audiences {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Audience composition"
>abstract="Create new audiences into a visual workflow canvas. Beyond starting from scratch to create a simple audience, you can also leverage workflow activities to refine your audience. Combine multiple audiences into a single one, enrich your audience with external attributes, or divide a it into multiple audiences based on rules of your choice."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"

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

➡️ [Discover this feature in video](#video) 

## Create your first audience {#create}

To create an audience, follow these steps:

1. Navigate to the **[!UICONTROL Audiences]** menu and click the **[!UICONTROL Create Audience]** button located in the top-right corner.

1. A new workflow is automatically created, allowing you to combine activities to generate your audience. By default, the canvas contains two main activities:

    * The "Query" **[!UICONTROL Build audience]** activity is the starting point of your workflow, allowing you to create an audience and use it as a foundation for your workflow.

    * The "New audience" **[!UICONTROL Save audience]** activity represents the final step in your workflow, enabling you to save the results as a new audience.

    ![](assets/create-audience-blank.png){zoomable="yes"}

    >[!IMPORTANT]
    >
    >Audience workflows are stored in the **Workflows** menu, alongside your other Campaign workflows. They are specifically designed to build audiences and are identifiable by their vertical canvas.
  
1. For better readability, we recommend changing the name of the workflow in the workflow settings' **Label** field. [Learn how to configure workflow settings](../workflows/workflow-settings.md)

1. Open the **[!UICONTROL Build audience]** activity and use the query modeler to define the population to include into your audience by filtering data contained in the database. [Learn how to configure a Build audience activity](../workflows/activities/build-audience.md)

1. If you want to perform additional operations on the population targeted into the workflow, add as many activities as required and connect them together. For more information on how the configure workflow activities, refer to the [workflows documentation](../workflows/activities/about-activities.md). 

    >[!NOTE]
    >
    >Channel activities are not available for use in audience workflows.

    ![](assets/audience-creation-canvas.png){zoomable="yes"}

1. Configure the **[!UICONTROL Save audience]** activity to specify how you want to save the population computed upstream in the workflow. [Learn how to configure a Save audience activity](../workflows/activities/save-audience.md)

1. When your workflow is ready, click **[!UICONTROL Start]** to execute it.

The workflow is saved in the **[!UICONTROL Workflows]** list, while the resulting audience(s) are accessible in the **[!UICONTROL Audiences]** list with the label defined in the **Save audience** activity. Learn how to monitor and manage audiences in [this section](manage-audience.md)

You can now use this audience as the main target of a delivery. [Learn more](add-audience.md)

## Audience workflow example {#example}

The example below shows an audience workflow configured to target female customers living in New York and create two new audiences depending on their latest purchase (Yoga or Running gear).

![](assets/audiences-example.png){zoomable="yes"}

1. The **[!UICONTROL Build audience]** activity targets all female profiles living in New York.
1. The **[!UICONTROL Enrichment]** activity enriches the audience with information from the Purchases table to identify which type of product the customers purchased.
1. The **[!UICONTROL Split]** activity divides the workflow into two paths based on the customers' latest purchase.
1. The **[!UICONTROL Save audience]** activities at the end of each path  create two new audiences into the database including the population computed in each path.

## Edit an audience {#edit}

You can modify an audience generated from a workflow whenever necessary by re-executing its corresponding workflow. This allows you to effortlessly refresh audience data or refine the audience by adjusting the query to suit your needs.

1. Navigate to the **Audiences** menu and open the audience you want to edit.
1. In the **Overview** tab, the **Last workflow** section provides a link to the workflow used to generate the audience. Click on it to access the workflow.
1. Make the desired changes and click the **Start** button to rerun the workflow again. Upon completion, the audience resulting from the worklow is automatically updated with the latest workflow results.

By default, rerunning an audience workflow replaces the entire content of the audience with new data, causing the loss of previous data.

If you prefer not to replace the existing audience results, configure the **Save audience** activities to align with your requirements. For example, you can change the **Audience label** field to store the new results into a new audience, or add the new results to the existing audience content without erasing previous data. [Learn how to configure a Save audience acitivty](../workflows/activities/save-audience.md)

![](assets/edit-audience-save.png){zoomable="yes"}

## How-to video {#video}

Learn how to build and manage audiences, how to select audiences for a delivery, and define control groups.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)
