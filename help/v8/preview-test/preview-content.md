---
audience: end-user
title: Preview delivery content
description: Learn how to preview your delivery content with Campaign Web user interface
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
---
# Preview the message content {#preview-content}

Use the [!DNL Campaign] content simulation capability to preview the content of your message before sending it. This feature allows you to control personalization and check how the message is displayed to your recipients.

To preview the content of your delivery, follow these steps:

1. Browse to the edit content screen of your delivery or to the [Email Designer](../email/get-started-email-designer.md).

1. Click the **[!UICONTROL Simulate content]** button.

    ![Image showing the Simulate content button](assets/simulate-button.png){zoomable="yes"}

1. Select the profiles to use for previewing your content. To perform this action, click the **[!UICONTROL Add test profile(s)]** button (for email and SMS) or the **[!UICONTROL Add subscriber(s)]** button (for push notifications).

1. Combine profiles and test profiles to preview your email or SMS message.

    * The **[!UICONTROL Test profiles]** tab lists all test profiles, which are additional and fictitious recipients in the database. [Learn how to work with test profiles](../audience/test-profiles.md).

    * The **[!UICONTROL Profiles]** tab lists all the profiles stored in your database. [Learn how to work with profiles](../audience/about-recipients.md).
    
    ![Image showing the selection of profiles](assets/simulate-select-profiles.png){zoomable="yes"}

1. When browsing the test profile or profile lists, use filters to refine your search. For example, define a rule to find all test profiles with the **[!UICONTROL Prospect]** status. [Learn how to add rules using the query modeler](../query/query-modeler-overview.md).

    ![Image showing filters applied to test profiles](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. Click **[!UICONTROL Select]** to confirm your selection.

    A preview of the delivery content appears in the right pane of the **[!UICONTROL Simulate]** screen. Personalized elements are replaced with the data from the profile selected in the left pane.

    ![Image showing the preview of delivery content](assets/simulate-preview.png){zoomable="yes"}

1. If multiple profiles are added, switch between them in the list to preview the corresponding delivery content. Add more test profiles or clear your selection using the corresponding buttons on the left pane.

1. For email deliveries, adjust the **[!UICONTROL Zoom level]** and preview your content on a desktop or mobile device using the dedicated icon in the top right corner.

1. From the **[!UICONTROL Simulate]** screen, you can also:
    * Send proofs to specific recipients for validation - [Learn more](test-deliveries.md).
    * Access the logs of the sent proofs - [Learn more](test-deliveries.md#access-test-deliveries).
    * For email only, check the message content rendering in popular email clients - [Learn more](email-rendering.md).