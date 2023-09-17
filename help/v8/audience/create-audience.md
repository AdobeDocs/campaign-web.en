---
audience: end-user
title: Create audiences
description: Learn how to create audiences in Adobe Campaign Web
badge: label="Beta" 
---

# Create audiences {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="From this screen, you can create and combine audiences into a visual canvas. Add various workflow activities such as **Split** or **Exclude** to generate new and refined audiences."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."

Campaign Web allows you to create new audiences into a visual workflow canvas. Beyond starting from scratch to create a simple audience, you can also leverage workflow activities to refine your audiences. For instance, you can multiple audiences into a single one, enrich audiences with external attributes, or divide a given audience into multiple ones.

Once you've crafted your workflow, the resulting audiences are automatically stored within Campaign database alongside your existing ones. These audiences can then be targeted in campaigns or standalone deliveries.

The main steps to create an audience are as follows:

1. Create an audience workflow.
1. Configure a Build audience activity to query the database based on your needs.
1. Add workflow activities to refine your audience (optional).
1. Configure a Save audience activity.
1. Run the workflow to save the resulting audience(s) into the database.


## Create your first audience {#create}

To create an audience, follow these steps:

1. Navigate to the **[!UICONTROL Audiences]** menu and click the **[!UICONTROL Create Audience]** button located in the top-right corner.
1. Provide a label for your audience.
1. Expand the **[!UICONTROL Additional options]** section to configure advanced audience parameters.

    By default, audiences are created into the **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Lists]** explorer menu. You can change the default storage location using the **[!UICONTROL Folder]** field.

    ![](assets/audiences-settings.png)

1. Once you have configured the audience settings, click the **[!UICONTROL Create Audience]** button.

1. A workflow canvas appears, featuring two default activites:

    * **[!UICONTROL Build audience]**: This is the starting point of your workflow, allowing you to create an audience and use it as a foundation for your workflow. [Learn how to configure a Build audience activity](../workflows/activities/build-audience.md)

    * **[!UICONTROL Save audience]**: This represents the final step in your workflow, enabling you to save the results as a new audience. [Learn how to configure a Save audience activity](../workflows/activities/save-audience.md)

1. If you want to perform additional operation after the **[!UICONTROL Build audience]** activity, add as many activities as required into your workflow. For more information on how the configure workflow activities, refer to the [workflows documentation](../workflows/activities/about-activities.md). 

    >[!NOTE]
    >
    >Channel activities are not available for use in audience workflows.

    ![](assets/audience-creation-canvas.png)

1. When your workflow is ready, click **[!UICONTROL Start]** to execute it.

1. The workflow is saved in the **[!UICONTROL Workflows]** list, while the resulting audience(s) are accessible in the **[!UICONTROL Audiences]** list. [Learn how to monitor & manage audiences](access-audiences.md)

## Audience workflow example {#example}

The example below shows an audience workflow configured to target female customers living in New York and create two new audiences depending on their center of interest into Yoga or Running gear. The two audiences are enriched with additional information related to the customers' purchases.

ADD SCREENSHOT

1. The Build audience activity targets all Female profiles living in New York.
1. The Enrichment activity enriches the audience with attributes from the Purchases table.
1. The Split activity divides the workflow into two paths based on the customers' centers of interest.
1. The Save audience activities at the end of each path to save each audience into the database.
