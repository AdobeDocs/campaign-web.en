---
audience: end-user
title: Select an existing audience
description: Learn how to select an audience
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
---

# Select an existing audience {#add-audience}
 
>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Select an existing audience"
>abstract="Browse the list to select an existing audience. Use the 'Show filters' icon to filter the list, or select a specific folder."

This section explains how to select an existing audience when defining the target population of a delivery. When defining the main target of a delivery, you can also:
* [Build a one-time audience](one-time-audience.md) using the query modeler.
* [Load an audience from an external file](file-audience.md) (for emails only).
 
Audiences that can be targeted in deliveries are accessible from the **Audience** left menu. They originate from multiple sources such as the Client console, Campaign Web audience workflows or Adobe Experience Platform. [Learn more on audiences](manage-audience.md)

To select an existing audience for your message, follow the steps below:

1. From the **Audience** section of the delivery creation assistant, click the **[!UICONTROL Select audience]** button then choose **[!UICONTROL Select audience]**. 

   ![](assets/create-audience.png){zoomable="yes"}

1. This screen displays all existing audiences, for the current folder.

    ![](assets/create-audience2.png){zoomable="yes"}

   To choose an audience from Adobe Experience Platform, browse to the `AEP Audiences folder` from the filter section of the screen. [Learn more on Adobe Experience Platform audiences](manage-audience.md#monitor)

    ![](assets/select-audience-folder.png){zoomable="yes"}

1. The filter section allows you to access filtering options to refine the audiences list. To do this, click **Add rules** to access the query modeler, which lets you create advanced filters for the list of audiences. [Learn how to use the query modeler](../query/query-modeler-overview.md)

    For example, you can define a rule to filter on the origin of the audiences, as shown below:

    ![](assets/filter-on-aep-audience.png){zoomable="yes"}

1. Click **Confirm** to add your audience as the delivery main target. Once done, you can still refine the audience using the query modeler by clicking the **Edit rules** button.

   ![](assets/refine-audience.png){zoomable="yes"}

1. You can also set a control group to measure the impact of your campaigns. The control group do not receive the message. This allows you to compare the behavior of the population which received the message with the behavior of contacts which did not. [Learn more](control-group.md)
