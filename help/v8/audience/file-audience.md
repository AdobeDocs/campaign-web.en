---
audience: end-user
title: Target recipients from a file
description: Learn how to use recipients from an external file to build your email audience
badge: label="Alpha" 
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
---
# Load an email audience from a file {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="File selection"
>abstract="Select the local file to upload. Supported formats are TXT and CSV. Align your file format with the sample file linked below."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Columns definition"
>abstract="Check the format of the columns to insert from your local file."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Formatting parameters"
>abstract="Check the formatting parameters for your file."

You can upload contacts from an external file. Profiles are not added to the database, but all fields in the input file are available for [personalization](../personalization/gs-personalization.md). Supported file formats are: text (TXT) and comma-separated value (CSV). 

>[!CAUTION]
>
>* This capability is only available for **standalone email deliveries**. It cannot be used in workflows, nor with SMS or Push deliveries.
>
>* You cannot use [control groups](control-group.md) when loading the target population from an external file.


To target profiles from a local file directly from the email interface, follow these steps:

1. Open an existing email delivery, or [create a new email delivery](../email/create-email.md).
1. In the email delivery creation window, from the **Audience** section, click the **Select audience** button and choose the **Select from file** option.

    ![](assets/select-from-file.png)

1. Select the local file to upload. The format must align with the [sample file](#sample-file). 
1. Preview and check how data is mapped in the central section of the screen.
1. Choose the column which contains the email address from the **Address Field** drop-down. You can also select the denylist colum if you have such information in the input file.
1. Adjust the column settings, and how to format data from the available options.
1. Click **Confirm** once settings are correct.

When creating and personalizing the message content, you can select fields from the input file in the [Personalization editor](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)


## Sample file {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Sample file"
>abstract="Supported file formats: txt, csv. Use first line as column header."

Supported formats are TXT and CSV. The first line is the column header.

Align your file format with the sample file below:

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
