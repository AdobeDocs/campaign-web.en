---
title: Work with GenStudio for Performance Marketing into Adobe Campaign
description: Learn to work with GenStudio for Performance Marketing in Adobe Campaign
feature: Email Design
topic: Content Management, Artificial Intelligence
role: User
level: Beginner, Intermediate
exl-id: c22a44a8-e4e2-453a-9ca2-b80f7c0edc19
---
# Work with GenStudio for Performance Marketing {#genstudio}

>[!CONTEXTUALHELP]
>id="ac_genstudio_button"
>title="Use a template built with GenStudio"
>abstract="Thanks to the seamless integration with Adobe GenStudio for Performance Marketing, you can easily import a GenStudio template enhanced with the Adobe AI technology."

## Get started with GenStudio {#gs-genstudio}

[Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"} is a generative AI-first application that lets marketing teams create their own ads and emails to drive impactful, personalized marketing campaigns that adhere to your brand standards and complies with your enterprise policies. By leveraging Adobe AI technology, it provides a comprehensive suite of tools that simplify the complexities of content creation and management so that creatives can focus on innovation.

>[!AVAILABILITY]
>
>This capability is available for the email channel only.

To enhance marketing efficiciency and to maintain brand consistency, you can seamlessly integrate [!DNL **GenStudio for Performance Marketing**] experiences with [!DNL **Adobe Campaign**]. This enable you to leverage [!DNL GenStudio]'s AI-power content creation alongside [!DNL Adobe Campaign]'s advanced orchestration capabilities.

>[!INFO]
>
>To go further, check out this [overview](https://business.adobe.com/products/genstudio-for-performance-marketing.html#watch-overview){target="_blank"} and a [demo](https://business.adobe.com/products/genstudio-for-performance-marketing.html#demo){target="_blank"} of [!DNL Adobe GenStudio for Performance Marketing].

## Use GenStudio capabilities in Adobe Campaign {#use-genstudio}

The [!DNL GenStudio for Performance Marketing] and [!DNL Adobe Campaign] integration enables you to have marketers from your company work better together to streamline processes.

For example, a technical marketer, who uses [!DNL Adobe Campaign] to develop and automate email campaigns, can collaborate with a performance marketer who creates content using [!DNL GenStudio].

With this integration, both can work together to easily integrate on-brand content from [!DNL GenStudio] into [!DNL Adobe Campaign], delivering engaging emails that target specific customer segments and drive sales.

### Export an HTML template from Adobe Campaign to GenStudio {#export-from-campaign-to-genstudio}

First, you can export a [!DNL Adobe Campaign] HTML template including your brand's guidelines to [!DNL GenStudio for Performance Marketing]. Follow the steps below.

1. In [!DNL Adobe Campaign], access the content of your email. [Learn how](../email/create-email.md#create-content)

1. In the Email Designer, select **[!UICONTROL Export HTML]** from the **[!UICONTROL More]** button.

    ![](assets/genstudio-export-template.png){zoomable="yes"}

1. Upload this HTML exported template into [!DNL GenStudio for Performance Marketing]. <!--Make sure you detect the fields that the generative AI uses to insert content in order to create an actionable template.-->

    >[!NOTE]
    >
    >Learn how to upload an HTML template into [!DNL GenStudio] in the [Adobe GenStudio for Performance Marketing User Guide](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"} dedicated section.<!--GenStudio doc to be updated with Campaign-->

1. In GenStudio, use this template to create several email variations with AI prompts and save them.

    >[!NOTE]
    >
    >Learn how to create email experiences in the GenStudio dedicated [section](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"}.
 
### Leverage GenStudio experiences in Adobe Campaign {#leverage-genstudio-experiences}

To leverage the [!DNL GenStudio] email variations that you just created by importing them into [!DNL Adobe Campaign], follow the steps below.

1. In [!DNL Adobe Campaign], [create an email delivery](../email/create-email.md).

1. From the email delivery dashboard, click the **[!UICONTROL Edit content]** button. [Learn more](../email/create-email.md#create-content)

1. On the Email Designer home page, select **[!UICONTROL Import HTML]** and click the **[!UICONTROL Adobe GenStudio for Performance Marketing]** button.

    ![](assets/genstudio-pem-import-email.png){zoomable="yes"}

1. Browse the GenStudio experiences to start building your content. You can filter the experiences on several criteria such as products, personas, brands, or even colors.

    <!--![](assets/genstudio-filter-experiences.png){zoomable="yes"}-->

1. Select an experience and click **[!UICONTROL Use]**.

    ![](assets/genstudio-use-experience.png){zoomable="yes"}

1. Select the folder where you want to import the GenStudio experience.

    ![](assets/genstudio-choose-destination.png){zoomable="yes"}

1. The selected content displays in the Email Designer.

    ![](assets/genstudio-email-content.png){zoomable="yes"}

    >[!NOTE]
    >
    >GenStudio experiences [created from a [!DNL Adobe Campaign] template](#export-from-ajo-to-genstudio) are imported directly into the Email Designer. GenStudio experiences created without a [!DNL Adobe Campaign] template are imported into [compatibility mode](../email/existing-content.md).

    Use the [email content editing tools](../email/create-email-content.md) and [personalization fields](../personalization/personalize.md) to edit your email as wanted. Save your content.

<!--Detail a use case with A/B testing to import other GenStudio variations and track how your tratments are performing.-->


<!--
## How-to video {#video}

Discover the process of exporting an email template from Adobe Campaign to GenStudio for Performance Marketing, crafting brand-compliant emails using the template in GenStudio, and importing them seamlessly back into Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3456038/?quality=12)
TO REPLACE WITH CAMPAIGN VIDEO WHEN/IF RELEASED
-->