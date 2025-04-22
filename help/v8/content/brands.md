---
audience: end-user
title: Manage brand
description: Learn how to create and manage your brand guidelines
hide: yes
hidefromtoc: yes
badge: label="Beta" type="Informative"
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
---
# Create and manage your brands {#brands}

>[!AVAILABILITY]
>
>This capability is released as a private beta. It will become progressively available to all customers in upcoming releases.

Brand guidelines are a comprehensive set of rules and standards that define a brand's visual and verbal identity. They serve as a reference to ensure consistent brand representation across all marketing and communication channels.

In [!DNL Adobe Campaign Web], users can manually enter and organize brand information or upload brand guideline documents for automatic data extraction.

## Access brands {#generative-access}

To access the **[!UICONTROL Brands]** menu in [!DNL Adobe Campaign Web], users must be assigned the **[!UICONTROL Administrator (admin)]** and **[!UICONTROL Brand kit]** product profiles to create and manage brands. For read-only access, users need the [!UICONTROL AI assistant] product profile.

[Learn more](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Learn how to assign brand-related permissions

1. In the [Admin Console](https://adminconsole.adobe.com/enterprise) home page, access your Campaign product.

    ![Admin Console home page showing Campaign product access](assets/brands_admin_1.png)

1. Select the **[!DNL Product profile]** based on the level of permissions you want to grant your user.

    ![Product profile selection in Admin Console](assets/brands_admin_2.png)

1. Click **[!DNL Add users]** to assign the selected product profile.

    ![Add users option in Admin Console](assets/brands_admin_3.png)

1. Type your user's name, user group, or email address.

1. Click **Save** to apply changes.

Users already assigned to this role have their permissions automatically updated.

+++

## Create your brand {#create-brand-kit}

To create and manage your brand guidelines, follow the steps below.

Users can either enter the details manually or upload a brand guidelines document to extract the information automatically:

1. From the **[!UICONTROL Content management]** menu, select **[!UICONTROL Brands]**.

1. In the **[!UICONTROL Brands]** menu, click **[!UICONTROL Create brand]**.

    ![Brands menu with Create brand option](assets/brands_1.png)

1. Enter a **[!UICONTROL Name]** for your brand.

1. Drag and drop or select your file to upload your brand guidelines and extract relevant brand information automatically. Click **[!UICONTROL Create brand]**.

    The information extraction process begins. Note that it may take several minutes to complete.

    ![File upload for brand guidelines extraction](assets/brands_7.png)

1. Your content and visual creation standards are automatically populated. Browse through the different tabs to adapt the information as needed.

1. From the **[!UICONTROL Writing Style]** tab, click ![Add icon](assets/do-not-localize/Smock_Add_18_N.svg) to add a guideline or exclusion, including examples.

    ![Writing Style tab with Add guideline option](assets/brands_2.png)

1. From the **[!UICONTROL Visual content]** tab, click ![Add icon](assets/do-not-localize/Smock_Add_18_N.svg) to add another guideline or exclusion.

1. To add an image showing correct usage, select **[!UICONTROL Examples]** and click **[!UICONTROL Select image]**. You can also add an image showing incorrect usage as an exclusion example.

    ![Visual content tab with example image options](assets/brands_3.png)

1. Once configured, click **[!UICONTROL Save]**, then **[!UICONTROL Publish]** to make your brand guideline available in AI Assistant.

1. To modify your published brand, click **[!UICONTROL Edit brand]**.

    >[!NOTE]
    >
    >This creates a temporary copy in edit mode, replacing the live version once published.

    ![Edit brand option in Brands menu](assets/brands_4.png)

1. From your **[!UICONTROL Brands]** dashboard, open the advanced menu by clicking the ![More options icon](assets/do-not-localize/Smock_More_18_N.svg) icon to:

    * View brand
    * Edit
    * Duplicate
    * Publish
    * Unpublish
    * Delete

    ![Advanced menu options in Brands dashboard](assets/brands_5.png)

Your brand guidelines are now accessible from the **[!UICONTROL Brand]** drop-down in AI Assistant menu. This enables AI Assistant to generate content and assets aligned with your specifications. [Learn more about AI Assistant](../email/generative-gs.md)

![AI assistant menu with Brand drop-down](assets/brands_6.png)