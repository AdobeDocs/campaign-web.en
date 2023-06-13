---
title: Personalize your content in Campaign
description: Learn how to personalize your content in Adobe Campaign web UI
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" 
---

# Built-in content blocks {#ootb-content-blocks}

Adobe Campaign offers a list of pre-configured content blocks. These content blocks are dynamic, personalized and have a specific rendering that you can insert into your deliveries. For example, you can add a logo, a greeting message, or a link to a mirror page. 

To add a content block into a delivery follow these steps:

1. Open a delivery and edit its content.

1. Locate the field where you want to add a content block and click the **[!UICONTROL Open personalization dialog]** icon to open the expression editor.

    ![](assets/content-block-access.png){width="800" align="center"}

1. In the expression editor, browse to the **[!UICONTROL Content blocks]** left menu.

1. To add a content block, place your cursor at the desired location within your content and click the '+' button to insert it.

    ![](assets/content-blocks.png){width="800" align="center"}

Built-in content blocks are:

* **[!UICONTROL Approval of Purl personalization]**
* **[!UICONTROL Default opt-out banner]**
* **[!UICONTROL Enabled by Adobe Campaign]**: inserts the "Enabled by Adobe Campaign" logo.
* **[!UICONTROL Facebook pre-entering]**
* **[!UICONTROL Formatting function for proper nouns]**: generates the **[!UICONTROL toSmartCase]** Javascript function, which changes the first letter of each word to uppercase. 
* **[!UICONTROL Greetings]**: inserts greetings with the recipient's full name, followed by a comma. Example: "Hello John Doe,".
* **[!UICONTROL Insert Logo]**: inserts a logo which is is defined in the instance settings.
* **[!UICONTROL Link to mirror page]**: inserts a link to the [mirror page](../content/mirror-page.md). Default format is: "If you are unable to view this message correctly, click here".
* **[!UICONTROL Mirror page URL]**: inserts the mirror page URL, enabling Delivery Designers to check the link.
* **[!UICONTROL Notification style]**
* **[!UICONTROL Offer acceptance URL in unitary mode]**: inserts an URL enabling to set an offer to **[!UICONTROL Accepted]**. (This block is available if the Interaction module is enabled)
* **[!UICONTROL Registration confirmation]**: inserts a link enabling to confirm subscription.
* **[!UICONTROL Registration link]**: inserts a subscription link. This link is defined in the instance settings. The default content is: "To register click here."
* **[!UICONTROL Registration link (with referrer)]**: inserts a subscription link, enabling to identify the visitor and delivery. This link is defined in the instance settings.
* **[!UICONTROL Registration page URL]**: inserts a subscription URL
* Social network sharing links
* **[!UICONTROL Style of content emails]** and **[!UICONTROL Notification style]**: generate code which format an email with predefined HTML styles. 
* **[!UICONTROL Unsubscription link]**: inserts a link enabling to unsubscribe from all deliveries (denylist). The default associated content is: "You are receiving this message because you have been in contact with ***your organization name*** or an affiliate. To no longer receive messages from ***your organization name*** click here."

>[!NOTE]
>
>You can define new blocks from Adobe Campaign v8 console that enables you to optimize your deliveries personalization. Learn more in [Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}.

