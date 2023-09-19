---
title: Work with recipients & audiences
description: Learn how to work with recipients Campaign Web
badge: label="Beta" 
---

# Work with recipients & audiences {#about-recipients}

## Recipients {#recipients}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Recipients"
>abstract="A recipient is a profile which is targeted to receive messages sent by Adobe Campaign. In Adobe Campaign, recipients are the default profiles targeted for sending deliveries (emails, SMS). From this list, you can view the recipient's profile, based on your permissions. Use the filtering options to browse this list. You can edit and update a small set of your recipient's attributes."

A recipient is a profile which is targeted to receive messages sent by Adobe Campaign. In Adobe Campaign, recipients are the default profiles targeted for sending deliveries (emails, SMS, etc.). Recipient data stored in the database enable you create audiences that will receive any given delivery, and to add personalization data in your delivery contents. Other types of profiles are stored in the database. They are designed for different uses: for example, seed profiles are made to test your deliveries before they are sent to the final audience.

Recipients can only be added from Campaign client console. However, they are visible in Campaign web, from the **Recipients** entry of the left navigation rail.

To edit the recipient's data, click the three dots next to its name and choose **Edit...**.

![Edit a recipient profile](assets/recipient-edit.png)

You can update a limited set of attributes, which are: its first name, last name, email, and phone number.

![Update a recipient profile](assets/recipient-update.png)

>[!NOTE]
>
>This limited profile editing form is provided for Beta program testing only. It will be improved in the future release. It allows the user to quickly add an email address and a phone number to any profile so that he/she can test the email and SMS channels and receive the messages sent.

You can filter the recipients using the search field, from the **Show filters** button.

You can also access recipients from the **Explorer** view, browse and create folders and subfolders, and check associated permissions.

![Recipient list from the Explorer view](assets/recipients-from-explorer.png)

>[!NOTE]
>
>Depending on your permissions, you might not have access to the full list of recipients stored in the database. Learn more about permissions in [this section](../get-started/permissions.md).

In addition, you can manage the subscription and unsubscription of your recipients to services such as newsletters. [Learn how to work with subscription services](create-service.md)

## Audiences {#audiences}

The audience is the main target of your delivery: the recipients who receive the messages. The type of audience depends on the target mapping defined in the delivery template. [Learn what is a delivery template](../msg/delivery-template.md). 

To define the population of an audience, you can:

* [Create new audiences](create-audience.md) from the **[!UICONTROL Audiences]** menu,
* [Select an existing audience](add-audience.md) created as a list in the client console,
* [Select an Adobe Experience Platform audience](aep-audience.md),
* [Build a new audience](segment-builder.md) with the rule builder by defining and combining filtering criteria,
* [Use an audience from an external file](file-audience.md). This option is only available for standalone email deliveries, and cannot be used in campaign deliveries.

When targeting an audience, you can also define **control groups** to avoid sending messages to a portion of your audience, and measure the impact of your campaigns. [Learn how to set a control group](control-group.md)

>[!NOTE]
>
>When sending messages in the context of a campaign workflow, the audience is defined in a specific **Build audience** workflow activity. In this context, you cannot load an audience from a file for an email delivery, and the audience is defined only in this dedicated activity. Learn how to define the audience of your delivery in a campaign workflow [in this section](../workflows/activities/build-audience.md)
