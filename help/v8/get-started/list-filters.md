---
audience: end-user
title: Browse, search and filter lists
description: Discover how to browse and filter lists Campaign Web v8
badge: label="Beta"
exl-id: 46b83e8c-6c8c-40a1-a08b-9d0b438b80cb
---
# Browse, search, and filter lists {#list-screens}

Most of the links from the left navigation menu display lists of objects, such as the list of **Deliveries** or **Campaigns**. Some of these list screens are read-only. You can customize the list display, and filter these lists, as detailed below.

To remove a filter, click the **Clear all** button.

## Customize list screens {#custom-lists}

The lists are displayed in columns. You can display additional information by changing the column configuration. To do this, click the **Configure column for a custom layout** icon in the top right corner of the list. 

![](assets/config-columns.png){width="70%" align="left" zoomable="yes"}

In the **Configure columns** screen, add or remove columns, and change the order in which they are displayed.

For example, for these settings:

![](assets/columns.png){width="70%" align="left" zoomable="yes"}

The list shows the following columns:

![](assets/column-sample.png){width="70%" align="left" zoomable="yes"}

Use the **Display advanced attributes** toggle to see all attributes for the current list. [Learn more](#adv-attributes)

## Sort data {#sort-lists}

You can also sort items in the list by clicking any column header. An arrow is displayed (Up or Down) indicating that the list is sorted on that column. 

For numeric or date columns, the **Up** arrow indicates that the list is sorted in ascending order while the **Down** arrow indicates a descending order. For string or alphanumeric columns, values are listed in alphabetical order.

## Built-in filters {#list-built-in-filters}

To find items quicker, you can use the search bar, or filter the list based on contextual criteria. 

![](assets/filter.png){width="70%" align="left" zoomable="yes"}

For example, you can filter deliveries on their status, channel, contact date, or folder. You can also hide tests.

## Custom filters{#list-custom-filters}

To create custom filters on data, browse to the bottom of the filters and click the **Add rules** button to access the rule builder.

Drag and drop attributes to build your filter criteria in the **Advanced filters** screen. 

![](assets/custom-filter.png){width="70%" align="left" zoomable="yes"}

Use the **Display advanced attributes** toggle to see all attributes for the current list. [Learn more](#adv-attributes)

The rule builder's operating principle for custom filters is similar to the rule builder used to create audiences. Detailed information on how to use it is available in the [Audiences documentation](../audience/segment-builder.md).

## Use advanced attributes {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Display advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Rule builder advanced fields"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Rule builder advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."


Only most common attributes are displayed by default in the attribute list and filter configuration screens. Attributes which were set as `advanced` attributes in the data schema are hidden from the configuration screens. 

Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links. The attribute list is updated instantly.


![](assets/adv-toggle.png){width="70%" align="left" zoomable="yes"}
