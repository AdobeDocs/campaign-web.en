---
audience: end-user
title: Filter lists
description: Learn how to filters Adobe Campaign Web lists using built-in and custom filters.
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
---
# Filter lists {#filter-lists}

Adobe Campaign Web provides filters within each list of objects, enabling you to filter information based on specific contextual criteria. For example, you can filter deliveries based on their status, channel, contact date, or folder. You can also hide proofs.

## Apply filters {#apply}

To apply filters to a list, click the **[!UICONTROL Show filters]** button located in the upper-left corner of the list, next to the search bar.

The filters pane opens, displaying available filters for the selected list. For example, you can filter campaigns based on their status, start and end dates, or storage folder, while the subscription services list can be filtered based on their channel and storage folder.

![Filters pane showing available filters for lists](assets/filters-pane.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

To filter a list based on your own criteria, create a custom filter. To do this, browse to the bottom of the filters pane and click the **Add rules** button. [Learn how to create custom filters](#custom).

Once applied to a list, filters are visible below the search bar. You can remove an individual filter at any time, or remove all filters by clicking the **Clear all** button.

## Create custom filters {#custom}

Custom filters allow you to refine lists based on your own specific criteria. They are designed using the Campaign query modeler. To create a custom filter, follow these steps:

1. Open the filters pane, and click the **Add rules** button located at the bottom of the pane.

1. The query modeler opens. Define and combine your filter criteria to suit your needs. Detailed information on how to use the query modeler is available in [this section](../query/query-modeler-overview.md).

    The example below shows a custom filter designed to display in the campaigns list SMS campaigns run by operators from the Running or Yoga departments.

    ![Custom filter example showing SMS campaigns filtered by department](assets/filters-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. Once your custom filter is configured, click **[!UICONTROL Confirm]** to apply it to the list.