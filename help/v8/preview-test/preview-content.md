---
audience: end-user
title: Preview delivery content
description: Learn how to preview your delivery content with Campaign Web UI
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Limited Availability"
---

# Preview the message content {#preview-content} 

Use the [!DNL Campaign] content simulation capability to preview the content of your message before sending it. This allows you to control personalization and check how it is displayed to your recipients.

To preview the content of your delivery, follow the steps below.

1. Browse to the edit content screen of your delivery or to the [Email Designer](../email/get-started-email-designer.md).

1. Click the **[!UICONTROL Simulate content]** button.

    ![](assets/simulate-button.png)

1. To select the profiles that will be used to preview your personalized content, use:

    * **[!UICONTROL Add test profile(s)]** for previewing email and SMS deliveries

    * **[!UICONTROL Add subscriber(s)]** for previewing push notifications

1. You can combine test profiles and profiles to preview your email or SMS message.

    * The **[!UICONTROL Test profiles]** tab lists all seed addresses, which are additional and fictitious recipients in the database.

        ![](assets/simulate-select-profiles.png)
    
        >[!NOTE]
        >
        >Test profiles can be created from the **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]** menu. [Learn more](../audience/test-profiles.md#create-test-profiles)

    * The **[!UICONTROL Profiles]** tab lists all the recipients stored into the **[!UICONTROL Profiles and Targets]** folder from the [!DNL Campaign] console. Learn more in [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}. 
    
        >[!NOTE]
        >
        >You can also view and manage profiles from the corresponding tab in the Campaign web UI. [Learn more](../audience/about-recipients.md)

1. Click **[!UICONTROL Select]** to confirm your selection.

    A preview of the delivery content is displayed in the right pane of the **[!UICONTROL Simulate]** screen. Personalized elements are replaced with the data from the profile selected in the left pane.

    ![](assets/simulate-preview.png)

1. If you have added multiple profiles, you can switch between them in the list to preview the corresponding delivery content. You can also add more test profiles and clear your selection using the corresponding buttons on the left pane.

1. For email deliveries, you can adjust the **[!UICONTROL Zoom level]** and preview your content on desktop or mobile device using the dedicated icon in the top right corner.

1. From the **[!UICONTROL Simulate]** screen you can also:
    * Send test deliveries to specific recipients for validation - [Learn more](test-deliveries.md)
    * Access the logs of the sent test deliveries - [Learn more](test-deliveries.md#access-test-deliveries)
    * For email only, check the message content rendering in popular email clients - [Learn more](email-rendering.md)



