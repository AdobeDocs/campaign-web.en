---
audience: end-user
title: Get started with the Content Assistant
description: Get Started with the Content Assistant
badge: label="Beta" 
---

# Get started with the Content Assistant {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Content Assistant"
>abstract="Once you have crafted and personalized your delivery, you can use the Content Assistant to enhance your content. This feature simplifies the process of personalization and content improvement by allowing you to fine-tune the content by describing what you want to generate."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Define context for content generation"
>abstract="To use the selected content as an input for content generation, activate the **Enhance with current content** toggle. You can also upload your brand assets to use them as a source. If you do not use the selected content, then uploading and selecting a brand assets are mandatory."

The Content Assistant, powered by generative AI, is a valuable tool for improving email content. It simplifies personalization and content enhancement, optimizing your email deliveries to better resonate with your audience. 

This feature saves time and ensures consistent quality by automatically generating complete email content. By using Generative AI, you can create compelling emails effortlessly, improving your communication's effectiveness and efficiency.

You can the Campaign Content Assistant in your emails to: [generate images](generative-image.md), [generate text content](generative-content.md), [generate the full HTML content](generative-email.md).


## Guardrails and limitations {#generative-guardrails}

General guidelines for using Content Assistant for email generation are listed below:

* The quality of the generated content is strongly influenced by the marketing objective / prompt you define. Use well defined prompt for the GenAI model to accurately interpret. 
* Upload brand asset to have accurate, on brand content. Else, content is based on publicly available info. The uploaded content can be: PDF files, Microsoft Word documents, JPEG, PNG, or ZIP files (with supported file formats).
* The recommended size for uploaded brand asset is less than 10MB. Larger files or lots of images can work but the processing time is increased.
* Use an Adobe Campaign authored email templates, or preferably [built-in email templates](../content/email-sample-templates.md) to create your email content. Email template with up to 8-10 images is recommended.


The following limitations apply to Campaign Content Assistant:

* Supported language is English only
* Only available for the email channel
* GenAI content might not always be accurate: please share your feedback so that our engineers can refine the models
* You may upload multiple brand assets, but can leverage only one for a specific generation

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Text generation" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Text generation with the Content Assistant</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="Image generation" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>Image generation with the Content Assistant</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="Email generation" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>Email generation with the Content Assistant</strong></a>
</div>
<p></td>
</tr></table>

