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

# Personalize your content {#add-personalization}

You can personalize any delivery by using the expression editor, which is accessible in fields with the **[!UICONTROL Open personalization dialog]** icon, such as the subject line, email links, and text/button content components. [Learn how to access the expression editor](gs-personalization.md/#access)

## Personalization syntax {#syntax}

Personalization tags follow a specific syntax: `<%=table.field%>`. For example, to insert the recipient's last name from the recipient table, use the `<%= recipient.lastName %>` syntax.

During the delivery preparation process, Adobe Campaign automatically interprets these tags and replaces them with the corresponding field values for each recipient. You can view the actual replacement by simulating your content.

## Add personalization tags {#add}

To add personalization tags into a delivery, follow these steps:

1. Open the expression editor using the **[!UICONTROL Open personalization dialog]** icon that is accessible from text-type editing fields, such as the subject line or the SMS body. [Learn how to access the expression editor](gs-personalization.md/#access)

    ![](assets/perso-access.png){width="800" align="center"}

1. The expression editor opens. Personalization fields available in the Adobe Campaign database are organized into several menus on the left side of the screen:

    ![](assets/perso-insert-field.png){width="800" align="center"}

    |Menu | Description | 
    |-----|------------|
    |![](assets/do-not-localize/perso-subscribers-menu.png) | The **[!UICONTROL Subscribers application]** menu lists fields related to the subscribers of an application, such as the used terminal or the operating system. *This menu is available for push notifications only* | 
    |![](assets/do-not-localize/perso-recipients-menu.png) | The **[!UICONTROL Recipient]** menu lists fields defined in the recipients table, such as recipients' names, ages, or addresses. | 
    |![](assets/do-not-localize/perso-message-menu.png)| The **[!UICONTROL Message]** menu lists fields related to the delivery logs, including all messages sent to recipients or devices across all channels, such as the date of the last event with a a given recipient |
    |![](assets/do-not-localize/perso-delivery-menu.png)| The **[!UICONTROL Delivery]** menu lists fields related to the parameters required for performing deliveries such as the delivery channel or label.|

    >[!NOTE]
    >
    >By default, each menu lists all fields within the selected table (Recipients, / Message / Delivery). If you want to include fields from tables linked to the selected table, enable the **[!UICONTROL Display advanced attributes]** option located below the list.

1. To add a personalization field, position your cursor at the desired location within your content and click the `+` button to insert it.

1. Once your content is ready, you can save it and test the rendering of the personalization by simulating your content. The example below shows the personalization of an SMS message with recipients' first names.

    ![](assets/perso-preview1.png){width="800" align="center"}

    ![](assets/perso-preview2.png){width="800" align="center"}
