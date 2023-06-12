---
audience: end-user
title: Preview email content
description: Learn how to preview your email content with Campaign Web UI
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Alpha" type="Positive"
---

# Preview email content {#preview-content} 

Use the [!DNL Campaign] content simulation capability to preview the content of your email before sending it. This allows you to control personalization and check how it is displayed to your recipients.

To preview the content of your email, follow the steps below.

1. Browse to the email [Edit content](../content/edit-content.md) screen or to the [Email Designer](../content/get-started-email-designer.md).

1. Click the **[!UICONTROL Simulate content]** button.

    ![](assets/simulate-button.png)

1. Use the **[!UICONTROL Add test profile(s)]** button to select the profiles that will be used to preview your personalized content.

1. You can combine test profiles and profiles to preview your email. 

    * The **[!UICONTROL Test profiles]** tab lists all seed addresses, which are additional and fictitious recipients in the database.
    
        >[!NOTE]
        >
        >Test profiles can be created in the [!DNL Campaign] console into the **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** folder. Learn more in [Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

    * The **[!UICONTROL Profiles]** tab lists all the recipients stored into the **[!UICONTROL Profiles and Targets]** folder from the [!DNL Campaign] console. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}

    ![](assets/simulate-select-profiles.png)

1. Click **[!UICONTROL Select]** to confirm your selection in both tabs.

    A preview of the email is displayed in the right pane of the **[!UICONTROL Simulate]** screen. Personalized elements are replaced with the data from the profile selected in the left pane.

    ![](assets/simulate-preview.png)

1. If you have added multiple profiles, you can switch between them in the list to preview the corresponding email content. You can also add more test profiles and clear your selection using the corresponding buttons on the left pane.

1. You can adjust the **[!UICONTROL Zoom level]** and preview your content on desktop or mobile device using the dedicated icon in the top right corner.

1. From the **[!UICONTROL Simulate]** screen you can also:
    * Check the email rendering in popular email clients - [Learn more](email-rendering.md)
    * Send test emails to specific recipients for validation - [Learn more](proofs.md)



