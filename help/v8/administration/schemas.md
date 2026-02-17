---
title: About schemas
description: Learn how to work with schemas.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
---
# About schemas {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Schemas"
>abstract="Adobe Campaign uses XML-based schemas to define the physical and logical structure of data within the application. From this screen, you can view all existing schemas, access schema details, configure custom forms, and create or extend schemas directly from the Web User Interface."

**[!DNL Adobe Campaign]** uses XML-based schemas to define the physical and logical structure of data within the application. A schema is an XML document linked to a database table that defines:

* The SQL table structure, including table name, fields, and relationships.
* The XML data structure, including elements, attributes, hierarchy, types, default values, and labels.

Schemas play a key role in:

* Mapping application data to database tables.
* Defining relationships between data objects.
* Specifying the structure and properties of each field.

Each entity in Adobe Campaign has a dedicated schema, ensuring data consistency and organization.

The schemas interface allows you to:

* [Access and customize schemas](schemas-browse-access.md) - View available schemas, explore their details and customize screen display
* [Configure list columns](schemas-list-columns.md) - Configure which columns are displayed by default in list views.
* [Edit custom fields](schemas-custom-fields.md) - Configure which custom fields are displayed in detail screens and organize them into sections.
* [Add collection lists](schemas-collection-lists.md) - Add collection lists to show related data in profile screens.
* [Create and manage schemas](schemas-create-publish.md#create-schemas) - Create new schemas and extend existing ones
* [Publish and synchronize schemas](schemas-create-publish.md#publish) - Synchronize schema changes with the database structure.
* [Work with custom forms](schemas-custom-forms.md) - Create, edit, and manage records in custom schemas using data entry forms.

>[!NOTE]
>
>You need to have administrator rights to manage schemas.

Detailed information on schemas is available in the [Campaign console documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.
