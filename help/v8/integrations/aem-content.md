---
audience: end-user
title: Manage assets with Adobe Experience Manager as a Cloud service
description: Learn how to manage content with Adobe Experience Manager as a Cloud service
badge: label="Limited Availability"
---
# Manage templates with [!DNL Adobe Experience Manager as a Cloud service]{#aem-assets}

## Get started with [!DNL Adobe Experience Manager as a Cloud service]{#create-aem}

The integration of the Adobe Campaign Web interface with Adobe Experience Manager facilitates the streamlined management of email delivery content and forms directly within the Adobe Experience Manager platform.

![](assets/do-not-localize/book.png)[Learn more on Adobe Experience Manager as a Cloud service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## Create a template in [!DNL Adobe Experience Manager as a Cloud service]{#create-aem-template}

1. Navigate to your [!DNL Adobe Experience Manager] author instance and click Adobe Experience at the upper left corner of the page. Choose **[!UICONTROL Sites]** from the menu.

1. Access **[!UICONTROL Campaigns > Name of your brand > Main Area > Name of your page]**.

1. Click **[!UICONTROL Create]** and select **[!UICONTROL Page]** from the dropdown menu.

    ![](assets/aem_1.png)

1. Select the **[!UICONTROL Adobe Campaign Email]** template and name your newsletter.

    ![](assets/aem_2.png)

1. Customize your email content by adding components, such as personalization fields from Adobe Campaign.. [Learn more](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. Once your email is ready, navigate to the **[!UICONTROL Page information]** menu and click **[!UICONTROL Start workflow]**.

    ![](assets/aem_3.png)

1. From the first drop-down, select **[!UICONTROL Approve Adobe Campaign]** as workflow model and click **[!UICONTROL Start workflow]**.

1. A disclaimer will appear at the top of your page stating, `This page is subject to the workflow Approve for Adobe Campaign`. Click **[!UICONTROL Complete]** next to the disclaimer to confirm the review and click **[!UICONTROL Ok]**.

    ![](assets/aem_4.png)

1. Click **[!UICONTROL Complete]** again and select **[!UICONTROL Newsletter approval]** in the **[!UICONTROL Next Step]** drop-down.

Your newsletter is now ready and synchronized in Adobe Campaign.

## Import an Adobe Experience Manager  as a Cloud service template{#aem-templates-perso}

Once the Experience Manager template is available in Adobe Campaign Web as a content template, you can identify and incorporate the necessary content for the email, including personalization.

1. In Campaign Web, from the **[!UICONTROL Deliveries]** menu, click **[!UICONTROL Create delivery]**.

1. In the email template window, select the built-in **[!UICONTROL Email delivery with AEM content]** template.

    ![](assets/aem_5.png)

1. Enter a **[!UICONTROL Label]** for the delivery and configure additional options based on your needs:

    * **[!UICONTROL Internal name]**: assign a unique identifier to the delivery.

    * **[!UICONTROL Folder]**: store the delivery in a specific folder.

    * **[!UICONTROL Delivery code]**: use this field to organize your deliveries based on your own naming convention.

    * **[!UICONTROL Description]**: specify a description for the delivery.

    * **[!UICONTROL Nature]**: specify the nature of the email for classification purposes.

1. Define an **[!UICONTROL Audience]** to your email. [Learn more](../email/create-email.md#define-audience)

1. Click **[!UICONTROL Edit content]**.

1. From the **[!UICONTROL Edit content]** menu, click **[!UICONTROL Select AEM content]**.

    ![](assets/aem_6.png)

1. Browse through your AEM template and select the one to import to Campaign Web.

    ![](assets/aem_8.png)

1. If changes are made to your templates directly in Adobe Experience Manager, simply select **[!UICONTROL Refresh AEM content]** to have the latest version of your template.

1. To remove linkage between Experience Manager and Campaign or to further personalize your Experience Manager template in the Email designer, click **[!UICONTROL Unlink AEM content]**.

    ![](assets/aem_9.png)

1. If you added personalized content to your Experience Manager template, click **[!UICONTROL Simulate Content]** to preview how it will appear in the message using test profiles. 

    [Learn more on preview and test profiles](../preview-test/preview-content.md)

1. When viewing the message preview, any personalized elements are automatically replaced with the corresponding data from the selected test profile. 

    If needed, additional test profiles can be added through the **[!UICONTROL Manage test profiles]** button.

Your delivery is now ready to be sent. 
