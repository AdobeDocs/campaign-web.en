---
audience: end-user
title: Create your first email
description: Campaign v8 Web documentation
---
# Send your first email {#first-email}


This use case presents how to create your first email 

In this example, we will schedule the sending of an email on a specific date to silver and gold loyalty customers. This email will be designed using a predefined HTML template from a ZIP file and will include personalization using profile's attributes.

![](assets/delivery-list.png)

## Create the email {#create-email}

1. Create a new delivery from the **[!UICONTROL Deliveries]** menu.
1. Select the **[!UICONTROL Email]** channel and the template to use then click **[!UICONTROL Create]**.

    >[!NOTE]
    >
    >info on templates. check info in V7 doc

    ![](assets/channel-template.png)

1. Provide a label for the delivery and configure additional options depending on your needs:

    * Internal name: 
    * Folder: 
    * Delivery code: 
    * Description: 
    * Nature: 
    
    check which settings are defined in the template and mention them(description? folder?, nature?)

    ![](assets/email-properties.png)

    >[!NOTE]
    >
    >info on delivery settings button + link to doc

## Create the email content {#create-content}

1. Click the **[!UICONTROL Edit content]** button to start creating the content of your email. 

   This screen allows you to configure the email content and design it using the Email Designer.

    ![](assets/edit-content.png)

    >[!NOTE]
    >
    >The From name and From email information are predefined in the selected email template.
    >
    >By default, email tracking is enabled for opens and clicks. To disable these options, unselect them from the Optional features section.

1. Specify the subject of your email using the Expression Editor. [Learn how to personalize your content](../personalization/personalize.md)

    In this example, we want to personalize the subject line using the profiles' first name.

    ![](assets/subject-line.png)

1. Add an attached file to your email if necessary. [Learn how to edit email content]()

1. Click the **[!UICONTROL Edit email body]** button to create and design the content of your email.

    Choose the method to use to create your email content. In this example, we want to import an existing HTML content.

    ![](assets/import-html.png)

1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)

1. Once your content has been imported, it displays in the Email Designer, allowing you to edit it if needed and to add personalization.

    In this example, we want to add personalization in the email title. To do this, select the component block then click **[!UICONTROL Add Personalization]**.

    ![](assets/add-perso.png)

1. Once your content is ready, save it then click the arrow to go back to the email creation screen.

    ![](assets/save-content.png)

## Define the audience {#define-audience}

1. Click the **[!UICONTROL Select audience]** button then choose an existing audience or create a new one.

    In this example, we want to use an existing audience targeting customers belonging to the silver and gold loyalty points levels.

    ![](assets/create-audience.png)

    >[!NOTE]
    >
    >Audiences available in the list originate either from your Campaign V8 instance or from Adobe Experience Platform if the Destination / Sources intgeration has been implemented on your instance. Learn how to select the email audience 

1. Once your audience has been selected, you can edit the rules if necessary. You can also set a control group in order to xxxxx

## Schedule the sending {#schedule}

xxxx


<!--
no Schedule -> send immediately
or schedule, date, hour, confirmation
-->

## Preview and test the email {#preview-test}

1. Preview test and send + ref to preview test send section

## Prepare and send {#prepare-send}

1. Monitor + ref to monitor section

## Access reports {#reports}

1. access deliver reports

