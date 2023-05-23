---
audience: end-user
title: Target recipients from a file
description: Learn how to use recipients from an external file to build your email audience
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
---
# Load recipients from a file {#audience-from-file}

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

You can upload contacts from an external file. This capability is only available for email deliveries. Supported file formats are: text (TXT) and comma-separated value (CSV). Profiles are not added to the database, but all fields in the input file are available for personalization.

>[!NOTE]
>
>You can build an import workflow to add or update multiple profiles in the database. Learn more


To target profiles from a local file directly from the interface, follow these steps:

1. In the email delivery creation window, from the **Audience** section, click the **Select audience** button and choose the **Select from file** option.

    ![](assets/select-from-file.png)

1. Select the local file to upload.
1. Preview and check how data is mapped in the central section of the screen.
1. Choose the column which contains the email address from the **Address Field** drop-down. You can also select the denylist colum if you have such information in the input file.
1. Adjust the column settings, and how to format data from the available options.
1. Click **Confirm** once settings are correct.

When creating and personalizing the message content, you can select fields from the input file in the Personalization editor.

![](assets/select-external-perso.png)

## Sample file {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Sample file"
>abstract="Supported file formats: txt, csv. Use first line as column header."


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
