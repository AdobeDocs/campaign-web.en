---
title: Add custom filters
description: Learn how to add custom filters as quick-access fields in the filters pane of a list view.
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
---
# Add custom filters {#custom-filters}

The **[!UICONTROL Inventory list configuration]** > **[!UICONTROL Custom filters]** section lets you choose which attributes are displayed as quick-access fields in the [filters pane](../query/filter.md) of a schema's list view, above the **[!UICONTROL Advanced filters]** rule builder.

For more information on the screen definition screen and how to access it, refer to the [Access the screen definition](schemas-browse-access.md#screen-def) section.

## Add custom filters {#add}

1. Browse to the **[!UICONTROL Schemas]** menu, and locate editable schemas using the filters. 

1. Select the schema name in the list to open it and click the **[!UICONTROL Screen edition]** button in the schema details view to access the screen definition. 

1. Go to the **[!UICONTROL Inventory list configuration]** section and click the ellipsis icon above the **[!UICONTROL Custom filters]** table, then choose **[!UICONTROL Select attributes]**.

   ![Custom filters selection](assets/schemas-custom-filters1.png)

1. Select one or multiple attributes and confirm. 

   You can select:

   * A direct attribute of the schema, for example a code or a category.
   * A link attribute, for example a brand linked to a product. In this case, the filter uses a search picker restricted to the linked schema.
   * A sub-attribute of a link, for example the full name of a linked folder, or the email of a linked recipient.

   ![Attribute picker showing direct attributes and link sub-attributes](assets/schemas-custom-filters2.png)

1. Click **[!UICONTROL Save]**. You can reorder custom filters using the up and down arrows or by dragging them. To remove a filter, click the ellipsis icon on its row and select **[!UICONTROL Delete]**.

1. Browse to the list of records for this schema and open the filters pane. The attributes you selected are displayed as **[!UICONTROL Custom filters]**, above the **[!UICONTROL Advanced filters]** rule builder.

   ![Custom filters displayed in the filters pane](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >A custom filter based on a date or date and time attribute is displayed as a date range picker.

1. Enter or select a value in one of the custom filters to refine the list. 

## Restrict values for a link-type custom filter {#settings}

For a custom filter based on a link attribute, you can restrict which values are available in the picker.

>[!NOTE]
>
>The **[!UICONTROL Edit]** option described below is only available for custom filters based on a link attribute. Custom filters based on other attribute types can only be reordered or removed.

1. On the row of a link-type custom filter, click the ellipsis icon and select **[!UICONTROL Edit]**.

   ![Edit option on a link-type custom filter](assets/schemas-custom-filters4.png)

1. In the **[!UICONTROL Filter settings]** tab, click **[!UICONTROL Edit filter]** and use the query modeler to define a condition that restricts the values available in the picker. For example, restrict a delivery filter to deliveries using the email channel.

   ![Filter settings tab in the Link settings dialog](assets/schemas-custom-filters5.png)

1. Confirm your changes.
