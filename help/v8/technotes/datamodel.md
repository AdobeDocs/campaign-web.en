---
title: Technote - Campaign datamodel
description: Work with Campaign datamodel 
---
# Work with Campaign datamodel{#campaign-datamodel}

## Get started with Campaign data model{#gs-datamodel}

Adobe Campaign comes with a pre-defined data model. This section gives some details on the built-in tables of the Adobe Campaign data model and their interaction. Adobe Campaign relies on a Cloud database containing tables that are linked together.

The basic structure of the Adobe Campaign data model can be described as follows:

* **Recipient table**: The datamodel relies on a main table which is by default the Recipient table (**nmsRecipient**). This table stores all the marketing profiles. Learn more about the recipient table in [this section](datamodel-tables.md#recipients-table).

* **Delivery table**: This table stores one record per delivery action. Learn more about the delivery table in [this section](datamodel-tables.md#delivery-table).

* **Log tables**: These tables store all the logs associated with the execution of the campaigns, and deliveries. Learn more about the log tables in [this section](datamodel-tables.md#log-tables).

* **Technical tables**: Gather technical data used for the applicative process. Learn more about the technical tables in [this section](datamodel-tables.md#technical-tables).


>[!NOTE]
>
> Key tables of Campaign datamodel are listed in [this page](datamodel-tables.md).


## Browse Campaign datamodel {#browse-datamodel}

### Schemas and tables {#tables-and-schemas}

The physical and logical structure of the data carried in the application is described in XML. It obeys a grammar specific to Adobe Campaign, called a **schema**. A schema is an XML document associated with a database table. It defines data structure and describes the SQL definition of the table: the name of the table, fields, links with other tables.

It also describes the XML structure used to store data: elements and attributes, their types, hierarchy of elements, default values, labels, descriptions, and other properties.

Adobe Campaign relies on data schemas to:

* Define how data object within the application are tied to underlying database tables.
* Define links between the different data objects within the Campaign application.
* Define and describe the individual fields included in each object.

You can browse Campaign schemas from the **Explorer** view. To access the list of schemas, browse to **Administration > Configuration > Data schemas**.

![](assets/data-schemas.png)

From Campaign client console, you can access the description of each table. Browse to **Administration > Configuration > Data schemas**, select a resource from the list, and click the **Documentation** tab.

### Syntax of schemas {#syntax-of-schemas}

The root element of the schema is **`<srcschema>`**. It contains the **`<element>`** and **`<attribute>`** sub-elements.

The first **`<element>`** sub-element coincides with the root of the entity.

```
<srcSchema name="recipient" namespace="cus">
  <element name="recipient">  
    <attribute name="lastName"/>
    <attribute name="email"/>
    <element name="location">
      <attribute name="city"/>
   </element>
  </element>
</srcSchema>
```

>[!NOTE]
>
>The root element of the entity has the same name as the schema.

### Schema identification {#identification-of-a-schema}

A data schema is identified by its name and its namespace.

A namespace lets you group a set of schemas by area of interest. For example, the **cus** namespace is used for customer-specific configuration (**customers**).

### Create and extend schemas {#create-or-extend-schemas}

To add a field or other element to one of the core data schemas in Campaign, such as the recipient table (nms:recipient), you have to extend that schema. 

To add an entirely new type of data that does not exist in Adobe Campaign (a table of contracts for example) you can create a custom schema directly. 

These actions can only be performed by expert users from Campaign client console.

### Browse links and attributes {#links-and-attributes}

When using the rule builder, you can browse Campaign data model and query the database, to retrieve the exact data you need. You can filter and preview any data associated to the current targeting dimension. All of the data types are defined by schemas, and each schema is implemented by a table in the database.

In the rule builder, you can expand the links of the table you are working on. These links connect the current table to other tables, and helps you understand the relationships between tables in the database. Once these links and tables are expanded, you can view the attributes you can use to create your filtering conditions, and save them as rules. In addition, you can also preview the data that is retrieved, and check your filtering rules.


For example, when creating a filtering rule on the recipient table (**nmsRecipient**), you can see the links to the other tables. The cardinality between the links can be unique (1:1), or multiple (1:N). The link cardinality type is represented by a specific icon.

>[!NOTE]
>
>To view linked tables, you must activate the **Display advanced attributes** toggle.


For example there is a single Folder for each recipient - 1:1 cardinality -, but a recipient can be included in multiple lists - 1:N cardinality.

![](assets/edit-rule-links.png)

In the main table, and in each linked table, you can select the attributes to use to design your filtering rules. Learn steps to define a rule with the rule builder in [this section](../audience/create-audience.md).