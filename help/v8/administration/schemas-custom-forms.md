---
title: Work with custom forms
description: Learn how to create, edit, and manage records in custom schemas using data entry forms.
---
# Work with custom forms {#custom-forms}

Custom forms are data entry interfaces that are directly linked to schemas. Each custom form corresponds to a specific schema and allows you to view, create, edit, and delete records in that schema's data table directly from the interface. They provide a user-friendly way to manage data in custom tables without needing to use the client console.

>[!NOTE]
>
>A custom form is only available for schemas that have a form definition configured. The form definition is part of the schema configuration and defines which fields are displayed, how they are organized, and how users interact with the data. If a schema doesn't have a form definition, you can only view the schema details but cannot manage records through a form interface.

## Access custom forms {#access-forms}

To access a custom form:

1. Navigate to **[!UICONTROL Administration]** > **[!UICONTROL Schemas]**.
1. Apply the **[!UICONTROL Editable]** filter to view schemas that have form definitions configured.
1. Select a schema from the list.
1. In the Explorer view, you will see an entry for the custom schema that allows you to access the form interface.

![Custom form access in Explorer view](assets/schemas-form-access.png)

## Create and edit records {#create-edit}

From the custom form, you can:

* **Create new records**: Click the **[!UICONTROL Create]** button to add a new record to the custom schema.
* **Edit existing records**: Select a record from the list and click to open it in edit mode.
* **Delete records**: Use the delete action available in the record details.

![Custom form showing create and edit actions](assets/schemas-form-actions.png)

When editing records, linked fields are automatically populated based on the relationships defined in your schemas. For example, if a purchase is linked to a product, and the product is linked to a brand, the relationships are automatically maintained when you create or edit records.

>[!NOTE]
>
>Changes made to custom forms are immediately available. Unlike previous versions, you don't need to publish or refresh the interface to see your updates.

## Navigate with custom filters {#custom-filters}

You can apply custom filters to navigate and find specific records in your custom forms. Filters help you refine the list view to display only the records that match your criteria.

By default, filters are available in the filter panel. You can apply filters on any field to quickly find the records you need. For example, you can filter purchases by price, products by brand, or any other field in your schema.

![Custom form with filters applied](assets/schemas-form-filters.png)

## Default columns and list configuration {#default-columns}

When you access a custom form, the list view displays default columns based on the fields referenced in the form definition. These default columns are fixed, but you can add sections to organize the display further.

The default columns are automatically determined from the schema configuration. If you need to customize which columns appear or how they are organized, you can configure this in the screen definition for the schema.

## Custom form capabilities and limitations {#form-capabilities}

Custom forms provide a powerful way to manage data, with the following capabilities:

* **Layout configuration**: Forms support sections, separators, and field organization. By default, fields are displayed in two columns, but you can configure them to span a single column.
* **Visibility conditions**: You can set visibility conditions for fields and sections based on other field values.
* **Mandatory fields**: You can mark fields as mandatory to ensure data completeness.
* **Linked data**: Forms automatically handle relationships between schemas. For example, if you have a purchase linked to a product, and the product linked to a brand, these relationships are maintained automatically.
* **Collection lists**: You can display related data in collection lists within the form detail view.

>[!NOTE]
>
>Custom forms in the Web User Interface provide a streamlined experience compared to the client console. While they don't include all advanced features available in the client console form engine (such as complex variables and advanced scripting), they cover most common use cases and are much faster to configure and use. Changes are immediately available without requiring publication or refresh.
