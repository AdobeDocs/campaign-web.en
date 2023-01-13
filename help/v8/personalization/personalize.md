---
title: Personalize your content in Campaign
description: Learn how to personalize your content in Adobe Campaign web UI
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
---
# Personalize your content{#add-personalization}

![](../assets/do-not-localize/badge.png)

You can personalize the message content by:

* Inserting dynamic **personalization fields**

    Personalization fields are used for first-level personalization of your messages. You can select any field available in the database from the personalization editor. For a delivery, you can select any field related to the recipient, the message or the delivery. These personalization attributes can be inserted in the subject line or body of your messages.

    ![](assets/perso-subject-line.png)

    The syntax above inserts the city of the recipient in your content: <%= recipient.location.city %>.
    
* Inserting pre-defined **content blocks**
    
    Campaign comes with a set of personalization blocks which contain a specific rendering that you can insert into your deliveries. For example, you can add a logo, a greeting message, or a link to the mirror page of the message. Content blocks are available from a dedicated entry un the personalization editor.

    ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## Personalize the email subject line {#personalize-subject-line}

To add personalization in the **[!UICONTROL Subject line]** field of the message, follow the steps below:

1. Click the **Open personalization dialog** icon on the right of the **Subject line** field.
1. Enter the subject line content and select the personalization attributes to add.
1. Click Confirm to validate. The personalization attributes are added to the subject line.

![](assets/perso-subject.png)

## Personalize your email content {#personalize-emails}

To personalize the email content, open the message in the Email designer and:

1. Click inside a text block.
1. In the contextual toolbar, select **Add personalization**.

    ![](assets/perso-add-to-content.png)

1. Insert the name of the recipient in the personalization editor and confirm.

    ![](assets/perso-add-name.png)

    The personalization attribute is added to the email content. 
    
    You can simulate the content to check rendering. [Learn more](../preview-test/preview-content.md)

    ![](assets/perso-rendering.png)


## Personalize links in your emails {#personalize-links}

To personalize a **link**:

1. Select a text block or an image.
1. In the contextual toolbar, select **Add personalization**.

    ![](assets/perso-link.png)

1. Use the personalization editor to define and personalize the link.

## Personalize your offers {#personalize-offers}

You can also access the personalization editor when adding text-type content to your offers' representations.
