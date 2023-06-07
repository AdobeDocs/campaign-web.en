---
title: Personalize your content in Campaign
description: Learn how to personalize your content in Adobe Campaign web UI
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
---

# Personalize your content{#add-personalization}

## Personalize the subject line of a message {#personalize-subject-line}

To add personalization in the **[!UICONTROL Subject line]** field of the message, follow the steps below:

1. Open a delivery and click **[!UICONTROL Edit content]**.
1. Click the **[!UICONTROL Open personalization dialog]** icon on the right of the **[!UICONTROL Subject line]** field for emails, or the **[!UICONTROL Title]** fields for push/SMS deliveries.

    ![](assets/perso-subject.png){width="600"}

1. Enter the subject line or title, and select the personalization attributes to add.

1. Click **[!UICONTROL Confirm]** to validate. The personalization attributes are added to the content.

## Personalize your email content {#personalize-emails}

To personalize the email content, open the message in the Email designer and:

1. Click inside a text block.
1. In the contextual toolbar, select **[!UICONTROL Add personalization]**.

    ![](assets/perso-add-to-content.png)

1. Insert the name of the recipient in the personalization editor and confirm.

    ![](assets/perso-add-name.png)

    The personalization attribute is added to the email content. 
    
    You can simulate the content to check rendering. [Learn more](../preview-test/preview-content.md)

    ![](assets/perso-rendering.png)

1. To add a content block to your email, apply the same steps and select a content block from the last icon:

    ![](assets/perso-insert-block.png)

1. Once inserted, the content block is added to the email content It is automatically adapted to the recipient profile when personalization is generated, at the delivery preparation step.

    ![](assets/perso-content-block-in-email.png)

## Personalize links in your emails {#personalize-links}

To personalize a **link**:

1. Select a text block or an image.
1. In the contextual toolbar, select **Insert link**.

    ![](assets/perso-link.png)

1. Enter the link label and use the **Insert link** button to personalize the link.

    ![](assets/perso-link-insert-icon.png)

1. Use the personalization editor to define and personalize the link, and confirm.

    ![](assets/perso-link-edit.png)


## Personalize your offers {#personalize-offers}

You can also access the personalization editor when adding text-type content to your offers' representations. Learn more in [this section](../content/offers.md).

