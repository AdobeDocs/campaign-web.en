---
title: Work with recipients & audiences
description: Learn how to work with recipients Campaign Web
badge: label="Beta"
---
# Work with recipients & audiences {#about-recipients}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360 view of your recipients"
>abstract="Create new recipients, and monitor them through powerful reports and tools. Access your recipient's attributes, interactions and logs. Use the filtering options to browse the recipient list, edit and update their profile."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="See release notes"


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profiles"
>abstract="A profile is an individual which is targeted to receive messages sent by Adobe Campaign. In Adobe Campaign, recipients are the default profiles targeted for sending deliveries (emails, SMS). From this list, you can view the recipient's profile, based on your permissions. Use the filtering options to browse this list. You can edit and update a small set of your recipient's attributes."

A recipient is a profile which is targeted to receive messages sent by Adobe Campaign. In Adobe Campaign, recipients are the default profiles targeted for sending deliveries (emails, SMS, etc.). Recipient data stored in the database enable you create audiences that will receive any given delivery, and to add personalization data in your delivery contents. Other types of profiles are stored in the database. They are designed for different uses: for example, seed profiles are made to test your deliveries before they are sent to the final audience.

Recipients can only be added from Campaign client console. However, they are visible in Campaign web, from the **Recipients** entry of the left navigation rail. You can also edit the recipient's attributes from that screen.

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

In addition, you can manage the subscription and unsubscription of your recipients to services such as newsletters. Learn how to work with subscription services in [this page](manage-services.md)

You can build workflows to deduplicate, enrich, combine profiles, and build audiences. Learn more in [this section](../workflows/gs-workflows.md).
