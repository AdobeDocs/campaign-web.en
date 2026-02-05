---
audience: end-user
title: Create multilingual emails with Adobe Experience Manager
description: Learn how to create multilingual email deliveries using Adobe Experience Manager language copies in Campaign Web.
feature: Email
topic: Content Management
role: User
level: Intermediate
---

# Create multilingual emails with Adobe Experience Manager {#aem-multilingual}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Experience Manager live and langage copies"
>abstract="You can now access Adobe Experience Manager language and live copies directly in Campaign. Real-time content refresh eliminates manual synchronization for streamlined multi-language workflows."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"

The Adobe Experience Manager integration enables you to create multilingual email deliveries using Adobe Experience Manager language copies. This allows you to manage content variants in different languages and deliver personalized emails based on recipient language preferences.

## Prerequisites {#prerequisites}

Before creating a multilingual email delivery, ensure you have:

* Access to an Adobe Experience Manager instance configured for Adobe Campaign Web interface integration.
* Adobe Experience Manager content with language copies already created and approved. Learn more about Language Copy Wizard in [Adobe Experience Manager documentation](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard)
* Email delivery template configured to receive Adobe Experience Manager content. Refer to the steps detailed in the [Enable multilingual mode](#enable-multilingual) section.

## Create your multilingual delivery

To create a multilingual email delivery, you first need to enable the multilingual option in your delivery settings. The system automatically detects available language copies and lets you choose which ones to add.

### Enable multilingual mode {#enable-multilingual}

Create a new delivery and enable the multilingual option in the advanced settings.

1. From the **[!UICONTROL Deliveries]** menu, click **[!UICONTROL Create delivery]**.

    ![](assets/lg-copy-1.png)

1. Select the **[!UICONTROL Email delivery with AEM content]** template and click **[!UICONTROL Create delivery]**.

    ![](assets/lg-copy-2.png)

1. Enter a label for the delivery and configure your audience. [Learn more](../email/create-email.md)

1. Access your delivery **[!UICONTROL Settings]**, then navigate to the **[!UICONTROL Advanced]** section.

1. Enable the **[!UICONTROL Enable AEM multilingual]** option.

    ![](assets/lg-copy-3.png)

1. Make sure that:

   * **[!UICONTROL Content editing mode]** is set to **[!UICONTROL AEM]**.
   * The correct Adobe Experience Manager **[!UICONTROL External account]** is selected.

1. Click **[!UICONTROL Save and close]**.

### Create content variants {#create-variants}

Select your Adobe Experience Manager content and choose which language variants to include in the delivery.

1. Click **[!UICONTROL Edit content]**.

1. Select **[!UICONTROL Create content variant]**.

    ![](assets/lg-copy-4.png)

1. Select your Adobe Experience Manager content from the list. 

    ![](assets/lg-copy-5.png)

1. The system detects all language copies associated with the selected content (parent-child relationship), e.g. if your Adobe Experience Manager content has variants in French, German, and Italian, all variants are available for selection.

    Select the language variants you want to include in your delivery.

    ![](assets/lg-copy-6.png)

1. Click **[!UICONTROL Save]**.

1. Review your language variants in the content editor. You can now [manage each variant individually](#manage-variants) or proceed with [sending the delivery](../monitor/prepare-send.md).

    ![](assets/lg-copy-7.png)

## Manage language variants {#manage-variants}

After creating content variants, you can manage them directly in the delivery:

1. To set a default language, access the advanced menu for your chosen variant and select **[!UICONTROL Set as default]**. The default language is used when a profile's language preference is not set or does not match any available variant.

    Click **[!UICONTROL Delete]** to remove any variant from your delivery.

    ![](assets/lg-copy-8.png)

1. From the Content variants advanced menu, click **[!UICONTROL Manage locales]** to add other Locales to your delivery. 

    ![](assets/lg-copy-9.png)

1. Select additional language copies to include more variants and click **[!UICONTROL Save]**.

    ![](assets/lg-copy-11.png)

1. If content is updated in Adobe Experience Manager, click **[!UICONTROL Refresh AEM content]** to synchronize all variants with the latest version.

    ![](assets/lg-copy-10.png)

1. Click **[!UICONTROL Unlink AEM content]** if you want to edit content directly in Campaign or break the link with Adobe Experience Manager.

   >[!CAUTION]
   >
   >After unlinking, you cannot refresh content from Adobe Experience Manager or create new variants. The content becomes independent from Adobe Experience Manager.


