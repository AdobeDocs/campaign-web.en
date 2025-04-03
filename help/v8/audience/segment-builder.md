---
audience: end-user
title: Build an audience with Campaign rule builder
description: Learn how to work with the rule builder
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
---
# Work with the rule builder {#segment-builder}

The rule builder lets you define the population targeted by your delivery by filtering data contained in the database. Use it to build an audience either from a workflow using a **[!UICONTROL Build audience]** activity, or directly when creating a delivery to create a one-time audience.

* [Learn how to create and save an audience](create-audience.md)
* [Learn how to create a one-time audience for a delivery](one-time-audience.md)

## The palette

The palette, located on the left side, contains all the elements that you can filter on to create your audience. Use the search bar to find elements quickly. Move the tiles contained in the palette into the center canvas to configure them and take them into account.

![](assets/segment-builder2.png)[The palette interface showing filtering options and tabs]{zoomable="yes"}{width="70%" align="left"}
    
The palette is divided into two tabs:

* **Attributes**: This tab provides access to all available fields from the schema. The list of fields depends on the targeting schema defined in the email template.

* **Audiences**: This tab lets you filter using one of the existing audiences defined in the Campaign Classic console or from Adobe Experience Platform. Learn how to monitor and manage audiences in [this section](manage-audience.md).

    >[!NOTE]
    >
    >To use Adobe Experience Platform audiences, configure the integration with Destinations. Refer to the [Adobe Experience Platform Destinations documentation](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html){target="_blank"}.

## The canvas

The canvas is the central zone where you can configure and combine rules based on the elements added from the palette. To add a new rule, drag a tile from the palette and drop it onto the canvas. Context-specific options are presented based on the type of data being added.

![](assets/segment-builder4.png)[The canvas interface showing rule configuration options]{zoomable="yes"}{width="70%" align="left"}

## The rule properties pane

On the right side, the **Rule properties** pane lets you perform the actions listed below.

![](assets/segment-builder5.png)[The rule properties pane showing available actions]{zoomable="yes"}{width="70%" align="left"}

* **View results:** Displays the list of profiles targeted by the audience.
* **Code view**: Shows a code-based version of the audience in SQL.
* **Display advanced attributes**: Check this option to view the complete list of attributes in the left palette, including nodes, groupings, 1-1 links, and 1-N links.
* **Calculate**: Updates and displays the number of profiles targeted by your query.
* **Select or save filter**: Use a predefined filter to filter your query, or save your query as a new filter for future reuse. [Learn how to work with predefined filters](../get-started/predefined-filters.md).

    >[!IMPORTANT]
    >
    >In this version of the product, some predefined filters are not available in the user interface. You can still use them. [Learn more](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations).

* **Attributes**: Displays a description of the created audience.

## Example

In this example, an audience is built to target all customers living in Atlanta or Seattle and born after 1980.

1. In the **Attributes** tab of the palette, search for the **Date of birth** field. Drag the tile and drop it onto the canvas.

    ![](assets/segment-builder6.png)[Adding the Date of birth field to the canvas]{zoomable="yes"}

1. In the canvas, choose the **After** operator and enter the desired date.

    ![](assets/segment-builder7.png)[Configuring the After operator for the Date of birth field]{zoomable="yes"}

1. In the palette, search for the **City** field and add it to the canvas below the first rule.

    ![](assets/segment-builder8.png)[Adding the City field to the canvas]{zoomable="yes"}

1. In the text field, enter the first city name, then press enter.

    ![](assets/segment-builder9.png)[Entering the first city name in the City field]{zoomable="yes"}

1. Repeat this action for the second city name.

    ![](assets/segment-builder10.png)[Entering the second city name in the City field]{zoomable="yes"}

1. Click **View results** to display the list and number of recipients matching the query. Add columns to visualize and check the data. In this example, add the **City** column to see Atlanta and Seattle.

    ![](assets/segment-builder11.png)[Viewing results with the City column added]{zoomable="yes"}

1. Click **Confirm**.