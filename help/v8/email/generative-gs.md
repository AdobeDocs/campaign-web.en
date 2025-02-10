---
audience: end-user
title: Get started with the AI Assistant Content Accelerator 
description: Get Started with the AI Assistant Content Accelerator 
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
---
# Work with the AI Assistant Content Accelerator  {#generative-gs}


>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI Assistant"
>abstract="Once you have crafted and personalized your delivery, you can use the AI Assistant to enhance your content. This feature simplifies the process of personalization and content improvement by allowing you to fine-tune the content by describing what you want to generate."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Define context with AI Assistant in Campaign"
>abstract="To use the selected content as an input for content generation, activate the **Enhance with current content** toggle. You can also upload your brand assets to use them as a source. If you do not use the selected content, then uploading and selecting a brand assets are mandatory."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe Generative AI terms"
>abstract="Access to this feature is subject to your agreement to the Adobe Experience Cloud Generative AI User Guidelines. Please review any output from this feature for accuracy and ensure it is appropriate for your use case."
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative AI User Guidelines"

>[!INFO]
>
>Immerse yourself in a hands-on experience with [our live feature preview](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator), designed to let you explore its features firsthand and fully understand its capabilities.


As the Marketing industry becomes more competitive, brands are seeking efficient ways to generate impactful content in an efficient and quick manner. AI Assistant Content Accelerator in Adobe Campaign Web, powered by Microsoft Azure OpenAI and Adobe Firefly, is Adobe's AI content generation capability that revolutionizes the way marketers create professional and brand-consistent content across channels like Email, SMS, Push. With advanced GenAI models and deep understanding of brand guidelines, AI Assistant auto-generates personalized, engaging, and effective content based on the marketing objective with content optimized for brand outlined styles, layouts, tone, and more. 

AI Assistant makes the creation and execution of marketing campaigns across channels like Email, SMS and Push intuitive, simple and hassle-free while saving time, improving efficiency, and driving better results.

>[!IMPORTANT]
>
>* Before starting using this capability, read out related [Guardrails and Limitations](#generative-guardrails).
>
>* You must agree to a [user agreement](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) before you can use the AI Assistant Content Accelerator in Adobe Campaign Web. For more information, contact your Adobe representative.

## Access the AI Assistant Content Accelerator {#generative-access}

The AI Assistant Content Accelerator for emails, push notifications, and SMS, is now in General Availability (GA), and available to all users. Required permissions and steps to grant access to users are detailed below.

+++  Learn how to assign Content generation related permissions

1. **Create Product Profile** -  In [Admin Console](https://stage.adminconsole.adobe.com/) create a product profile with the following specific pattern: 
    `Campaign - <instance-name> - AIAssistant`

1. **Add users** -  Add required user to that product profile, 
    or 
    **Create User Group** and add that user group to product profile and add users to that product profile.

Learn how to define permissions in Campaign in [this section](../get-started/permissions.md).

+++

## Guardrails and limitations {#generative-guardrails}

General guidelines for using the AI Assistant Content Accelerator in Adobe Campaign Web for email generation are listed below:

* The quality of the generated content is strongly influenced by the marketing objective / prompt you define. Use well defined prompt for the GenAI model to accurately interpret. 
* Upload brand asset to have accurate, on brand content. Else, content is based on publicly available info. The uploaded content can be in the following formats: PDF, JPEG, PNG, or ZIP files (with supported file formats).
* The maximum size for uploaded brand asset is 50MB. Larger files or lots of images can work but the processing time is increased.
* Use [built-in email templates](../email/create-email-templates.md), brand specific template or custom template to create your email content using Content Accelerator. Email templates with up to 8-10 images is recommended.
* Make sure to report any problematic outputs using the thumb up, thumb down or flag icons when selecting variants.
* Your use of the AI assistant is subject to the Adobe Experience Cloud Generative AI User Guidelines. [Learn more](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* As part of Adobe's commitment to promote transparency in the use of generative AI tools in media creation, Adobe will apply Content Credentials when content or a project that included a Firefly generated asset is downloaded or exported. [Learn more](https://helpx.adobe.com/firefly/using/content-credentials.html)

The following limitations apply to AI Assistant Content Accelerator in Adobe Campaign Web:

* AI Assistant Content Accelerator in Adobe Campaign Web is currently supported in English only. Non-English inputs may produce inconsistent or erroneous results. Issues arising from non-English responses will not be addressed or improved at the present time.
* Only available for the email, push and SMS channels.
* GenAI content might not always be accurate: please share your feedback so that our engineers can refine the models.
* You may upload multiple brand assets, but can leverage only one for a specific generation.

## AI Assistant content generation capabilities {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Email generation" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Email generation with the AI Assistant</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="SMS generation" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>SMS generation with the AI Assistant</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="Push generation" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Push notification generation with the AI Assistant</strong></a>
</div>
<p></td>
</tr></table>
