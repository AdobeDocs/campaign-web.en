---
audience: end-user
title: Design a direct mail delivery
description: Learn how to design your direct mail delivery with Adobe Campaign Web
---

# Design a direct mail delivery {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Extraction file content"
>abstract="Click the **Edit content** button to start designing the extraction file required by your direct mail provider. This allows you to define the file properties such as its label and format, and to specify the columns that you want to include in the file."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="File properties"
>abstract="Configure the properties of the extraction file such as its name and format. You can personalize the file name using attributes from the database using the expression editor."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Content"
>abstract="In this section, specify the columns to display in the extraction file. Once done, you can get a preview of the extraction file using the **Simulate content** button."

To design the content of a direct mail delivery, click the **[!UICONTROL Edit content]** button from your delivery page then configure the extraction file properties and content.

The extraction file is required by direct mail providers to send mail to your customers.

![](assets/dm-content-details.png){zoomable="yes"}

## Configure the extraction file properties {#properties}

1. In the **[!UICONTROL File name]** field, specify the desired name for the extraction file.

    You can also personalize the file name using attributes from the database. To do this, click the **[!UICONTROL Open personalization dialog]** icon to open the expression editor. [Learn how to personalize your content](../personalization/personalize.md)

1. In the **[!UICONTROL File format]** field, choose the desired format for the extraction file; **Text**, **Text using fixed with columns**, **CSV (Excel)** or **XML**. 

    Available values depend on the selected format

    +++ Extraction format options
    
    * Use first line as column header (Text / CSV (Exce))
    * Column separator (Text)
    * String delimiter (Text)
    * End of line (Text)
    * Encoding
    * Date format and separators
    * Number format
    * Export labels instead of internal values of enumerations

    +++

1. **[!UICONTROL Requested quantity]** and Size limit.

## Define the extraction file content {#content}

In the **[!UICONTROL Content]** section, specify the columns to display in the extraction file. To do this, follow these steps:

1. Click the **[!UICONTROL Add Attribute]** button to create a new column.
1. Choose the attribute to display in the column then confirm.
1. The column is added to the extraction file content. You can change its label and modify the linked attribute using the edit icon.
1. Repeat these steps to add as many columns as needed for your extraction file. <!--Note that you can add up to xx columns.-->
1. To sort the extraction file using one of the columns, click the icon in the **[!UICONTROL Sorting]** column and select the desired sorting method.
1. To change the position of a column, use the up and down arrows.

![](assets/dm-content-attributes.png)

You can now preview and test your direct mail message and send it to your audience. [Learn how to test & send direct mail messages](send-direct-mail.md)