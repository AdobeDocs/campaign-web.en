---
title: About schemas
description: Learn how to work with schemas.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
TQID: https://experienceleague.adobe.com/D7gEyOdvyADCac9T3By3KKnx7kpN8LuE2-rnRBJDyMA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: b82389f8-9b5e-4083-8e3b-3cef299fb8b9
    internal-label: Schemas
subfeature_v2:
  - id: cfc95e9b-b035-4403-a6a9-b27a8a053a37
    internal-label: PI
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# About schemas {#schemas}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Schema authoring"
>abstract="You can now create and manage schemas directly from the Campaign Web User Interface. You can create new tables, extend existing schemas and create custom forms."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"

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
