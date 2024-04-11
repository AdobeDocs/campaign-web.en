---
audience: end-user
title: Use the Extract file workflow activity
description: Learn how to use the Extract file workflow activity
---
# Extract file {#extract-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="Extract file"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="File to extract"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="Destination format"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="Post processing"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="Outbound transition"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="Process error"
>abstract="TBC"

The **Extract file** activity is a **Data management** activity. Use this activity to export data from Adobe Campaign in an external file stored on your Campaign server. The activity must be placed after a **[!UICONTROL Build audience]** activity in order to be used.

To configure the **Extract file** activity, add an **Extract file** activity into your workflow then follow the steps below.

## Configure the file to extract {#extract-configuration}

The **[!UICONTROL File to extract]** section allows you to configure the properties of the file to extract and the data to include. 

![](../assets/extract-file-file.png)

1. In the **[!UICONTROL File name]** field, enter the desired name for the extracted file.

    You can personalize the extracted file's name using attributes from the database. To do this, click the **[!UICONTROL Open personalization dialog]** icon to open the expression editor. [Learn how to personalize your content](../../personalization/personalize.md)

1. Specify the columns to present in the extracted file. To do this, follow these steps:

    1. Click the **[!UICONTROL Add output column]**.
    1. Choose the attribute to display in the column then confirm. Available attributes depend on the targeting dimension selected in the Build audience activity.   
    1. Once the column is added, you can change its **[!UICONTROL Label]** and modify the associated **[!UICONTROL Attribute]**.
    1. If you want to apply a transformation to the column's values, select it from the drop-down list. For example, you can switch all values in the selected column to upper case.

1. Repeat these steps to add as many columns as needed in the extraction file.

1. To remove all duplicate rows from the extracted file, toggle on the **[!UICONTROL Remove duplicate rows(Listing)]** option.

1. To sort the extracted file based on an attribute, toggle on the **[!UICONTROL Enable Sorting]** option then select the attribute to use to sort the file and the sorting method to use (ascending or descending).

## Configure the extracted file format {#file}

The **[!UICONTROL Destination]** format section allows you to configure how the extracted file is formatted.

![](../assets/extract-file-format.png)

1. Choose the **[!UICONTROL Output format]** for the extracted file: **Text**, **Text using fixed with columns**, **CSV (Excel)** or **XML**. 

1. Click the **[!UICONTROL Extraction format]** button to access specific options related to the selected output format. Available values depend on the selected format.

    +++ Available Extraction format options
    
    * **[!UICONTROL Use first line as column header]** (Text / CSV (Excel) format): Toggle this option on to use the first column as header.
    * **[!UICONTROL Column separator]** (Text format): Specify the character to use as column separator in the output file.
    * **[!UICONTROL String delimiter]** (Text format): Specify how to delimit strings in the ouput file.
    * **[!UICONTROL End of line]** (Text format): Specify how to delimit the end of lines in the output file.
    * **[!UICONTROL Encoding]**: Choose the encoding of the output file.
    * **[!UICONTROL Date format and separators]**: Specify how dates should be formatted in the output file.
    * **[!UICONTROL Number format]**: Specify how numbers should be formatted in the output file.
    * **[!UICONTROL Export labels instead of internal values of enumerations]**: Toggle this option on in case you export enumeration values and you want to retrieve columns labels, which are easier to understand, rather than internal IDs.

    +++

## Add a post-processing stage {#script}

The **[!UICONTROL Export modification script]** allows you to apply a processing stage to execute during the data extraction such as zipping or encryption. To do this, click the **[!UICONTROL Edit script]** button.

The expression editor opens, allowing you to configure the script to apply. Enter the command to apply to the file. The left hand-side pane provides predefined syntaxes that you can leverage to build your script:

* The **[!UICONTROL Event variables]** menu allows you to use [events variable](#event-variables) from the workflow into your code.
* The **[!UICONTROL Conditions]** menu provides functions that allow you to build conditions. [Learn how to create condtions in the expression editor](../../personalization/conditions.md#condition-perso-editor)
* The **[!UICONTROL Add current date]** menu provides functions related to date formatting.

![](../assets/extract-file-format.png)

## Additional options {#additiona-options}

Once the output file extraction has been configured, additional options related to transitions and error management are available: 

* **[!UICONTROL Generate outbound transition]**: Toggle this option on to add an outbound transition and configure its label.
* **[!UICONTROL Do not generate a file if the inbound transition is empty]**: Toggle this option on to skip the file extraction if the inbound transition contains no data.
* **[!UICONTROL Process error]**: Toggle this option on to add an outbound transition if any error is encountered during the file extraction.

## Example {#example}

xxxx
