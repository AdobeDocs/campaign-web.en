---
audience: end-user
title: Get started with AI Assistant
description: Get Started with AI Assistant
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
---
# Work with AI Assistant {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI Assistant"
>abstract="After crafting and personalizing your delivery, use AI Assistant to enhance your content. This feature simplifies personalization and content improvement by allowing you to fine-tune the content by describing what you want to generate."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Define context with AI Assistant in Campaign"
>abstract="To use the selected content as input for content generation, activate the **Enhance with current content** toggle. You can also upload your brand assets to use them as a source. If you do not use the selected content, uploading and selecting brand assets are mandatory."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe Generative AI terms"
>abstract="Access to this feature depends on your agreement to the Adobe Experience Cloud Generative AI User Guidelines. Review any output from this feature for accuracy and ensure it is appropriate for your use case."
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative AI User Guidelines"

>[!INFO]
>
>Immerse yourself in a hands-on experience with [our live feature preview](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator), designed to let you explore its features firsthand and fully understand its capabilities.

As the marketing industry becomes more competitive, brands seek efficient ways to generate impactful content quickly. AI Assistant in Adobe Campaign Web, powered by Microsoft Azure OpenAI and Adobe Firefly, is Adobe's AI content generation capability that transforms how marketers create professional and brand-consistent content across channels like email, SMS, and push notifications. With advanced GenAI models and a deep understanding of brand guidelines, AI Assistant auto-generates personalized, engaging, and effective content based on the marketing objective, optimizing content for brand-outlined styles, layouts, tone, and more.

AI Assistant simplifies the creation and execution of marketing campaigns across channels like email, SMS, and push notifications, saving time, improving efficiency, and driving better results.

>[!IMPORTANT]
>
>* Before using this capability, review the related [Guardrails and Limitations](#generative-guardrails).
>
>* You must agree to a [user agreement](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) before using AI Assistant in Adobe Campaign Web. For more information, contact your Adobe representative.

## Access AI Assistant {#generative-access}

AI Assistant for emails, push notifications, and SMS is now in General Availability (GA) and available to all users. Required permissions and steps to grant access to users are detailed below.

+++ Learn how to assign Content generation-related permissions

1. **Create Product Profile** - In [Admin Console](https://stage.adminconsole.adobe.com/), create a product profile with the following specific pattern: 
    `Campaign - <instance-name> - AIAssistant`

1. **Add users** - Add the required user to that product profile,  
    or  
    **Create User Group** and add that user group to the product profile, then add users to that product profile.

Learn how to define permissions in Campaign in [this section](../get-started/permissions.md).

+++

## Guardrails and limitations {#generative-guardrails}

General guidelines for using AI Assistant in Adobe Campaign Web for email generation are listed below:

* The quality of the generated content depends heavily on the marketing objective or prompt you define. Use a well-defined prompt for the GenAI model to interpret accurately.  
* Upload brand assets to ensure accurate, on-brand content. Otherwise, content is based on publicly available information. The uploaded content can be in the following formats: PDF, JPEG, PNG, or ZIP files (with supported file formats).  
* The maximum size for uploaded brand assets is 50MB. Larger files or numerous images may increase processing time.  
* Use [built-in email templates](../content/create-email-templates.md), brand-specific templates, or custom templates to create your email content using AI Assistant. Email templates with up to 8–10 images are recommended.  
* Report any problematic outputs using the thumbs-up, thumbs-down, or flag icons when selecting variants.  
* Your use of AI Assistant is subject to the Adobe Experience Cloud Generative AI User Guidelines. [Learn more](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).  
* As part of Adobe's commitment to transparency in the use of generative AI tools in media creation, Adobe applies Content Credentials when content or a project that includes a Firefly-generated asset is downloaded or exported. [Learn more](https://helpx.adobe.com/firefly/using/content-credentials.html).  

The following limitations apply to AI Assistant in Adobe Campaign Web:

* AI Assistant in Adobe Campaign Web is currently supported in English only. Non-English inputs may produce inconsistent or erroneous results. Issues arising from non-English responses will not be addressed or improved at this time.  
* Only available for the email, push, and SMS channels.  
* GenAI content might not always be accurate. Share your feedback so engineers can refine the models.  
* You may upload multiple brand assets but can leverage only one for a specific generation.  

## AI Assistant content generation capabilities {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[Email generation with AI Assistant]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Email generation with AI Assistant</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[SMS generation with AI Assistant]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>SMS generation with AI Assistant</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[Push notification generation with AI Assistant]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Push notification generation with AI Assistant</strong></a>
</div>
<p></td>
</tr></table>