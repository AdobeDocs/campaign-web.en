---
audience: end-user
title: Send offers
description: Send offers
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
---
# Send offers {#offers-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Offers settings"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Offers Advanced Settings"
>abstract="TBC"

>[!NOTE]
>
>This documentation is under construction and frequently updated. The final version of this content will be ready in January 2023.

Adobe Campaign v8 web allows you to send with your emails offers that have been created in the console using the Interaction module. 

For more information on Interaction and how to manage an offer catalog in the console, refer to the [Campaign V8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=en)

The steps to propose offers with an email from Campaign v8 web are as follows:

1. [Configure the offers to send](#configure),
1. [Insert the offers into the email](#insert).

## Configure the offers to propose {#configure}

To select the offers to propose in your email, click the **[!UICONTROL Offers]** button from the email content edition screen.

![](assets/create-content-offers.png)

1. Select the **[!UICONTROL Offer space]** that matches your offer environment.

1. To refine the engine's choice of offers, select a specific **[!UICONTROL Offer category]** in which offers are sorted.

    If no category is specified, all the offers contained in the environment will be taken into account by the Offer engine, unless an **[!UICONTROL Offer theme]** is selected.

    >[!NOTE]
    >
    >Themes are key words defined upstream in the categories. They act as a filter and let you refine the number of offers to be presented by selecting them in a set of categories. 

1. Use the **[!UICONTROL Propositions]** field to specify the number of offers you want to insert into the email.

1. Select the **[!UICONTROL Exclude non-eligible recipients]** option if necessary.

    This option lets you activate or deactivate the exclusion of recipients for whom there are not enough eligible offers.  If this box is checked, recipients who don't have enough propositions will be excluded from the delivery. If you don't select this option, these recipients will not be excluded but they won't have the requested number of propositions.

1. If necessary, select the **[!UICONTROL Hide everything ig no offer is selected]** option.

    This option lets you choose how the message will be processed in case one of the propositions does not exist. When this box is checked, the representation of the missing proposition is not displayed and no content will appear in the message for this proposition. If the box isn't checked, the message itself is cancelled during sending and recipients will no longer receive any messages.

Once you have configured the offers to propose into your email, you can insert them into the email using the Expression Editor. [Learn how to insert offers into the email](#insert)

## Insert offers into the email {#insert}

document detailed steps

Offers are inserted using the Expression Editor

offers can be inserted:
* in the emai sublect line
* in the email body from the Email Designer
