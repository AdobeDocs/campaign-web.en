---
title: Create and publish schemas
description: Learn how to create, extend, and publish schemas.
exl-id: 1da53fe0-1d64-4907-ba06-206f69e83d7c
---
# Create and publish schemas {#create-publish}

## Create and manage schemas {#create-schemas}

You can create new schemas, extend existing schemas, and access external databases.

### Create or extend a schema {#create-new}

To create or extend a schema:

1. Navigate to **[!UICONTROL Administration]** > **[!UICONTROL Schemas]**.
1. Click **[!UICONTROL Create schema]**.

   ![Schema creation dialog](assets/schemas-create1.png)

1. Enter a namespace for your schema (for example, `cus` for custom schemas).
1. Enter a unique name and label, and choose if you want to create a new schema or extend an existing one.

1. Click **[!UICONTROL Create]**.
   ![Schema creation dialog](assets/schemas-create2.png)

The schema is created and the generated schema structure is displayed. 

By default, the schema is empty. You now need to add the fields you want to include in your schema using the schema editor:

1. Click the pencil icon in the **[!UICONTROL Content]** section of the schema details screen.
2. Add the needed elements and save. Here is an example of a custom schema structure:

   ![Schema creation dialog](assets/schemas-create3.png)

The system automatically validates the XML structure and generates the schema.

### Define the screen edition {#define-attributes}

After creating the schema, you need to define the screen edition. 

For more information on the screen definition screen and how to access it, refer to the [Access the screen definition](schemas-browse-access.md#screen-def) section.

In our example, we simply add two custom fields:

1. Click the **[!UICONTROL Screen edition]** button in the schema details view to access the screen definition.

1. Click the ellipsis icon above the **[!UICONTROL List of custom fields]** table and choose **[!UICONTROL Select attributes]**.
1. Select the custom fields you want to add and confirm.

   ![Schema creation dialog](assets/schemas-create4.png)

## Publish and synchronize schemas {#publish}

After creating or modifying a schema, you need to publish it to synchronize the logical schema with the physical database structure.

### Publish schema changes {#publish-changes}

>[!CAUTION]
>
>Publishing schema changes modifies the database structure. Make sure you understand the impact of these changes before confirming the publication.

To publish your schema changes:

1. Navigate to **[!UICONTROL Administration]** > **[!UICONTROL Schemas]** to access the schema list.
1. Click **[!UICONTROL Publishing]** and confirm.

   ![Schema publication dialog showing changes to be applied](assets/schemas-publish1.png)

1. Select, in the list, the schema you want to synchronize.

   ![Schema publication dialog showing changes to be applied](assets/schemas-publish2.png)

1. Review the SQL script that will be executed to update the database structure.
1. Click **[!UICONTROL Publish]** and confirm to proceed with the publication.

>[!NOTE]
>
>The process may take some time depending on the size of your database and the complexity of the changes.

### Create a navigation entry {#navigation}

After publishing a custom schema, you can create a navigation entry in the Explorer to access your custom data:

1. Navigate to the **[!UICONTROL Explorer]** menu and select a folder where you want to place your custom schema.
1. Click the ellipsis icon, and click **[!UICONTROL Create new folder]**.
   ![Navigation entry creation for custom schema](assets/schemas-publish3.png)
1. Add a label and choose your schema in the **[!UICONTROL Folder type]** field.
   ![Navigation entry creation for custom schema](assets/schemas-publish5.png)
1. The custom schema will now be accessible from the **[!UICONTROL Explorer]** view.

From the new folder, you can:

* View the list of records in your custom schema.
* Create new records.
* Edit and delete existing records.
* Customize which columns are displayed by default in the list view.
