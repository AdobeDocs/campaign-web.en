---
audience: end-user
title: Text with the AI Assistant
description: Get Started with the AI Assistant in Campaign
badge: label="Beta"
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
hide: yes
hidefromtoc: yes
---
# Email generation with the AI Assistant {#generative-content}

>[!BEGINSHADEBOX]

**Table of content**

* [Get started with the AI Assistant](generative-gs.md)
* **[Email generation with the AI Assistant](generative-content.md)**
* [SMS generation with the AI Assistant](generative-sms.md)
* [Push notification generation with the AI Assistant](generative-push.md)

>[!ENDSHADEBOX]

Once you have created and personalized your emails, use Journey Optimizer AI Assistant in Campaign powered by generative AI to take your content to the next level.

The AI Assistant can help you optimize the impact of your deliveries by suggesting different content that is more likely to resonate with your audience.

>[!NOTE]
>
>Before starting using this capability, read out related [Guardrails and Limitations](generative-gs.md#guardrails-and-limitations).

## Content generation with the AI Assistant {#generative-text}

Here is how your AI Assistant can help you write compelling emails:

* **Summarize**: Lengthy information can overload email recipients. Use the AI Assistant to condense key points into clear, concise summaries that grab attention and encourage them to read further.

* **Elaborate**: The AI Assistant can help you expand on specific topics, providing additional details for better understanding and engagement.

* **Simplify Language**: Leverage the AI Assistant to simplify your language, ensuring clarity and accessibility for a wider audience.

* **Rephrase**:The AI Assistant can rephrase your message in different ways, keeping your writing fresh and engaging for diverse audiences.

* **Change Tone**: The tone of your email should resonate with your audience. Whether you want to sound informative, playful, or persuasive, the AI Assistant can adapt the message accordingly.

In the following example, we will leverage the AI assistant to enhance the content of our email invitation for our upcoming event.

1. After creating and configuring your email delivery, click **[!UICONTROL Edit content]**.

    For more information on how to configure your email delivery, refer to [this page](../email/create-email-content.md).

1. Personalize your email as needed and access the **[!UICONTROL AI Assistant]** menu.

    You can also select a **[!UICONTROL Text component]** to only target a specific content.

    ![](assets/text-genai-1.png){zoomable="yes"}

1. Enable the **[!UICONTROL Use original content]** option for the AI Assistant to personalize new content based on your delivery, delivery name, and selected audience.

    >[!IMPORTANT]
    >
    > Your prompt must always be tied to a specific context by uploading a brand asset or enabling the **[!UICONTROL Enhance current content]** option.

1. Fine tune the content by describing what you want to generate in the **[!UICONTROL Prompt]** field. 

    If you are looking for assistance in crafting your prompt, access the **[!UICONTROL Prompt Library]** which provides a diverse range of prompt ideas to improve your deliveries.

    ![](assets/text-genai-2.png){zoomable="yes"}

1. You can toggle the **[!UICONTROL Subject line]** or **[!UICONTROL Preheader]** to include them to the variant generation.

    Note that this is available if you did not select a specific Text component.

1. Click **[!UICONTROL Upload brand asset]** to add any brand asset which contains content that can provide additional context the AI Assistant.

    ![](assets/text-genai-3.png){zoomable="yes"}

1. Tailor your prompt with the different options:

    * **[!UICONTROL Communication strategy]**: Select the desired communication approach for the generated text.
    * **[!UICONTROL Language]**: Choose the language for the variant's content.
    * **[!UICONTROL Tone]**: Ensure that the text is appropriate for your audience and purpose.
    * **[!UICONTROL Lenght]**: Select the length of your content using the range slider. Only available if you selected a specific Text component.

    ![](assets/text-genai-4.png){zoomable="yes"}

1. Once your prompt is ready, click **[!UICONTROL Generate]**.

1. Browse through the generated **[!UICONTROL Variations]** and click **[!UICONTROL Preview]** to view a full-screen version of the selected variation.

1. Navigate to the **[!UICONTROL Refine]** option within the **[!UICONTROL Preview]** window to access additional customization features and fine-tune your variation to your preferences.

    Click **[!UICONTROL Select]** once you found the appropriate content.

    ![](assets/text-genai-5.png){zoomable="yes"}

1. Insert personalization fields to customize your email content based on profiles data. Then, click the **[!UICONTROL Simulate content]** button to control the rendering, and check personalization settings with test profiles. [Learn more](../preview-test/preview-content.md)

    ![](assets/text-genai-7.png){zoomable="yes"}

When you have defined your content, audience and schedule, you are ready to prepare your email delivery. [Learn more](../monitor/prepare-send.md)

## Image generation with the AI Assistant {#generative-image}

Leverage the AI Assistant to generate diverse and tailored visuals for your email campaigns. For instance, it can be used to:

* **Generate**: Generate a diverse range of compelling images specifically designed for your email campaigns. Granular control over settings such as color palette, lightning and composition allows you to resonate with distinct audience segments and achieve your unique campaign objectives.

* **Generate Similar**: Use the AI Assistant to generate images similar from a selected variant.

* **Brand asset**: Optimize image selection for email campaigns by leveraging both internal brand assets and external sources such as Adobe Firefly.

In the example below, learn how to leverage the AI Assistant to optimize and improve your content, ensuring a more user-friendly experience. Follow these steps:

1. After creating and configuring your email delivery, click **[!UICONTROL Edit content]**.

    For more information on how to configure your email delivery, refer to [this page](../email/create-email-content.md).

1. Fill in the **[!UICONTROL Basic details]** for your delivery. Once done, click **[!UICONTROL Edit email content]**.

1. Select the asset you want to change with the AI Assistant.

1. From the right-hand menu, select **[!UICONTROL AI Assistant]**.

    ![](assets/image-genai-1.png){zoomable="yes"}

1. Fine tune the content by describing what you want to generate in the **[!UICONTROL Prompt]** field. 

    If you are looking for assistance in crafting your prompt, access the **[!UICONTROL Prompt Library]** which provides a diverse range of prompt ideas to improve your deliveries.

    ![](assets/image-genai-2.png){zoomable="yes"}

1. Click **[!UICONTROL Upload brand asset]** to add any brand asset which contains content that can provide additional context the AI Assistant.

    >[!IMPORTANT]
    >
    > Your prompt must always be tied to a specific context.

1. Select the **[!UICONTROL Aspect ratio]** of your asset. This determines the width and height of the asset. 

    You have the option to choose from common ratios such as 16:9, 4:3, 3:2, or 1:1, or you can enter a custom size.

1. Customize the **[!UICONTROL Color & tone]**, **[!UICONTROL Content type]**, **[!UICONTROL Lighting]** and **[!UICONTROL Composition]** settings to match your desired asset characteristics.

    ![](assets/image-genai-3.png){zoomable="yes"}

1. Once you are satisfied with your prompt configuration, click **[!UICONTROL Generate]**.

1. Browse the **[!UICONTROL Variation suggestions]** to find the desired Asset.

    Click **[!UICONTROL Preview]** to view a full-screen version of the selected variation.

    ![](assets/image-genai-5.png){zoomable="yes"}

1. Choose **[!UICONTROL Show Similar]** if you want to view related images to this variant.

1. Click **[!UICONTROL Select]** once you found the appropriate content.

    ![](assets/image-genai-6.png){zoomable="yes"}

1. After defining your message content, click the **[!UICONTROL Simulate content]** button to control the rendering, and check personalization settings with test profiles.  [Learn more](../preview-test/preview-content.md)

    ![](assets/image-genai-7.png){zoomable="yes"}

1. When you have defined your content, audience and schedule, you are ready to prepare your email delivery. [Learn more](../monitor/prepare-send.md)
