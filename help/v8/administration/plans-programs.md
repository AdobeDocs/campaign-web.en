---
audience: end-user
title: Plans and Programs
description: Learn how to create and configure plans and programs in Adobe Campaign

---
# Plans and Programs

Adobe Campaign allows you to configure your folder hierarchy for marketing plans and programs.
To better organize them, Adobe recommends the following hierarchy : Plan > Programs > Campaigns
- A **plan** may contain multiple programs. It defines strategic objectives for a period of time.
- A **program** may contain other programs as well as campaigns, workflows and landing pages.
- A **campaign** may contain deliveries, workflows and landing pages.

## Create and configure a plan {#create-plan}

To create a plan, you need to create a folder with the folder type **[!UICONTROL Plan]** [Learn more about creating a folder](create-manage-folder.md).

  ![](assets/plan_create.png){zoomable="yes"}

Go to the **[!UICONTROL Folder settings]** of your plan to manage it. 

![](assets/plan_settings.png){zoomable="yes"}

You have the possibility to define **[!UICONTROL Custom options]**, and to set the scheduling date of your plan.

![](assets/plan_options.png){zoomable="yes"}

To manage the  **[!UICONTROL Custom options]** :
- Go to the **[!UICONTROL Schemas]**
- Choose the **[!UICONTROL Editable]** schemas in the filters
- Click on the icon of **[!UICONTROL Edit custom details]**

![](assets/plan_edit.png){zoomable="yes"}

You will have the possibility to configure them : 

![](assets/plan_customfields.png){zoomable="yes"}

## Create and configure a program

To create a program in your plan ([Learn more about creating a plan](#create-plan)), you need to be in your plan and create a folder with the folder type **[!UICONTROL Program]** [Learn more about creating a folder](create-manage-folder.md).

![](assets/program_create.png){zoomable="yes"}

Go to the **[!UICONTROL Folder settings]** of your program to manage it. 

![](assets/program_settings.png){zoomable="yes"}

You have the possibility to define **[!UICONTROL Custom options]**, and to set the scheduling date of your program.

![](assets/program_options.png){zoomable="yes"}

To manage the  **[!UICONTROL Custom options]** :
- Go to the **[!UICONTROL Schemas]**
- Choose the **[!UICONTROL Editable]** schemas in the filters
- Click on the icon of **[!UICONTROL Edit custom details]**

![](assets/program_edit.png){zoomable="yes"}

You will have the possibility to configure them : 

![](assets/program_customfields.png){zoomable="yes"}

## How to link a campaign to a program

You have 2 ways to link a campaign to a program :

#### Way #1 : You already have a program and want to create a campaign linked to it

To link a new campaign to your program, create directly you campaign in the program : 

![](assets/program_campaign_create.png){zoomable="yes"}

The **[!UICONTROL Folder]** settings will be automatically filed with the path to your program.

![](assets/program_campaign_folder.png){zoomable="yes"}

#### Way #2 : You already have an existing campaign and want to link it to an existing program

Go to the **[!UICONTROL Settings]** button of the campaign you want to link to your program : 

![](assets/campaign_settings.png){zoomable="yes"}

In its **[!UICONTROL Properties]**, click the **[!UICONTROL Folder]** icon in the **[!UICONTROL Folder]** settings, in order to choose your **[!UICONTROL Program]** folder.

![](assets/campaign_folder.png){zoomable="yes"}

Select your **[!UICONTROL Program]** folder and click on **[!UICONTROL Confirm]** button, and then on **[!UICONTROL Save and Close]** button.

![](assets/campaign_linked.png){zoomable="yes"}

Your campaign is now listed in your program : 

![](assets/campaign_in_program.png){zoomable="yes"}