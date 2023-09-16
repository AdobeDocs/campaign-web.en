---
audience: end-user
title: Create audiences
description: Learn how to create audiences in Adobe Campaign Web
badge: label="Beta" 
---

# Create audiences {#create-audiences}


>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."

Campaign Web allows you to create workflows where you can combine existing audiences into a visual canvas. By incorporating various workflow activities such as **Split** or **Exclude**, you can generate new and refined audiences.

Once you've crafted your workflow, the resulting audiences are automatically stored within Campaign Web alongside your existing ones. These audiences can then be targeted in campaigns or standalone deliveries.

To create an audience, follow these steps:

1. Navigate to the **[!UICONTROL Audiences]** menu and click the **[!UICONTROL Create Audience]** button located in the top-right corner.
1. Provide a label for your audience.
1. Expand the **[!UICONTROL Additional options]** section to configure advanced audience parameters.

    By default, audiences are created into the **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Lists]** explorer menu. You can change the default storage location using the **[!UICONTROL Folder]** field.

    ![](assets/audiences-settings.png)

1. Once you have configured the audience settings, click the **[!UICONTROL Create Audience]** button.

1. A workflow canvas appears, featuring two default activites:

    * **[!UICONTROL Build audience]**: This is the starting point of your workflow, allowing you to create an audience and use it as a foundation for your workflow.
    * **[!UICONTROL Save audience]**: This represents the final step in your workflow, enabling you to save the results as a new audience.

1. Customize your workflow by adding as many activites as required. For more information on how the configure workflow activities, refer to the [workflows documentation](../workflows/activities/about-activities.md). 

    >[!NOTE]
    >
    >Channel activities are not available for use in audience workflows.

    ![](assets/audience-creation-canvas.png)

1. When your workflow is ready, click **[!UICONTROL Start]** to execute it.

1. The workflow is saved in the **[!UICONTROL Workflows]** list, while the resulting audience(s) are accessible in the **[!UICONTROL Audiences]** list. [Learn how to monitor & manage audiences](access-audiences.md)
