---
title: Work with recipients & audiences
description: Learn how to work with recipients Campaign Web
badge: label="Beta" 
---

# Work with recipients & audiences {#about-recipients}

In Adobe Campaign, the target population of a delivery is an audience. An audience is a set of people who share similar behaviors and/or characteristics. This collection of people can either be generated, selected, or loaded [as detailed below](#audiences). In most common cases, the audience is made of profiles, which are stored as [recipients](#recipients) in Adobe Campaign. You can also work with other target mappings by changing the dimension as explained [in this section](#targeting-dimensions).

## What are recipients? {#recipients}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Recipients"
>abstract="A recipient is a profile which is targeted to receive messages sent by Adobe Campaign. In Adobe Campaign, recipients are the default profiles targeted for sending deliveries (emails, SMS). From this list, you can view the recipient's profile, based on your permissions. Use the filtering options to browse this list. You can edit and update a small set of your recipient's attributes."

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

In addition, you can manage the subscription and unsubscription of your recipients to services such as newsletters. [Learn how to work with subscription services](manage-services.md)

You can build workflows to deduplicate, enrich, combine profiles, and build audiences. Learn more in [this section](../workflows/gs-workflows.md).

## What are audiences? {#audiences}

The audience is the main target of your delivery: the recipients who receive the messages. The type of audience depends on the target mapping defined in the delivery template. [Learn what is a delivery template](../msg/delivery-template.md). 

To define the population of an audience, you can:

* [Create new audiences](create-audience.md) from the **[!UICONTROL Audiences]** menu,
* [Select an existing audience](add-audience.md) created as a list in the client console or coming from Adobe Experience Platform,
* [Build a new audience](segment-builder.md) with the rule builder by defining and combining filtering criteria,
* [Use an audience from an external file](file-audience.md). This option is only available for standalone email deliveries, and cannot be used in campaign deliveries.

When targeting an audience, you can also define **control groups** to avoid sending messages to a portion of your audience, and measure the impact of your campaigns. [Learn how to set a control group](control-group.md)

>[!NOTE]
>
>When sending messages in the context of a campaign workflow, the audience is defined in a specific **Build audience** workflow activity. In this context, you cannot load an audience from a file for an email delivery, and the audience is defined only in this dedicated activity. Learn how to define the audience of your delivery in a campaign workflow [in this section](../workflows/activities/build-audience.md)

## Targeting dimensions {#targeting-dimensions}

The targeting dimension, aka. target mapping, is the type of data that an operation is handling. It lets you define the targeted population: recipients, contract beneficiaries, operators, subscribers, etc.

The targeting dimension of a workflow is defined by the first **[!UICONTROL Build audience]** activity and is used across all further activities until the end of the workflow. For example, if you perform a query on the recipients from the database, the outbound transition will contain data of type recipient and it will be transmitted to the next activity.

Note that you can switch the targeting dimension in a workflow using a [Change dimension activity](../workflows/activities/change-dimension.md). This allows you, for example, to query the database on a specific table such as purchases or subscriptions, and then change the targeting dimension to Recipients in order send deliveries to the corresponding recipients.

By default, email and SMS delivery templates target **[!UICONTROL Recipients]**. Their target dimension therefore uses the fields of the **nms:recipient** table. For Push notifications, the default target dimension is **Subscriber applications nms:appSubscriptionRcp**, which is linked to the recipients table.

You can also use other built-in target mappings in your workflows and deliveries that are listed below: 

|  Name  | Use to | Schema  |
|---|---|---|
|  Recipients  | Deliver to recipients (built-in recipient table)  | nms:recipient  |
|  Visitors  | Deliver to visitors whose profiles have been collected via referral (viral marketing) for ex.  | mns:visitor  |
|  Subscriptions  | Deliver to recipients who are subscribed to an information service such as a newsletter | nms:subscription  |
|  Visitor subscriptions  | Deliver to visitors who are subscribed to an information service  | nms:visitorSub  |
|  Operators  | Deliver to Adobe Campaign operators  | nms:operator  |
|  External file  | Deliver via a file that contains all information needed for delivery  | No linked schema, no target entered  |
|  Subscriber applications  | Deliver to recipients who are subscribed to an application | nms:appSubscriptionRcp  |

In addition, you can create a new target mapping depending on your needs. This is performed from the client console. Learn more in [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
