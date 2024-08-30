---
audience: end-user
title: Distribution of values
description: Learn how to query the database to see the distribution of values
---
# Distribution of values {#distribution-values}

The distribution of values helps to know the percentage of a value in a column within a table. It is available for columns composed of sequels or expressions.

## Distribution of values in a folder {#distribution-values-folder}

To know the distribution of values in a folder, proceed as below :

For example, among the deliveries, we want to know the distribution of values of the **Channel** column.

To get this information, go to the **[!UICONTROL Deliveries]** folder and click on **[!UICONTROL Configure columns]** icon.

In the **[!UICONTROL Configure columns]** window, click on the **[!UICONTROL Information]** icon of the column you want to know. Then, click on the **[!UICONTROL Distribution of values]** button.

![](assets/values_deliveries.png){zoomable="yes"}

You will get the percentage of the values in the **[!UICONTROL Channel]** column.

![](assets/values_percentage.png){zoomable="yes"}

>[!NOTE]
>
> For columns with many values, only the first twenty values will be displayed. A notification **[!UICONTROL Partial load]** will warn you.

You can also have the distribution of values of a link. 

In the attributes list, click the **+** button next to the desired link, as shown below. This adds the link to the **[!UICONTROL Output columns]**. You can have now the **[!UICONTROL Information]** icon, allowing you to view the distribution of its values. If you do not want to keep the link in the **[!UICONTROL Output columns]**, make sure to click on the **[!UICONTROL Cancel]** button.

![](assets/values_link.png){zoomable="yes"}

## Distribution of values in a query {#distribution-values-query}

If you are in a workflow, knowing the distribution of values within a query can assist you in refining your segmentation. 

To access the feature, in your query, click the attribute selection button as shown below. Then, click on the **[!UICONTROL Information]** icon next to the selected attribute. You can have access there to the **[!UICONTROL Distribution of values]** button.

![](assets/values_query.png){zoomable="yes"}

>[!NOTE]
>
> The **[!UICONTROL Distribution of values]** feature is accessible in every attribute picker.
