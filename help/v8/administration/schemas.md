---
title: Work with schemas
description: Learn how to work with schemas.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
---
# Work with schemas {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Schemas"
>abstract="Adobe Campaign uses XML-based schemas to define the physical and logical structure of data within the application. From this screen, you can view all existing schemas, access schema details, configure custom forms, and create or extend schemas directly from the Web User Interface."

## About schemas {#about}

**[!DNL Adobe Campaign]** uses XML-based schemas to define the physical and logical structure of data within the application. A schema is an XML document linked to a database table that defines:

* The SQL table structure, including table name, fields, and relationships.
* The XML data structure, including elements, attributes, hierarchy, types, default values, and labels.

Schemas play a key role in:

* Mapping application data to database tables.
* Defining relationships between data objects.
* Specifying the structure and properties of each field.

Each entity in Adobe Campaign has a dedicated schema, ensuring data consistency and organization.

The schemas interface allows you to:

* [Browse and access schemas](#access) - Navigate to the schemas menu, view available schemas and explore their details.
* [Customize screen display](#screen-definition) - Configure which columns appear in list views, which fields are displayed in detail screens, add collection lists as tabs, and organize the layout to match your needs.
* [Create and manage schemas](#create-schemas) - Create new schemas, extend existing ones, or access external databases.
* [Publish and synchronize schemas](#publish) - Synchronize schema changes with the database structure.
* [Work with custom forms](#custom-forms) - Create, edit, and manage records in custom schemas using data entry forms.

Detailed information on schemas is available in the [Campaign console documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.

## Browse and access schemas {#access}

Schemas are accessible from the **[!UICONTROL Administration]** > **[!UICONTROL Schemas]** menu.

![Schemas list screen showing available schemas and filters](assets/schemas-list.png)

From this screen, you can view all existing schemas. Filters are available to help refine the list, such as displaying only editable schemas.

To open a schema, select its name. A detailed schema view displays.

![Schema details screen showing schema properties and content](assets/schema-details.png)

### Schema overview {#overview}

The **[!UICONTROL Overview]** tab provides a general view of the schema:

* The **[!UICONTROL Properties]** section displays key information, such as the schema name, namespace, and associated table name.

* The **[!UICONTROL Schema definition]** section shows details about the schema definition, including the primary key used for data reconciliation and its links with other tables. 

    Click the **[!UICONTROL Schema preview]** button to view the different fields and links composing the schema. This allows you to check the complete structure of a schema. If the schema has been extended with custom fields, you can visualize all its extensions.

* The **[!UICONTROL Content]** section displays the XML content of the schema, allowing you to switch between the source and the generated syntax.

### Schema data {#data}

The **[!UICONTROL Data]** tab provides information on the schema data.

![Schema data tab showing data structure and attributes](assets/schemas-data.png)

## Customize screen display {#screen-definition}

The screen definition allows you to configure how schema fields are displayed and edited in the interface. You can configure default columns for list views, customize which custom fields are displayed in detail screens, add collection lists to show related data, and organize fields into sections with separators and visibility criteria. 

Click the **[!UICONTROL Screen edition]** button in the schema details view to access the screen definition. The different lists allow you to reorder elements by using the up and down arrow icons or drag and dropping them. To remove items, click the trash icon on a specific row or select **[!UICONTROL Delete all]** from the to ellipsis icon.

![Screen definition General section](assets/schemas-general.png)

### Configure default list columns {#list-columns}

The **[!UICONTROL Inventory list configuration]** section allows you to configure which columns are displayed by default in list views. Each column shows its label and the corresponding attribute.

To add new columns to the default list:

1. Click the ellipsis icon (three dots).
1. Choose **[!UICONTROL Select columns]**.
1. Select the attributes you want to display in list views and confirm.

   ![List columns configuration](assets/schemas-list-columns.png)

### Edit custom fields {#fields}

Test profiles, Recipoient, campaigns, deliveries

Custom fields are additional attributes added to out-of-the-box schemas through the Adobe Campaign console. They allow you to customize schemas by including new attributes to suit your organization's needs. 

Custom fields can be displayed in various screens, such as profile details in the interface. You can control which fields are visible and how they appear in the interface.

![Custom fields screen showing editable attributes](assets/schemas-custom.png)

To add new custom fields to the list:

1. Click the ellipsis icon above the **[!UICONTROL List of custom fields]** table and choose **[!UICONTROL Select attributes]**.
1. Select the custom fields you want to add and confirm.

   ![Custom fields screen showing editable attributes](assets/schemas-custom2.png)

To add a separator:

1. Click the ellipsis icon above the **[!UICONTROL List of custom fields]** table.
1. Click the ellipsis icon on the separator row in the list, and select **[!UICONTROL Edit]**.
1. Enter a **[!UICONTROL Label]** for the separator and (optional) set a **[!UICONTROL Visible if]** condition to control when the separator is displayed.

   ![Separator properties dialog](assets/schemas-custom3.png)

To automatically populate the list with available custom fields:

1. Click the ellipsis icon above the **[!UICONTROL List of custom fields]** table.
1. Choose **[!UICONTROL Fill automatically the list of custom fields]**.

To configure individual field properties:

1. Click the ellipsis icon on a field row in the list and select **[!UICONTROL Edit]**.
1. Enter a custom **[!UICONTROL Label]** if you want to override the default field label.
1. Set a **[!UICONTROL Visible if]** condition to control when the field is displayed.
1. Check **[!UICONTROL Mandatory]** to make the field required.
1. Check **[!UICONTROL Read-only]** to prevent users from editing the field value.
1. Check **[!UICONTROL Span two columns]** to make the field span the full width of the form.

   ![Attribute settings dialog](assets/schemas-attribute-settings.png)

Click **[!UICONTROL Preview]** to display the custom fields in a sample screen.

![Preview custom fields](assets/schemas-custom4.png)

For detailed information on how to edit custom fields in a schema, refer to this section: [Configure custom fields](../administration/custom-fields.md).

### Add collection lists {#collection-lists}

The **List of custom lists** section allows you to define collection links, such as purchases. The related data is then displayed in profile screens through a dedicated tab.

>[!NOTE]
>
>Currently, this capability is only available for the Recipients schema. 

To add collections lists:

1. Click the ellipsis button and choose **Select custom lists**.

   ![Collection lists creation](assets/schemas-collection1.png)

1. Select one of the available custom lists, for example purchases, then click **Confirm**.

   ![Collection lists creation](assets/schemas-collection2.png)

1. Browse to the **Profiles** menu and filter profiles that have made purchases. 

   ![Collection lists creation](assets/schemas-collection3.png)

1. Click on a profile. You notice that the new tab is displayed. You can add more columns if needed. 

   ![Collection lists creation](assets/schemas-collection4.png)

## Create and manage schemas {#create-schemas}

You can create new schemas, extend existing schemas, and access external databases.

### Create or extend a schema {#create-new}

To create or extend a schema:

1. Navigate to **[!UICONTROL Administration]** > **[!UICONTROL Schemas]**.
1. Click **[!UICONTROL Create]**.

   ![Schema creation dialog](assets/schemas-create1.png)

1. Enter a namespace for your schema (for example, `cus` for custom schemas).
1. Enter a name and label, and choose if you want to create a new schema or extend an existing one.

1. Click **[!UICONTROL Create]**.
   ![Schema creation dialog](assets/schemas-create2.png)

The schema is created and the generated schema structure is displayed. 

By default, the schema is empty. You now need to a add the fields you want to include in your schema using the schema editor:

1. Click the pencil icon in the **[!UICONTROL Content]** section of the schema screen.
2. Add the needed elements and save. Here is an exemple of a custom schema structure:

   ![Schema creation dialog](assets/schemas-create3.png)

The system automatically validates the XML structure and generates the schema.

### Define the screen edition {#define-attributes}

After creating the schema, you need to define the screen edition:

In our example, we simply add two custom fields:

1. Click the ellipsis icon above the **[!UICONTROL List of custom fields]** table and choose **[!UICONTROL Select attributes]**.
1. Select the custom fields you want to add and confirm.

   ![Schema creation dialog](assets/schemas-create4.png)

For more information on screen edition, refer to this [section](#screen-definition).

## Publish and synchronize schemas {#publish}

After creating or modifying a schema, you need to publish it to synchronize the logical schema with the physical database structure.

### Publish schema changes {#publish-changes}

>[!CAUTION]
>
>Publishing schema changes modifies the database structure. Make sure you understand the impact of these changes before confirming the publication.

To publish your schema changes:

1. Navigate to **[!UICONTROL Administration]** > **[!UICONTROL Schemas]**.
1. Click **[!UICONTROL Publishing]** and confirm.

   ![Schema publication dialog showing changes to be applied](assets/schemas-publish1.png)

1. Select, in the list, the schema you want to synchronize.

   ![Schema publication dialog showing changes to be applied](assets/schemas-publish1.png)

1. Review the SQL script that will be executed to update the database structure.
1. Click **[!UICONTROL Publish]** and confirm to proceed with the publication.

>[!NOTE]
>
>The process may take some time depending on the size of your database and the complexity of the changes.

### Create a navigation entry {#navigation}

After publishing a custom schema, you can create a navigation entry in the Explorer to access your custom data:

1. Navigate to the **[!UICONTROL Explorer]** menu.
1. Select a folder where you want to place your custom schema, click the ellipsis icon, and click **[!UICONTROL Create new foler]**.
   ![Navigation entry creation for custom schema](assets/schemas-publish3.png)
1. Add a label and choose your schema in the **[!UICONTROL Folder type]** field.
   ![Navigation entry creation for custom schema](assets/schemas-publish5.png)
1. The custom schema will now be accessible from the **[!UICONTROL Explorer]** view.

![Navigation entry creation for custom schema](assets/schemas-navigation.png)

From the new folder, you can:

* View the list of records in your custom schema.
* Create new records.
* Edit and delete existing records.
* Customize which columns are displayed by default in the list view.

## Work with custom forms {#custom-forms}

Custom forms are data entry interfaces that are directly linked to schemas. Each custom form corresponds to a specific schema and allows you to view, create, edit, and delete records in that schema's data table directly from the interface. They provide a user-friendly way to manage data in custom tables without needing to use the client console.

>[!NOTE]
>
>A custom form is only available for schemas that have a form definition configured. The form definition is part of the schema configuration and defines which fields are displayed, how they are organized, and how users interact with the data. If a schema doesn't have a form definition, you can only view the schema details but cannot manage records through a form interface.

### Access custom forms {#access-forms}

To access a custom form:

1. Navigate to **[!UICONTROL Administration]** > **[!UICONTROL Schemas]**.
1. Apply the **[!UICONTROL Editable]** filter to view schemas that have form definitions configured.
1. Select a schema from the list.
1. In the Explorer view, you will see an entry for the custom schema that allows you to access the form interface.

![Custom form access in Explorer view](assets/schemas-form-access.png)

### Create and edit records {#create-edit}

From the custom form, you can:

* **Create new records**: Click the **[!UICONTROL Create]** button to add a new record to the custom schema.
* **Edit existing records**: Select a record from the list and click to open it in edit mode.
* **Delete records**: Use the delete action available in the record details.

![Custom form showing create and edit actions](assets/schemas-form-actions.png)

When editing records, linked fields are automatically populated based on the relationships defined in your schemas. For example, if a purchase is linked to a product, and the product is linked to a brand, the relationships are automatically maintained when you create or edit records.

>[!NOTE]
>
>Changes made to custom forms are immediately available. Unlike previous versions, you don't need to publish or refresh the interface to see your updates.

### Navigate with custom filters {#custom-filters}

You can apply custom filters to navigate and find specific records in your custom forms. Filters help you refine the list view to display only the records that match your criteria.

By default, filters are available in the filter panel. You can apply filters on any field to quickly find the records you need. For example, you can filter purchases by price, products by brand, or any other field in your schema.

![Custom form with filters applied](assets/schemas-form-filters.png)

### Default columns and list configuration {#default-columns}

When you access a custom form, the list view displays default columns based on the fields referenced in the form definition. These default columns are fixed, but you can add sections to organize the display further.

The default columns are automatically determined from the schema configuration. If you need to customize which columns appear or how they are organized, you can configure this in the screen definition for the schema.

### Custom form capabilities and limitations {#form-capabilities}

Custom forms provide a powerful way to manage data, with the following capabilities:

* **Layout configuration**: Forms support sections, separators, and field organization. By default, fields are displayed in two columns, but you can configure them to span a single column.
* **Visibility conditions**: You can set visibility conditions for fields and sections based on other field values.
* **Mandatory fields**: You can mark fields as mandatory to ensure data completeness.
* **Linked data**: Forms automatically handle relationships between schemas. For example, if you have a purchase linked to a product, and the product linked to a brand, these relationships are maintained automatically.
* **Collection lists**: You can display related data in collection lists within the form detail view.

>[!NOTE]
>
>Custom forms in the Web User Interface provide a streamlined experience compared to the client console. While they don't include all advanced features available in the client console form engine (such as complex variables and advanced scripting), they cover most common use cases and are much faster to configure and use. Changes are immediately available without requiring publication or refresh.
