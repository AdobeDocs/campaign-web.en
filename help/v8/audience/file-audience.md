---
audience: end-user
title: Target recipients from a file
description: Learn how to use recipients from an external file to build your email audience
badge: label="Beta" 
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


>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="Preview your file"
>abstract="Check the preview of your file. This sceen only shows up to 30 records."



You cannot upload profiles directly into Campaign from the interface, but you can target profiles stored in an external file. Profiles are not added to the database, but all fields in the input file are available for [personalization](../personalization/gs-personalization.md). Supported file formats are: text (TXT) and comma-separated value (CSV). 

>[!CAUTION]
>
>* This capability is only available for **standalone email deliveries**. It cannot be used in workflows, nor with SMS or Push deliveries.
>
>* You cannot use [control groups](control-group.md) when loading the target population from an external file.
>
>* Profiles are not added to the database, and only loaded and available for this specific standalone email delivery.

## Select and configure your file {#upload}

To target profiles from a local file directly from the email interface, follow these steps:

1. Open an existing email delivery, or [create a new email delivery](../email/create-email.md).
1. In the email delivery creation window, from the **Audience** section, click the **Select audience** button and choose the **Select from file** option.

    ![](assets/select-from-file.png)

1. Select the local file to use. The format must align with the [sample file](#sample-file). 
1. Preview and check how data is mapped in the central section of the screen.
1. Choose the column which contains the email address from the **Address Field** drop-down. You can also select the denylist colum if you have such information in the input file.
1. Adjust the column settings, and how to format data from the available options.
1. Click **Confirm** once settings are correct.

When creating and personalizing the message content, you can select fields from the input file in the [Personalization editor](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)

## Sample file {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Load an audience from a file"
>abstract="Supported file formats are TXT and CSV. Use first line as column header. Align your file format with the sample file provided in the link below."

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

## Preview & test your email {#test}

Campaign Web allows you to preview and send test emails when using an audience uploaded from a file. To do this, follow these steps:

1. Click the **[!UICONTROL Simulate content button]** from your delivery content editing screen and click the **[!UICONTROL Add test profile(s)]** button. 

1. The profiles contained in the uploaded file display. Select the profile(s) that you want to use for previewing your content and click **[!UICONTROL Select]**.

1. A preview of the delivery content displays in the right pane of the screen. Personalized elements are replaced with the data from the profile selected in the left pane. [Learn more on delivery content preview](../preview-test/preview-content.md) 

    ![](assets/file-upload-preview.png)

1. To send test emails, click the **[!UICONTROL Test]** button.

1. Click the **[!UICONTROL Upload proof profiles]** button and select the .txt or .csv file that contains your proof recipients.

    >[!CAUTION]
    >
    >Ensure that the file format matches the one used for uploading your audience. Any format errors will display an alert.

1. When the proof recipients are added and you are ready to send the proofs, click the **[!UICONTROL Send test email]** button and confirm the sending.

    ![](assets/file-upload-test.png)

1. You can monitor the sending of the test email using the View test email log button at any time. [Learn more on test emails monitoring](../preview-test/test-deliveries.md#access-sent-test-deliveries-access-proofs)
