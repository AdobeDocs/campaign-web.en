---
audience: end-user
title: Edit the email content
description: Learn how to edit the email content in Campaign Web UI
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha" type="Positive"
---
# Edit the email content {#configure-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Create the email content"
>abstract="With this section, you can create the content for your email and use the Email Designer to give it a polished look."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Email parameters"
>abstract="The From Name and From Email values are defined in the email template. The Subject Line can be personalized using the expression editor."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Email attachment"
>abstract="Select one or multiples files to insert in your message."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Tracking options"
>abstract="By default, tracking is enabled for the delivery. You can disable this option from here."

To start creating the content of an email, click the **[!UICONTROL Edit content]** button from the [email creation](../email/create-email.md) screen.

![](assets/email-edit-content.png)

The screen that opens allows you to define basic details, perform some additional actions such as adding attachments or setting up offers, and access the Email Designer to build your content.

![](assets/email-edit-content-dashboard.png)

The steps to edit the content of your email are as follows:

1. In the **[!UICONTROL From name]** field, use a name that is easily identifiable by the recipients, such as your brand's name, to increase the opening rate of your deliveries.

1. Define the email **[!UICONTROL Subject line]**. To do this, type your subject directly into the dedicated field, or open the Expression Editor to define to add personalization using various attributes and content blocks or offers. [Learn how to personalize content](../personalization/personalize.md)
    To further improve the recipient's experience, you can add a person's name, for example "Emma from Megastore".

1. In the **[!UICONTROL From email]** address field, make sure the address domain is the same as the subdomain that you delegated to Adobe.

    You can change the part preceding the '@', but not the domain address.

    <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. Define the email **[!UICONTROL Subject line]**. Type your subject directly into the dedicated field, or open the Expression Editor to add personalization using various attributes and content blocks or offers. [Learn how to personalize content](../personalization/personalize.md)

1. If you want to attach a file to the email, click the **[!UICONTROL Add attachment]** button then select one or multiple file(s).
    
    >[!NOTE]
    >
    >    To avoid performance issue, it is recommended not to include more than one attachment per email.

    <!--limitation on size + number of files?-->

1. If you want to send offers with your email, select them using the **[!UICONTROL Set up offers]** button.

    You are then able to insert them into the email using personalization fields. [Learn how to send offers](offers.md)

1. Click the **[!UICONTROL Edit email body]** button to structure and design the content of the email. Additional information on how to design email content are available in these sections:

    * [Learn how to design emails](create-email-content.md)
    * [Style your content](get-started-email-style.md)

1. By default, tracking is enabled for the delivery. You can disable this option from the **[!UICONTROL Optional features]** section. [Learn how to add links and manage tracking](message-tracking.md)

1. Once the content of your email has been defined, use the **[!UICONTROL Simulate content]** button to check how it displays before sending it. [Learn how to preview and test your email](../preview-test/preview-test.md)
