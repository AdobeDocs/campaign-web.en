---
audience: end-user
title: Import recipients from a file
description: Learn how to import recipients from an external file
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
---
# Import recipients from a file {#audience-from-file}

You can add or update contacts from the delivery interface, by uploading a text file (TXT) or a comma-separated value file (CSV). They will then be added to the database. 

>[!NOTE]
>
>You can also build an import workflow to add or update multiple profiles.  


To add profiles from a local file directly from the interface, follow these steps:

1. In the delivery creation window, click the **Select audience** button and select the **Select from file** option.
1. Select the local file to upload.
1. Define the column settings and how to format data. You can skip a column using the **Ignore column** toggle.
1. Preview how data is mapped in the central section of the screen.
1. Click **Confirm** once settings are correct.

When creating and personalizing the message content, you can select fields from the input file in the Personalization editor.

## Sample file {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Sample file"
>abstract="Supported file formats: txt, csv, xls. Use first line as column header."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
