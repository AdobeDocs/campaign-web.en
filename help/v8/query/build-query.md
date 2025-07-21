---
audience: end-user
title: Build your first query using the query modeler
description: Learn how to build your first query in Adobe Campaign Web query modeler.
exl-id: efd762b5-a7ae-49b4-ab74-5b43da1e574d
---

# Build your first query {#build-query}

To start building a query, access the query modeler from the location of your choice, depending on the action you want to perform. The query modeler opens with a blank canvas. Click the **+** button to configure the first node of your query.

>[!IMPORTANT]
>
>A brand new interface for the Query modeler is available. The New rule builder allows you to build your query with more ease thanks to its simplified interface. To switch to this experience, press the toggle button in the top-right corner. You can go back to the classic Query modeler anytime you want by simply pressing the toggle back to disable the new interface. You can apply the same principles as the query modeler in this new interface.
>![Image showing the toggle for the new rule builder interface](assets/query-modeler-toggle.png){zoomable="yes"} 

You can add two types of elements:

* **Filtering components** (Custom condition, Select audience, Predefined filter) allow you to build your own rules, select an audience, or use a predefined filter to refine your query. They are added at the start of your query and on dotted transitions. [Learn how to work with filtering components](#filtering)

    Example: *Recipients who subscribed to the 'Sports' newsletter*, *Recipients living in New York*, *Recipients living in San Francisco*

>[!BEGINTABS]

>[!TAB Classic query modeler]

![Example of adding filtering components to a query.](assets/query-add-component.png){zoomable="yes"}


>[!TAB New Rule builder]

![Example of adding filtering components to a query.](assets/ruleb-1.png){zoomable="yes"}

>[!ENDTABS]



* **Group operators** (AND, OR, EXCEPT) allow you to group filtering components in the diagram. They are added on existing transitions before a filtering component. [Learn how to work with operators](#filtering)

    Example: *Recipients who are Super VIP **AND** VIP to reward **OR** VIP Demo, **EXCEPT** recipients under 21 years old and above 45.

>[!BEGINTABS]

>[!TAB Classic query modeler]

![Description: Example of adding group operators to a query.](assets/ruleb-13.png){zoomable="yes"}

>[!TAB New rule builder]

![Example of adding filtering components to a query.](assets/ruleb-14.png){zoomable="yes"}

>[!ENDTABS]


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

    ![Selecting attributes for a custom condition in a query.](assets/query-custom-condition-fields.png){zoomable="yes"}

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

>[!BEGINTABS]

>[!TAB Classic query modeler]

![Example of a query targeting profiles aged 21 or more.](assets/query-custom-condition.png){zoomable="yes"}

>[!TAB New rule builder]

![Example of a query targeting profiles aged 21 or more.](assets/ruleb-3.png){zoomable="yes"}

>[!ENDTABS]

For date-type attributes, predefined values are available using the **[!UICONTROL Presets]** option.

>[!BEGINTABS]

>[!TAB Classic query modeler]

![Example of using date presets in a query.](assets/date-presets.png){zoomable="yes"}

>[!TAB New rule builder]

![Example of using date presets in a query.](assets/ruleb-4.png){zoomable="yes"}

>[!ENDTABS]

#### Custom conditions on linked tables (1-1 and 1-N links){#links}

Custom conditions allows you to query tables linked to the table currently used by your rule. This includes tables with a 1-1 cardinality link, or collection tables (1-N link).

For a **1-1 link**, navigate to the linked table, select the desired attribute and define the expected value.

You can also directly select a table link in the **Value** picker and confirm. In that case, values available for the selected table need to be selected using a dedicated picker, as shown in the example below.

+++Query example

Here, the query is targeting brands whose label is "running". 

1. Navigate inside the **Brand** table and select the **Label** attribute.

    ![Screenshot of the Brand table](assets/1-1-attribute.png){zoomable="yes"}{width="85%" align="center"}

1. Define the expected value for the attribute.

    ![Example of a defined expected value](assets/1-1-table.png){zoomable="yes"}{width="85%" align="center"}

Here is a query sample where a table link has been selected directly. Available values for this table must be selected from a dedicated picker.

![Example of a query sample](assets/1-1-table-direct.png){zoomable="yes"}{width="85%" align="center"}

+++ 

For a **1-N link**, you can define sub-conditions to refine your query, as shown in the example below.

+++Query example

Here, the query is targeting recipients who made purchases related to the BrewMaster product, for a total amount of at least 100$.

1. Select the **Purchases** table and confirm.

    ![Screenshot of the Purchase table](assets/1-N-collection.png){zoomable="yes"}{width="50%" align="center"}

1. An outbound transition is added, allowing you to create sub-conditions.

    ![Example of an outbound transition](assets/1-n-subcondition.png){zoomable="yes"}{width="85%" align="center"}

1. Select the **Price** attribute and target purchases of 1000$ or more

    ![Screenshot of the Price attribute](assets/1-n-price.png){zoomable="yes"}{width="85%" align="center"}

1. Add sub-conditions to suit your needs. Here we have added a condition to target profiles who purchased a BrewMaster product.

    ![Example of sub-conditions](assets/custom-condition-1-N.png){zoomable="yes"}{width="85%" align="center"}

+++ 

#### Work with aggregate data {#aggregate}

Custom conditions allow you to perform aggregate operations. To do this, you need to directly select an attribute from a collection table:

1. Navigate inside the desired collection table and select the attribute on which you want to perform an aggregate operation.

    ![Screenshot of the attribute list](assets/aggregate-attribute.png){zoomable="yes"}{width="85%" align="center"}

1. In the properties pane, toggle on the **Aggregate data** option and select the desired aggregate function.

>[!BEGINTABS]

>[!TAB Classic query modeler]

![Screenshot of the Aggregate data option](assets/aggregate.png){zoomable="yes"}{width="85%" align="center"}

>[!TAB New rule builder]

![Screenshot of the Aggregate data option](assets/ruleb-5.png){zoomable="yes"}{width="85%" align="center"}

>[!ENDTABS]

### Select an audience {#audiences}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Select audience"
>abstract="By using the **Select audience** option, you can choose the audience that you want to use to filter your query."

To filter your query using an existing audience, follow these steps:

>[!BEGINTABS]

>[!TAB Classic query modeler]

1. Click the **+** button on the desired node and choose **[!UICONTROL Select audience]**.

1. The **Select audience** properties pane opens on the right hand side. Choose the audience that you want to use to filter your query.

    *Query example returning all profiles belonging to the "Festival Goers" audience":*

    ![Screenshof of a query example](assets/query-audience.png){zoomable="yes"}

>[!TAB New rule builder]

1. Click the **Expand** button next to the **[!UICONTROL Add condition]** button and choose **[!UICONTROL Select audience]**.

1. The **Select audience** properties pane opens on the right hand side. Choose the audience that you want to use to filter your query.

    *Query example returning all profiles belonging to the "Coffee Works" audience":*

    ![Screenshof of a query example](assets/ruleb-7.png){zoomable="yes"}

>[!ENDTABS]

### Use a predefined filter {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Predefined filter"
>abstract="By using the **Predefined filter** option, you can select a predefined filter from the list of custom filters or from favorites."

To filter your query using a predefined filter, follow these steps:

>[!BEGINTABS]

>[!TAB Classic query modeler]

1. Click the **+** button on the desired node and select **[!UICONTROL Predefined filter]**.

1. The **Predefined filter** properties pane opens on the right hand side. Select a predefined filter from the list of custom filters or from favorites.

    *Query example returning all profiles corresponding to the "Inactive customers" predefined filter:*

    ![Screenshot of a query example](assets/query-predefined-filter.png){zoomable="yes"}

>[!TAB New rule builder]

1. Click the **Expand** button next to the **[!UICONTROL Add condition]** button and select **[!UICONTROL Predefined filter]**.

1. The **Predefined filter** properties pane opens on the right hand side. Select a predefined filter from the list of custom filters or from favorites.

    *Query example returning all profiles corresponding to the "Inactive customers" predefined filter:*

    ![Screenshot of a query example](assets/ruleb-8.png){zoomable="yes"}

>[!ENDTABS]

### Copy-paste components {#copy}

The query modeler allows you to copy one or multiple filtering components and paste them at the end of a transition. This operation can be executed within the current query canvas, or in any canvas within your instance.

>[!NOTE]
>
>The copied selection is kept as long as you are working in your instance. If you log off and log back in, your selection will no longer be available for pasting.

>[!IMPORTANT]
>
>It is currently impossible to copy and paste components in the New Rule builder experience. To follow these next steps, please click the **[!UICONTROL Get back to the classic experience]** toggle at the top to use the Classic Query modeler.


To copy-paste filtering components, follow these steps:

1. Select the filtering component that you want to copy by clicking on it in the query canvas. To select multiple components, use the multiple selection tool available in the toolbar located at the upper-right corner of the canvas.

1. Click the **[!UICONTROL Copy]** button in the component's properties pane or in the blue ribbon at the bottom of the screen if you have selected multiple components.

    |Copy a single component|Copy multiple components|
    |  ---  |  ---  |
    |![](assets/copy-single-component.png){zoomable="yes"}{width="200" align="center" zoomable="yes"}|![](assets/copy-multiple-components.png){zoomable="yes"}{width="200" align="center" zoomable="yes"}|

1. To paste the component(s), click the + button at the end of the desired transition and select **Paste n items**.

    ![Example of pasting the components](assets/copy-paste.png){zoomable="yes"}

## Drag and drop components {#drag-and-drop}

>[!IMPORTANT]
>
>This feature is only available for the new rule builder experience. 

When you are adding components to your query, you can move them up and down using the drag and drop feature.

To the left of every component, you can click on the dots and hold them to drag the component up and down depending on where you want to put and group the components.

![Gif showing how to drag and drop the components in the new rule builder](assets/ruleb-drag.gif){zoomable="yes"}

## Combine filtering components with operators {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Group"
>abstract="In this pane, you can change the operator used to link filtering conditions together."

Each time you add a new filtering component to your query, it is automatically linked to the other component by an **AND** operator. This means that results from the two filtering components are combined.

In this example, we have added a new audience-type filtering components on the second transition. The component is linked to the predefined filter condition with an **AND** operator, meaning that the query results include recipients targeted by the "Newsletter Subscribers - MADRID" predefined filter AND belonging to the "Purchasers (All time)" audience.

>[!BEGINTABS]

>[!TAB Classic query modeler]

![Example of a query](assets/query-operator.png){zoomable="yes"}

To change the operator used to link filtering conditions together, click on it and select the desired operator in the **Group** pane that opens on the right hand side.

Available operators are:

* **AND (Intersection)**: Combines results matching all the filtering components in the outbound transitions. 
* **OR (Union)**: Includes results matching at least one of the filtering components in the outbound transitions.
* **EXCEPT (Exclusion)**: Excludes results matching all the filtering componentns in the outbound transition. 

![Example of a query](assets/query-operator-change.png){zoomable="yes"}

In addition, you can create intermediate groups of components by grouping components into a same group and linking them together. That way, the AND operator will be put by default, you can then change it to the desired operator.

>[!TAB New rule builder]

![Example of a query](assets/ruleb-9.png){zoomable="yes"}

To change the operator used to link filtering conditions together, click on it, it will change to OR, EXCEPT and then back to AND, and select the desired operator.

Available operators are:

* **AND (Intersection)**: Combines results matching all the filtering components in the outbound transitions. 
* **OR (Union)**: Includes results matching at least one of the filtering components in the outbound transitions.
* **EXCEPT (Exclusion)**: Excludes results matching all the filtering componentns in the outbound transition.

![Example of a query](assets/ruleb-10.gif){zoomable="yes"}

>[!ENDTABS]

In the example below, we have created an intermediate group to include results from either the "VIP to reward" or "Super VIP" audiences.

>[!BEGINTABS]

>[!TAB Classic query modeler]

![Example of a query](assets/query-intermediate-group.png){zoomable="yes"}

>[!TAB New rule builder]

![Example of a query in the new rule builder](assets/ruleb-11.png){zoomable="yes"}

>[!ENDTABS]

## Check and validate your query

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Rule properties"
>abstract="Once you've built your query in the canvas, you can check it using the **Rule properties** pane located on the right hand side.<br/>This pane allows you to display the resulting data, to retrieve an SQL code version of the query, and check the number of targeted records.<br/>Use the **Select or save filter** button to save your query as a predefined filter, or replace the canvas content with an existing filter."

Once you've built your query in the canvas, you can check it using the **Rule properties** pane located on the right hand side  This pane displays when building a query to create an audience. Available operations are:

* **View results:** Displays the data resulting from your query. You can also view results on each condition and group in the rule builder. First calculate the target population, then click on the result number to view the results.
* **Code view**: Displays a code-based version of the query in SQL. 
* **Calculate**: Updates and displays the number of records targeted by your query. You can also calculate the target population on each condition and group in the rule builder. You can click on the result number to view the results.
* **Select or save filter**: Choose an existing predefined filter to use in the canvas, or save your query as a predefined filter for future reuse. [Learn how to work with predefined filters](../get-started/predefined-filters.md)

    >[!IMPORTANT]
    >
    >Select a predefined filter from the Rule properties pane replaces the query that has been built in the canvas with the selected filter.

When your query is ready, click the **[!UICONTROL Confirm]** button in the upper-right corner to save it.


>[!BEGINTABS]

>[!TAB Classic query modeler]

You can modify your query at any time by opening it. Keep in mind that upon opening an existing query, it displays in a simplified view without the visiblity of  **+** buttons. To add new elements to the query, select a component or operator on the canvas to display the **+** buttons.

![Example of a query](assets/edit-audience.png){zoomable="yes"}

>[!TAB New Rule builder]

You can modify your query at any time by opening it, to do that, click on the **[!UICONTROL Add condition]** button on the top-left corner.

![Example of a query in the new rule builder](assets/ruleb-11.png){zoomable="yes"}

>[!ENDTABS]
