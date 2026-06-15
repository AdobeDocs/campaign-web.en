---
audience: end-user
title: Browse and filter lists
description: Discover how to browse and filter lists Campaign Web v8
exl-id: 46b83e8c-6c8c-40a1-a08b-9d0b438b80cb
TQID: https://experienceleague.adobe.com/GKGmvMJtlQgAftvZuOb33tQSgqHC9s8qlYJMVFnWjz0
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
---
# Browse and filter lists {#list-screens}

Most links from the left navigation menu display lists of objects, such as the list of **Deliveries** or **Campaigns**. Some of these list screens are read-only. You can customize the list display, filter these lists, and export list data as CSV files, as detailed below.

## Customize list screens {#custom-lists}

The lists are displayed in columns. You can display additional information by changing the column configuration. To do this, click the **Configure column for a custom layout** icon in the top right corner of the list.

![The screenshot shows the Configure column icon used to customize the layout of list columns.](assets/config-columns.png){zoomable="yes"}{width="70%"}

In the **Configure columns** screen, add or remove columns, and change the order in which they are displayed.

You can change the order of your list either by **drag and drop**, or by using **up and down arrows** as shown below:

![The screenshot demonstrates how to reorder list columns using drag-and-drop or arrow buttons.](assets/list-reorder.png){zoomable="yes"}{width="70%"}

For example, for these settings:

![The screenshot displays an example of column settings in the Configure columns screen.](assets/columns.png){zoomable="yes"}{width="70%" zoomable="yes"}

The list shows the following columns:

![The screenshot shows the resulting list with columns configured as per the example settings.](assets/column-sample.png){zoomable="yes"}{width="70%"}

## Sort data {#sort-lists}

You can sort items in the list by clicking any column header. An arrow is displayed (Up or Down), indicating that the list is sorted on that column.

For numeric or date columns, the **Up** arrow indicates that the list is sorted in ascending order, while the **Down** arrow indicates a descending order. For string or alphanumeric columns, values are listed in alphabetical order.

## Filters {#list-built-in-filters}

To find items quicker, use the search bar or built-in and custom filters to adapt the list based on contextual criteria. 

![The screenshot shows the filter options available for refining the list view.](assets/filter.png){zoomable="yes"}{width="70%"}

Detailed information on how to use filters and create your own custom filters is available in [this section](../query/filter.md).

## Export list data {#export-list}

You can export data from any list screen including tracking logs. To export a list, follow these steps:

1. Open the list you want to export.
1. Adjust the displayed columns and apply any search or filters. The export takes into account the columns displayed on screen and any active search or filters.
1. Scroll down to load more rows if needed. Only the rows currently loaded in the list are exported.
1. Click the **Export loaded rows as CSV** button above the list. The file is saved to your browser's default download folder.

![The screenshot shows the export of a list.](assets/filter-export.png){zoomable="yes"}


<!--
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

Only the most common attributes are displayed by default in the attribute list and filter configuration screens. Attributes set as `advanced` attributes in the data schema are hidden from the configuration screens.

Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links. The attribute list updates instantly.

[The screenshot shows the Display advanced attributes toggle used to reveal hidden attributes in the rule builder palette.](assets/adv-toggle.png){zoomable="yes"}{width="70%" zoomable="yes"}
-->