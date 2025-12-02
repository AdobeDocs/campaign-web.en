---
audience: end-user
title: Generative content
description: Learn how to generate complete content experiences with AI Assistant in Journey Optimizer.
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
---
# Generate full content with AI Assistant {#generative-full-content}

>[!IMPORTANT]
>
>Before starting to use this capability, read the related [Guardrails and Limitations](generative-gs.md#generative-guardrails).
></br>
>
>You must agree to a [user agreement](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} before using AI Assistant in Adobe Campaign Web. For more information, contact your Adobe representative.

Use AI Assistant in Adobe Campaign Web to generate complete content experiences across your email, landing pages, and push notification channels. AI Assistant helps you optimize the impact of your deliveries by creating comprehensive content that resonates with your audience.

## For Email and Landing page {#email-web-channels}

AI Assistant can produce complete content experiences for your email deliveries and landing pages, generating both text and images. This robust functionality helps you create compelling, on-brand content that connects with your audience across all digital touchpoints.

### Access and configure {#access-configure}

Before you begin creating content with AI Assistant, you will need to set up your delivery and open the content editor. Use the steps below to prepare your workspace and access the AI Assistant panel.

1. Create and configure your delivery:

   * **Email**: After creating and configuring your email delivery, click **[!UICONTROL Edit content]**. [Learn more](../email/create-email-content.md)
   * **Landing Page**: After creating and configuring your landing page, click **[!UICONTROL Edit content]**. [Learn more](../landing-pages/create-lp.md)

1. Personalize your layout as needed and access the **[!UICONTROL AI Assistant]** menu.

    ![AI Assistant panel showing brand selection and prompt field](assets/full-email-1.png){zoomable="yes"}

### Generate content {#generate-content}

With AI Assistant open, you can now configure the generation settings to create content that matches your brand and campaign goals. Customize text and image parameters, add brand assets, and provide prompts to guide the AI in generating relevant variations for your audience.

1. Select your **[!UICONTROL Brand]** to ensure AI-generated content aligns with your brand specifications. [Learn more](brands.md) on Brands.

1. Fine tune the content by describing what you want to generate in the **[!UICONTROL Prompt]** field. 

     If you need assistance crafting your prompt, access the **[!UICONTROL Prompt Library]**, which provides a diverse range of prompt ideas to improve your deliveries. [Learn more on prompt best practices](ai-assistant-prompting-guide.md)

    ![Screenshot showing the Prompt Library in Adobe Campaign Web](assets/full-email-2.png){zoomable="yes"}

1. **For Emails**, you can toggle the **[!UICONTROL Subject line]** and **[!UICONTROL Preheader]** options to include them in the variant generation.

1. Tailor your prompt using the **[!UICONTROL Text settings]** option:

    * **[!UICONTROL Communication strategy]**: Choose the most suitable communication style for your generated text.
    * **[!UICONTROL Languages]**: Choose the language of your generated content.
    * **[!UICONTROL Tone]**: Ensure the tone of your email resonates with your audience. Whether you want to sound informative, playful, or persuasive, AI Assistant adapts the message accordingly.

        ![Screenshot showing text settings options in Adobe Campaign Web](assets/full-email-4.png){zoomable="yes"}

1. Choose your **[!UICONTROL Image settings]**:

    * **[!UICONTROL Content type]**: Categorize the nature of the visual element, distinguishing between different forms of visual representation such as photos, graphics, or art.
    * **[!UICONTROL Visual intensity]**: Control the image's impact by adjusting its intensity. A lower setting (2) creates a softer appearance, while a higher setting (10) makes the image more vibrant.
    * **[!UICONTROL Color & tone]**: Adjust the overall appearance of the colors and the mood or atmosphere conveyed.
    * **[!UICONTROL Lighting]**: Modify the lighting in the image to shape its atmosphere and highlight specific elements.
    * **[!UICONTROL Composition]**: Arrange elements within the frame of the image.

1. From the **[!UICONTROL Reference content]** menu, click **[!UICONTROL Upload file]** to add any brand asset which contains content that can provide additional context AI Assistant or select a previously uploaded one.

    Previously uploaded files are available in the **[!UICONTROL Uploaded reference content]** drop-down. Simply toggle the assets you wish to include in your generation.

    ![Screenshot showing brands settings options in Adobe Campaign Web](assets/full-email-3.png){zoomable="yes"}

1. Once your prompt is ready, click **[!UICONTROL Generate]**.

### Refine and finalize {#refine-finalize}

After generating content variations, you can fine-tune the results to ensure they meet your exact requirements. Review the brand alignment, adjust tone and language, and prepare the content for activation in your delivery.

1. After generation, browse through the **[!UICONTROL Variations]**.

1. Click the percentage icon to view your **[!UICONTROL Brand Alignment Score]** and identify any misalignments with your brand.

    Learn more on [Brand alignment score](brands-score.md).

    ![](assets/full-email-7.png){zoomable="yes"}
    
1. Click **[!UICONTROL Preview]** to view a full-screen version of the selected variation or **[!UICONTROL Apply]** to replace your current content.

1. Navigate to the **[!UICONTROL Refine]** option within the **[!UICONTROL Preview]** window to access additional customization features:

    * **[!UICONTROL Rephrase]**: Rewrite the message while preserving its meaning. This option helps you generate alternative wording, improve flow, or adjust phrasing without changing the core message.

    * **[!UICONTROL Use simpler language]**: Leverage AI Assistant to simplify your language, ensuring clarity and accessibility for a wider audience.

    * **[!UICONTROL Translate]**: Simplify your language to ensure clarity and accessibility for a wider audience.

    * **[!UICONTROL Change tone]**: Adjust the tone of the message to better match your communication style, i.e. making it more friendly, professional, urgent, or inspirational.

    * **[!UICONTROL Change Communication strategy]**: Modify the messaging approach based on your objectives, such as creating urgency, or emphasizing exciting appeal.

        ![Refine menu displaying options](assets/full-email-5.png){zoomable="yes"}

1. Open the **[!UICONTROL Brand Alignment]** tab to see how your content aligns with your [brand guidelines](brands.md).

1. Click **[!UICONTROL Select]** once you found the appropriate content. 

1. Insert personalization fields to customize your content based on profiles data. Then, click the **[!UICONTROL Simulate content]** button to control the rendering, and check personalization settings with test profiles. [Learn more](../preview-test/preview-content.md)

1. Review and activate your content:
   * **Email**: When you have defined your content, audience and schedule, you are ready to prepare your email delivery. [Learn more](../monitor/prepare-send.md)
   * **Landing Page**: Once your landing page is ready, you can publish it to make it available for use in a message. [Learn more](../landing-pages/create-lp.md)

## For Mobile Channels {#mobile-channels}

AI Assistant also supports content generation for mobile push notifications, enabling you to create engaging titles, messages, and images for your mobile apps. This helps you maintain consistent, high-quality communication across all customer touchpoints, including mobile.

### Access and configure {#mobile-access-configure}

To use AI Assistant for push notifications, first set up your push delivery and open the content editor. The steps below will guide you through preparing your delivery and accessing the AI Assistant tools.

1. After creating and configuring your push notification delivery, click **[!UICONTROL Edit content]**.

    For more information on configuring your push delivery, refer to [this page](../push/create-push.md).

1. Personalize your push notification as needed. [Learn more](../push/content-push.md)

1. Access the **[!UICONTROL Show AI Assistant]** menu.

    ![Screenshot showing the Show AI Assistant menu](assets/push-genai-1.png){zoomable="yes"}

### Generate content {#mobile-generate-content}

Once you have accessed AI Assistant for push notifications, you can configure the generation settings to create compelling mobile content. Define your text and image preferences, select brand assets, and use prompts to generate push notification variations that engage your mobile users.

1. Select your **[!UICONTROL Brand]** to ensure AI-generated content aligns with your brand specifications. [Learn more](brands.md) on Brands.

1. Fine tune the content by describing what you want to generate in the **[!UICONTROL Prompt]** field. 

    If you are looking for assistance in crafting your prompt, access the **[!UICONTROL Prompt Library]** which provides a diverse range of prompt ideas to improve your delivery. [Learn more on prompt best practices](ai-assistant-prompting-guide.md)
    
    ![AI Assistant with Prompt field and options](assets/push-genai-2.png){zoomable="yes"}

1. Choose which field you want to generate: **[!UICONTROL Title]**, **[!UICONTROL Subtitle]**, **[!UICONTROL Message]** and/or **[!UICONTROL Image]**.

1. Tailor your prompt with the **[!UICONTROL Text settings]** option:

    * **[!UICONTROL Communication strategy]**: Choose the most suitable communication style for your generated text.
    * **[!UICONTROL Languages]**: Choose the language of your generated content.
    * **[!UICONTROL Tone]**: The tone of your push notifications should resonate with your audience. Whether you want to sound informative, playful, or persuasive, AI Assistant can adapt the message accordingly.

        ![Text settings panel for push notifications](assets/push-genai-3.png){zoomable="yes"} 

1. Choose your **[!UICONTROL Image settings]**:

    * **[!UICONTROL Content type]**: Categorize the nature of the visual element, distinguishing between different forms of visual representation such as photos, graphics, or art.
    * **[!UICONTROL Visual intensity]**: Control the image's impact by adjusting its intensity. A lower setting (2) creates a softer, more restrained appearance, while a higher setting (10) makes the image more vibrant and visually powerful.
    * **[!UICONTROL Lighting]**: Adjust the lighting in the image to shape its atmosphere and highlight specific elements.
    * **[!UICONTROL Composition]**: Arrange elements within the frame of the image.

        ![Image settings for push notifications](assets/push-genai-4.png){zoomable="yes"} 

1. From the **[!UICONTROL Reference content]** menu, click **[!UICONTROL Upload file]** to add any brand asset which contains content that can provide additional context AI Assistant or select a previously uploaded one.

    Previously uploaded files are available in the **[!UICONTROL Uploaded reference content]** drop-down. Simply toggle the assets you wish to include in your generation.

1. Once your prompt is ready, click **[!UICONTROL Generate]**.

### Refine and finalize {#mobile-refine-finalize}

After reviewing your generated push notification variations, you can polish the content to perfection. Use refinement tools to adjust language and tone, verify brand alignment, and personalize the content before activating your push campaign.

1. Browse through the generated **[!UICONTROL Variations]**.

1. Click the percentage icon to view your **[!UICONTROL Brand Alignment Score]** and identify any misalignments with your brand.

    Learn more on [Brand alignment score](brands-score.md).

    ![Generated push notification variations with Brand Alignment Score](assets/push-genai-6.png){zoomable="yes"}

1. Click **[!UICONTROL Preview]** to view a full-screen version of the selected variation or click **[!UICONTROL Apply]** to replace your current content.

1. Navigate to the **[!UICONTROL Refine]** option within the **[!UICONTROL Preview]** window to access additional customization features:

    * **[!UICONTROL Use as reference content]**: Use the chosen variant as the reference content for generating other results.
    * **[!UICONTROL Rephrase]**: Rephrase your message in different ways to keep your writing fresh and engaging for diverse audiences.
    * **[!UICONTROL Use simpler language]**: Simplify your language to ensure clarity and accessibility for a wider audience.
    * **[!UICONTROL Translate]**: Simplify your language to ensure clarity and accessibility for a wider audience.

    You can also change the **[!UICONTROL Tone]** and **[!UICONTROL Communication strategy]** of your text.

    ![Refine options for push notifications](assets/push-genai-5.png){zoomable="yes"}

1. Open the **[!UICONTROL Brand Alignment]** tab to see how your content aligns with your [brand guidelines](brands.md).

1. Click **[!UICONTROL Select]** once you found the appropriate content.

1. Insert personalization fields to customize your email content based on profile data. Then, click the **[!UICONTROL Simulate content]** button to control the rendering and check personalization settings with test profiles. [Learn more](../preview-test/preview-content.md)

When you define your content, audience, and schedule, prepare your push delivery. [Learn more](../monitor/prepare-send.md)

## How-to video {#video}

Learn how to use AI Assistant to generate full email content, text, and images.

>[!VIDEO](https://video.tv.adobe.com/v/3428984)