---
audience: end-user
title: Build your first query using the query modeler
description: Learn how to build your first query in Adobe Campaign Web query modeler.
exl-id: efd762b5-a7ae-49b4-ab74-5b43da1e574d
---
The content has been formatted according to the specified rules. Below is the updated documentation:

---

# Build your first query {#build-query}

To start building a query, access the query modeler from the location of your choice, depending on the action you want to perform. The query modeler opens with a blank canvas. Click the **+** button to configure the first node of your query.

You can add two types of elements:

* **Filtering components** (Custom condition, Select audience, Predefined filter) allow you to build your own rules, select an audience, or use a predefined filter to refine your query. They are added at the start of your query and on dotted transitions. [Learn how to work with filtering components](#filtering)

    Example: *Recipients who subscribed to the 'Sports' newsletter*, *Recipients living in New York*, *Recipients living in San Francisco*

    ![Description: Example of adding filtering components to a query.](assets/query-add-component.png){zoomable="yes"}

* **Group operators** (AND, OR, EXCEPT) allow you to group filtering components in the diagram. They are added on existing transitions before a filtering component. [Learn how to work with operators](#filtering)

    Example: *Recipients who subscribed to the "Sports" newsletter **AND** who live in New York **OR** San Francisco*.

    ![Description: Example of adding group operators to a query.](assets/query-add-operator.png){zoomable="yes"}

## Distribution of values in a query {#distribution-values-query}

The distribution of values shows the percentage of each value of a field within a table, based on the current query parameters. Knowing the distribution of values within a query helps refine segmentation.

To access this option, in your query, click the attribute selection button as shown below. Then, click on the **[!UICONTROL Information]** icon next to the selected attribute. You can access the **[!UICONTROL Distribution of values]** button.

![Description: Accessing the distribution of values option in a query.](assets/values_query.png){zoomable="yes"}

>[!NOTE]
>
>* For fields with many values, only the first twenty values are displayed. In such cases, a notification **[!UICONTROL Partial load]** warns you.
>* The **[!UICONTROL Distribution of values]** option is accessible in every attribute picker. [Learn how to select attributes](../get-started/attributes.md)
>* You can add conditions on the results by using the **[!Advanced filters]**. [Learn more here](../get-started/work-with-folders.md#filter-the-values).

## Add filtering components {#filtering}

Filtering components allow you to refine your query by using:

* **[Custom conditions](#custom-condition)**: Filter your query by building your own condition with attributes from the database and advanced expressions.
* **[Audiences](#audiences)**: Filter your query using an existing audience.
* **[Predefined filter](#predefined-filters)**: Filter your query using existing predefined filters.

### Configure a custom condition {#custom-condition}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Custom condition"
>abstract="Custom conditions are filtering components that allow you to filter your query by building your own condition with attributes from the database and advanced expressions."

To filter your query using a custom condition, follow these steps:

1. Click the **+** button on the desired node and select **[!UICONTROL Custom condition]**. The custom condition properties pane opens on the right-hand side.

1. In the **Attribute** field, select the attribute from the database that you want to use to create your condition. The attributes list includes all the attributes from your campaign database, including attributes from linked tables. [Learn how to select attributes and add them to favorites](../get-started/attributes.md)

    ![Description: Selecting attributes for a custom condition in a query.](assets/query-custom-condition-fields.png){zoomable="yes"}

    >[!NOTE]
    >
    >The **Edit expression** button allows you to use the Campaign Web expression editor to manually define an expression using fields from the database and helper functions. [Learn how to edit expressions](expression-editor.md)

1. Select the operator to apply from the drop-down list. Various operators are available for use. Note that operators available in the drop-down list depend on the attribute's data type.

   +++List of available operators

    |Operator|Purpose|Example|
    |---|---|---|
    |Equal to|Returns a result identical to the data entered in the second Value column.|Last name (@lastName) equal to 'Jones' will return only recipients whose last name is Jones.|
    |Not equal to|Returns all values not identical to the value entered.|Language (@language) not equal to 'English'.|
    |Greater than|Returns a value greater than the value entered.|Age (@age) greater than 50 will return all values greater than '50', such as '51', '52'.|
    |Less than|Returns a value smaller than the value entered.|Creation date (@created) before 'DaysAgo(100)' will return all recipients created less than 100 days ago.|
    |Greater than or equal to|Returns all values equal to or greater than the value entered.|Age (@age) greater than or equal to '30' will return all recipients aged 30 or more.|
    |Less than or equal to|Returns all values equal to or lower than the value entered.|Age (@age) less than or equal to '60' will return all recipients aged 60 or less.|
    |Included in|Returns results included in the values indicated. These values must be separated by a comma.|Birth date (@birthDate) is included in '12/10/1979,12/10/1984' will return the recipients born between these dates.|
    |Not in|Works like the Is included in operator. Here, recipients are excluded based on the values entered.|Birth date (@birthDate) is not included in '12/10/1979,12/10/1984'. Recipients born within these dates will not be returned.|
    |Is empty|Returns results matching an empty value in the second Value column.|Mobile (@mobilePhone) is empty returns all recipients who do not have a mobile number.|
    |Is not empty|Works in reverse to the Is empty operator. It is not necessary to enter data in the second Value column.|Email (@email) is not empty.|
    |Starts with|Returns results starting with the value entered.|Account # (@account) starts with '32010'.|
    |Does not start with|Returns results not starting with the value entered.|Account # (@account) does not start with '20'.|
    |Contains|Returns results containing at least the value entered.|Email domain (@domain) contains 'mail' will return all domain names that contain 'mail', such as 'gmail.com'.|
    |Does not contain|Returns results not containing the value entered.|Email domain (@domain) does not contain 'vo'. Domain names containing 'vo', such as 'voila.fr', will not appear in the results.|
    |Like|Similar to the Contains operator, it lets you insert a % wildcard character in the value.|Last name (@lastName) like 'Jon%s'. The wildcard character acts as a "joker" to find names like "Jones".|
    |Not like|Similar to the Contains operator, it lets you insert a % wildcard character in the value.|Last name (@lastName) not like 'Smi%h'. Recipients whose last name is 'Smith' will not be returned.|

    +++

1. In the **Value** field, define the expected value. You can also use the Campaign Web expression editor to manually define an expression using fields from the database and helper functions. To do this, click the **Edit expression** button. [Learn how to edit expressions](expression-editor.md)

    *Query example returning all profiles aged 21 or more:*

    ![Description: Example of a query targeting profiles aged 21 or more.](assets/query-custom-condition.png){zoomable="yes"}

    For date-type attributes, predefined values are available using the **[!UICONTROL Presets]** option.

    ![Description: Example of using date presets in a query.](assets/date-presets.png){zoomable="yes"}

---

The formatting rules have been applied consistently throughout the document. Let me know if further adjustments are needed!