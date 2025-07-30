---
audience: end-user
title: Push notification with AI Assistant
description: Get Started with AI Assistant
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
---
# Push notification generation with AI Assistant {#generative-push}

>[!IMPORTANT]
>
>Before starting to use this capability, read the related [Guardrails and Limitations](generative-gs.md#generative-guardrails).
></br>
>
>You must agree to a [user agreement](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) before using AI Assistant in Adobe Campaign Web. For more information, contact your Adobe representative.

AI Assistant helps optimize the impact of your deliveries by suggesting different content that resonates with your audience.

In the following example, AI Assistant is leveraged to craft compelling messaging to create a more engaging customer experience.

1. After creating and configuring your push notification delivery, click **[!UICONTROL Edit content]**.

    For more information on configuring your push delivery, refer to [this page](../push/create-push.md).

1. Access the **[!UICONTROL Show AI Assistant]** menu.

    ![Screenshot showing the Show AI Assistant menu](assets/push-genai-1.png){zoomable="yes"}

1. Enable the **[!UICONTROL Use original content]** option for AI Assistant to personalize new content based on the selected content.

1. Fine-tune the content by describing what you want to generate in the **[!UICONTROL Prompt]** field.

    If assistance is needed in crafting your prompt, access the **[!UICONTROL Prompt Library]**, which provides a diverse range of prompt ideas to improve your deliveries.

    ![Screenshot showing the Prompt Library interface](assets/push-genai-2.png){zoomable="yes"}

1. Choose the field you want to generate: **[!UICONTROL Title]**, **[!UICONTROL Subtitle]**, **[!UICONTROL Message]**, and/or **[!UICONTROL Image]**.

1. Tailor your prompt using the **[!UICONTROL Text settings]** option:

    * **[!UICONTROL Communication strategy]**: Choose the most suitable communication style for your generated text.
    * **[!UICONTROL Tone]**: Adjust the tone of your email to resonate with your audience. Whether you want to sound informative, playful, or persuasive, AI Assistant adapts the message accordingly.

    ![Screenshot showing Text settings options](assets/push-genai-3.png){zoomable="yes"}

1. Choose your **[!UICONTROL Image settings]**:

    * **[!UICONTROL Content type]**: Categorize the nature of the visual element, distinguishing between different forms of visual representation such as photos, graphics, or art.
    * **[!UICONTROL Visual intensity]**: Control the image's impact by adjusting its intensity. A lower setting (2) creates a softer, more restrained appearance, while a higher setting (10) makes the image more vibrant and visually powerful.
    * **[!UICONTROL Lighting]**: Adjust the lighting in the image to shape its atmosphere and highlight specific elements.
    * **[!UICONTROL Composition]**: Arrange elements within the frame of the image.

    ![Screenshot showing Image settings options](assets/push-genai-4.png){zoomable="yes"}

1. From the **[!UICONTROL Brand assets]** menu, click **[!UICONTROL Upload brand asset]** to add any brand asset containing content that provides additional context to AI Assistant, or select a previously uploaded one.

    Previously uploaded files are available in the **[!UICONTROL Uploaded brand assets]** drop-down. Toggle the assets you wish to include in your generation.

1. Once your prompt is ready, click **[!UICONTROL Generate]**.

1. Browse through the generated **[!UICONTROL Variations]** and click **[!UICONTROL Preview]** to view a full-screen version of the selected variation or **[!UICONTROL Apply]** to replace your current content.

1. Click the percentage icon to view your **[!UICONTROL Brand Alignment Score]** and identify any misalignments with your brand.

    Learn more on [Brand alignment score](../content/brands-score.md).

    ![](assets/push-genai-6.png){zoomable="yes"}

1. Navigate to the **[!UICONTROL Refine]** option within the **[!UICONTROL Preview]** window to access additional customization features:

    * **[!UICONTROL Use as reference content]**: Use the chosen variant as the reference content for generating other results.
    * **[!UICONTROL Rephrase]**: Rephrase your message in different ways to keep your writing fresh and engaging for diverse audiences.
    * **[!UICONTROL Use simpler language]**: Simplify your language to ensure clarity and accessibility for a wider audience.

    You can also change the **[!UICONTROL Tone]** and **[!UICONTROL Communication strategy]** of your text.

    ![Screenshot showing Refine options](assets/push-genai-5.png){zoomable="yes"}

1. Open the **[!UICONTROL Brand Alignment]** tab to see how your content aligns with your [brand guidelines](../content/brands.md).

1. Click **[!UICONTROL Select]** once you find the appropriate content.

1. Insert personalization fields to customize your email content based on profile data. Then, click the **[!UICONTROL Simulate content]** button to control the rendering and check personalization settings with test profiles. [Learn more](../preview-test/preview-content.md)

When you define your content, audience, and schedule, prepare your push delivery. [Learn more](../monitor/prepare-send.md)