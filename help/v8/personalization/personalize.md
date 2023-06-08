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

Personalization can be added to any delivery using the expression editor, which is accessible  in every fields with the **[!UICONTROL Open personalization dialog]** icon, such as the subject line field, or email links and text/button content components. [Learn where to add dynamic content](gs-personalization.md/#access)

## Personalization syntax {#syntax}

A personalization tag always uses the following syntax: `<%=table.field%>`. For example, to insert the name of the recipient, stored in the recipient table, the personalization tag uses the <%= recipient.lastName %> syntax.

When a delivery is prepared, these tags are automatically interpreted by Adobe Campaign and replaced by the value of the field for a given recipient. The physical replacement can then be viewed when simulating your content.

## Add personalization tags {#add}

To add personalization tags into a delivery, open the expression editor using the **[!UICONTROL Open personalization dialog]** icon that is accessible from text-type editing fields, such as the subject line or the SMS body. [Learn where to add dynamic content](gs-personalization.md/#access)

![](assets/perso-access.png)

The expression editor displays. Personalization fields are organized into three menus, located to the left of the screen. These menus give access to all fields available in the Adobe Campaign database.

![](assets/perso-insert-field.png)

|Menu | Description | 
|-----|------------|
|![](assets/do-not-localize/perso-recipients-menu.png) | The **[!UICONTROL Recipient]** menu lists all the fields defined in the recipients table, such as the recipients' name, age, or address. | 
|![](assets/do-not-localize/perso-message-menu.png)| The **[!UICONTROL Message]** menu lists all the fields related to the delivery logs, i.e. all messages sent to recipients or devices across all channelsk, such as the date of the last event with a a given recipient |
|![](assets/do-not-localize/perso-delivery-menu.png)| The **[!UICONTROL Delivery]** menu lists all the fields related to the parameters required for performing deliveries such as the delivery channel, label, etc.|

>[!NOTE]
>
>By default, each menu shows all fields within the selected table (Recipients, / Message / Delivery). If you want to include fields from tables linked to the selected table, enable the **[!UICONTROL Display advanced attributes]** option located below the list.

To add a personalization field, place your cursor at the desired location within your content and click the + button to insert it.

Once your content is ready, you can save it and test the rendering of the personalization by simulating your content. In the example below, we are personalizing an SMS message with the targeted profiles' first names.

*Add the personalization tag in the message content*

![](assets/perso-preview1.png)

*Simulate the rendering of the personalization for a given test profile*

![](assets/perso-preview2.png)
