---
audience: end-user
title: Create audiences
description: Learn how to create audiences in Adobe Campaign Web
badge: label="Beta" 
---

# Create audiences {#create-audiences}

Campaign Web allows you to create create workflows where you can combine existing audiences into a visual canvas and leverage various activites (split, exclude…) to create new audiences.

Once done, the resulting audiences are saved backed into Campaign Web along with existing audiences and can be leveraged in standalone deliveries or campaigns to target individuals.

## Create your first audience {#create}

To create an audience, follow these steps:

1. Navigate to the **[!UICONTROL Audiences]** menu and click **[!UICONTROL Create Audience]** button in the top-right corner.
1. Provide a label for the audience.
1. Expand the Additional options section to configure advancer parameters for the audience.

    >[!NOTE]
    >
    >By default, audiences are created into the Profiles and Targets / Lists explrer menu. You can change the default storage location in the **[!UICONTROL Folder]** field.

1. Once the audience settings are configured, click **[!UICONTROL Create Audience]** button.

1. A workflow canvas displays, with two default activites:

    * **[!UICONTROL Build audience]**: the starting point of your workflow. This activity allows you to select one or multiple audiences as a basis for your workflow,
    * **[!UICONTROL Save audience]**: the last step of your workflow. This activity allows you to save the result of your workflow into a new audience.

1. Configure your workflow by adding as many activites as needed activities. For more information on how the configure the various activites, refer to the [workflows documentation](../workflows/activities/about-activities.md). 

    >[!NOTE]
    >
    >Channel activities are not available for use in audience workflows.

    ![](assets/audience-creation-canvas.png)

1. When your workflow is ready, click **[!UICONTROL Start]** to execute it.

1. The workflow is saved into the **[!UICONTROL Workflows]** list, and the resulting audience(s) into the **[!UICONTROL Audiences]** list. [Learn how to monitor & manage audiences](access-audiences.md)
