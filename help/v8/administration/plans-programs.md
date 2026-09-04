---
audience: end-user
title: Plans and Programs
description: Learn how to create and configure plans and programs in Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
TQID: https://experienceleague.adobe.com/FSiHCjupRlS0zoI9HPdcU--Y2PZot5fQOzWICwmV-oQ
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: b82389f8-9b5e-4083-8e3b-3cef299fb8b9
    internal-label: Schemas
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Plans and programs {#plan-and-programs}

Adobe Campaign allows you to configure your folder hierarchy for marketing plans and programs.

To better organize these components, Adobe recommends the following hierarchy: Plan `>` Programs `>` Campaigns.

* A **plan** may contain multiple programs. It defines strategic objectives for a specific period.
* A **program** may contain other programs as well as campaigns, workflows, and landing pages.
* A **campaign** may contain deliveries, workflows, and landing pages.

## Create and configure a plan {#create-plan}

To create a plan, create a folder with the folder type **[!UICONTROL Plan]**. [Learn more about creating a folder](../get-started/work-with-folders.md)

![Screenshot showing the creation of a plan folder](assets/plan_create.png){zoomable="yes"}

Go to the **[!UICONTROL Folder settings]** of your plan to manage it.

![Screenshot showing the folder settings for a plan](assets/plan_settings.png){zoomable="yes"}

Define **[!UICONTROL Custom options]**, and set the scheduling date of your plan.

![Screenshot showing the custom options for a plan](assets/plan_options.png){zoomable="yes"}

To manage the **[!UICONTROL Custom options]**:

1. Browse to the **[!UICONTROL Schemas]**.
1. Choose the **[!UICONTROL Editable]** schemas in the filters.
1. Click the schema.

![Screenshot showing the editing of custom details for a plan](assets/plan_edit.png){zoomable="yes"}

1. Click the **[!UICONTROL Screen edition]** button.

    ![](assets/plan_edit2.png){zoomable="yes"}

Configure the custom options:

![Screenshot showing the configuration of custom fields for a plan](assets/plan_customfields.png){zoomable="yes"}

## Create and configure a program {#create-program}

Programs are available from the left navigation menu, similar to the list views for campaigns, deliveries, and workflows. The **[!UICONTROL Programs]** entry lets you create a program within an existing program, not under a plan. 

To create your first, top-level program in a plan, navigate to your plan in the Explorer (see this [section](#create-plan)), and create a folder with the folder type **[!UICONTROL Program]**. [Learn more about creating a folder](../get-started/work-with-folders.md).

To create a program within an existing program, follow the steps below:

1. Browse to the **[!UICONTROL Programs]** entry in the left navigation menu. This view lists all your programs and lets you search and filter. Clicking a program opens it in the Explorer view.

   ![Screenshot showing the program list view](assets/program_view.png){zoomable="yes"}

1. Click **[!UICONTROL Create program]** and configure the following options:

   ![Screenshot showing the Create program screen](assets/program_create.png){zoomable="yes"}

   * Enter a **[!UICONTROL Label]**.
   * Select the existing program to use as the **[!UICONTROL Parent folder]**.
   * Optionally, set a **[!UICONTROL Date range]** in the **[!UICONTROL Schedule]** section.

   >[!TIP]
   >
   >If you create a program from the Explorer view, the parent folder is automatically set to the current program.

1. Click **[!UICONTROL Create program]** again to save changes and create the program. The program is then displayed in the Explorer view. You can rename it, delete it, and access its settings, like any other folder. You can also create sub-programs within this program.

   ![Screenshot showing the program in the Explorer view](assets/program_explorer.png){zoomable="yes"}

Custom options for a program are configured the same way as for a plan. See [Create and configure a plan](#create-plan).

## How to link a campaign to a program

You have two ways to link a campaign to a program:

### Way #1: You already have a program and want to create a campaign linked to it

To link a new campaign to your program, create the campaign directly within the program.

![Screenshot showing the creation of a campaign within a program](assets/program_campaign_create.png){zoomable="yes"}

The **[!UICONTROL Folder]** settings will automatically populate with the path to your program.

![Screenshot showing the folder settings for a campaign linked to a program](assets/program_campaign_folder.png){zoomable="yes"}

### Way #2: You already have an existing campaign and want to link it to an existing program

Go to the **[!UICONTROL Settings]** button of the campaign you want to link to your program.

![Screenshot showing the settings button for a campaign](assets/campaign_settings.png){zoomable="yes"}

In its **[!UICONTROL Properties]**, click the **[!UICONTROL Folder]** icon in the **[!UICONTROL Folder]** settings to choose your **[!UICONTROL Program]** folder.

![Screenshot showing the folder selection for linking a campaign to a program](assets/campaign_folder.png){zoomable="yes"}

Select your **[!UICONTROL Program]** folder, click the **[!UICONTROL Confirm]** button, and then click the **[!UICONTROL Save and Close]** button.

![Screenshot showing a campaign linked to a program](assets/campaign_linked.png){zoomable="yes"}

Your campaign is now listed in your program.

![Screenshot showing a campaign listed within a program](assets/campaign_in_program.png){zoomable="yes"}