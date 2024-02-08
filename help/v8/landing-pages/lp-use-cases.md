---
solution: Journey Optimizer
product: journey optimizer
title: Landing page use cases
description: Discover the most common use cases with landing pages in Journey Optimizer
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: landing, landing page, use case
exl-id: 8c00d783-54a3-45d9-bd8f-4dc58804d922
---
# How to use a landing page {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="Copy URL with caution"
>abstract="To fully test or leverage your landing page, you cannot copy-paste this link directly into a web browser or into your deliveries. Instead, use the **Simulate content** function to test it, and follow the steps described in documentation to make proper use of your landing page."

To make proper use of your landing page, you should reference it as a link in a delivery using the dedicated option.

>[!CAUTION]
>
>To fully leverage your landing page, you cannot copy-paste the link displayed in the published delivery dashboard directly into your deliveries or into a web page.

In the [!DNL Adobe Campaign Web] inferface, four out-of-the-box templates allow you to implement different use cases. However, the main steps remain the same and are detailed below.

1. [Create a landing page](create-lp.md#create-landing-page) and select the template of your choice, according to your use case:

    * [Acquisition](#lp-acquisition)
    * [Subscription](#lp-subscription)
    * [Unsubscription](#lp-unsubscription)
    * [Denylist](#lp-denylist)

1. Define the landing page properties and settings.

    ![](assets/lp-uc-properties.png)

1. According to your case, select the **[!UICONTROL Acquisition]**, **[!UICONTROL Subscription]**, **[!UICONTROL Unsubscription]** or **[!UICONTROL Denylist]** page.

1. The content of the page is displayed. Select the part corresponding to the landing page form.

    ![](assets/lp-uc-form.png)

1. Make as many other updates to the landing page labels and fields as needed. Edit the rest of your content as you want, save your changes and close.

1. Follow the steps detailed below for each use case.

1. Edit the **[!UICONTROL Confirmation]** page as needed, as well as the **[!UICONTROL Error]** and **[!UICONTROL Expiration]** pages. It will be displayed to your recipients once they submit the registration form.

    ![](assets/lp-uc-confirmation-page.png)

1. Test and [publish](create-lp.md#publish-landing-page) your landing page.

1. Create an [email](../email/create-email.md) delivery to drive traffic to the landing page.

1. [Insert a link](../email/message-tracking.md#insert-links) into your message content. Select **[!UICONTROL Landing page]** as the **[!UICONTROL Link type]** and choose the [landing page](create-lp.md#configure-primary-page) that you created.

    ![](assets/lp_subscription-uc-link.png)

    >[!NOTE]
    >
    >To be able to send your message, make sure the landing page you select is not expired yet. Learn how to update the expiry date [in this section](create-lp.md#create-landing-page).

Once they receive the email, if your recipients click the link to the landing page, and submit the landing page form, they will be directed to the confirmation page and any other action defined in your landing page will be applied (for example, users will be subscribed to your service, or will not receive any more communications from you).

Below are some examples of how you can use [!DNL Adobe Campaign] landing pages to have your customers opt in/out from receiving some or all of your communications.

## Profile acquisition {#lp-acquisition}

1. [Create a landing page](create-lp.md#create-landing-page). Select the **[!UICONTROL Acquisition]** template.

1. Define the landing page properties and settings.

    ![](assets/lp-uc-properties.png)

1. Select the **[!UICONTROL Acquisition]** page to edit its content.

1. The content of the page is displayed. Select the part corresponding to the landing page form.

## Subscription to a service {#lp-subscription}

One of the most common use cases consists in inviting your customers to [subscribe to a service](../audience/manage-services.md) (such as a newsletter or an event) through a landing page. Follow the steps below.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Start by creating a confirmation template for users subscribing to your event, so that you can select it easily when creating the service. [Learn more](../audience/manage-services.md#create-confirmation-message)

    ![](assets/lp-uc-confirmation-email.png)

1. Create a subscription service, which will store the registered users to your event. [Learn how to create a service](../audience/manage-services.md)

1. Select the template that you created as the confirmation email the users will receive upon subscribing.

    ![](assets/lp-uc-subscription-service.png)

1. [Create a landing page](create-lp.md#create-landing-page) to enable your recipients to register for your event. Select the **[!UICONTROL Subscription]** template.

    <!--![](assets/lp-uc-subscription-template.png)-->

1. Define the landing page properties and settings.

    <!--![](assets/lp-uc-properties.png)-->

1. Select the **[!UICONTROL Subscription]** page to edit its content.

    ![](assets/lp-uc-subscription-page-edit.png)

1. The content of the page is displayed. Select the part corresponding to the landing page form and expand the **[!UICONTROL Checkbox 1]** section.

    In the **[!UICONTROL Subscriptions & services]** fields, select the service that you created for your event. Leave the **[!UICONTROL Subscribe if checked]** option enabled.

    ![](assets/lp-uc-subscription-checkbox-1.png)

1. You can add an additional checkbox to offer subscription to your newsletter for example.

<!--

1. You can also update the profiles who register for your event for the email channel. Expand the **[!UICONTROL Call to action]** section and select Additional updates.

    ![](assets/lp-uc-subscription-call-to-action.png)-->

1. Make as many other updates to the landing page labels and fields as needed. Edit the rest of your content as you want, save your changes and close.

1. Edit the **[!UICONTROL Confirmation]** page as needed, as well as the **[!UICONTROL Error]** and **[!UICONTROL Expiration]** pages. It will be displayed to your recipients once they submit the registration form.

    ![](assets/lp-uc-confirmation-page.png)

1. Test and [publish](create-lp.md#publish-landing-page) your landing page.

1. Create an **Email** delivery to drive traffic to the registration landing page. Design the email to announce that registration is now open for your event.

1. [Insert a link](../email/message-tracking.md#insert-links) into your message content. Select **[!UICONTROL Landing page]** as the **[!UICONTROL Link type]** and choose the [landing page](create-lp.md#configure-primary-page) that you created for registration.

    ![](assets/lp_subscription-uc-link.png)

    >[!NOTE]
    >
    >To be able to send your message, make sure the landing page you select is not expired yet. Learn how to update the expiry date [in this section](create-lp.md#create-landing-page).

Once they receive the email, if your recipients click the link to the landing page, and submit the landing page form, they will be directed to the confirmation page and they will be added to the subscription list.

## Unsubscription {#lp-unsubscription}

1. [Create a landing page](create-lp.md#create-landing-page). Select the **[!UICONTROL Unsubscription]** template.

1. Define the landing page properties and settings.

1. Select the **[!UICONTROL Unsubscription]** page to edit its content.

1. The content of the page is displayed. Select the part corresponding to the landing page form.

## Setting up opt-out landing pages {#lp-denylist}

Providing the capability to recipients to unsubscribe from receiving communications from a brand is a legal requirement. Learn more about the applicable legislation in the [Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/privacy/regulations/overview.html#regulations){target="_blank"}.

Therefore, you must always include an **unsubscribe link** in every email sent out to recipients:

* Upon clicking this link, the recipients will be directed to a landing page including a button to confirm opting out.
* Upon clicking the opt-out button, the profile data will be updated with this information.

You can set up a **[!UICONTROL Denylist]** landing page that will enable users to opt out from all deliveries.

To give users the ability to opt out from all deliveries, you have to create and publish a **[!UICONTROL Denylist]** landing page.

Once a user clicks on the landing page link, the **[!UICONTROL No longer contact (by any channel)]** option in the profile is automatically selected.

![](assets/blocklisting_allchannels.png)

define an **[!UICONTROL Opt-out]** checkbox and choose to update **[!UICONTROL Channel (email)]**: the profile that checks the opt-out box on your landing page will be opted out from all your communications.

Once the message is received, if a recipient clicks the unsubscribe link in the email, your landing page is displayed.

![](assets/lp_opt-out-submit-form.png)

If the recipient checks the box and submits the form:

* The opted-out recipient is redirected to the confirmation message screen.

* The profile data is updated and will not receive communications from your brand unless subscribed again.

To check that the corresponding profile's choice has been updated, go to Profiles and select the profile.







