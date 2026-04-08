---
audience: end-user
title: Configure the WhatsApp channel
description: Learn how to configure your environment to send WhatsApp messages using the Adobe Campaign Web user interface
feature: Whatsapp, Channel Configuration
role: Admin
level: Intermediate
exl-id: d1f40cd8-f311-4df6-b401-8858095cef3e
---
# Configure the WhatsApp channel {#whatsapp-config}

Before sending WhatsApp messages, complete setup in the **Adobe Campaign Web user interface** and connect your Meta WhatsApp assets. Typical sequence:

1. [Create your WhatsApp API credentials](#WhatsApp-credentials)
1. [Create your WhatsApp webhooks](#WhatsApp-webhook)
1. [Create your WhatsApp channel configuration](#WhatsApp-configuration)

An administrator with access to **[!UICONTROL Administration]** should perform these steps. [Learn more about permissions](../get-started/permissions.md).

## Create WhatsApp API credentials {#whatsapp-credentials}

1. In the Adobe Campaign Web user interface, browse the left rail to **[!UICONTROL Administration]** `>` **[!UICONTROL Channels]** and select **[!UICONTROL API Credentials]**. Click **[!UICONTROL Create new API credentials]**.

1. Configure your API credentials:

    * **API Token**: Enter your API token. Learn more in [Meta Documentation](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
    * **Business Account ID**: Enter the unique number for your business portfolio. Learn more in [Meta Documentation](https://www.facebook.com/business/help/1181250022022158?id=180505742745347).

    ![](assets/whatsapp-api.png)

1. Click **[!UICONTROL Continue]**.

1. Choose the **WhatsApp Business Account** to connect to these API credentials.

    ![](assets/whatsapp-api-2.png)

1. Select the **Sender name** used to send your WhatsApp messages.

1. Phone number settings are filled in automatically:

    * **Quality Rating**: Reflects customer feedback on messages sent in the past 24 hours.
        * Green: High quality
        * Yellow: Medium quality
        * Red: Low quality

        Learn more about [Quality rating](https://www.facebook.com/business/help/766346674749731#)

    * **Throughput**: Rate at which your phone number can send messages.

1. Click **[!UICONTROL Submit]** when API credential setup is complete.

Continue with webhooks below.

## Create Webhook {#WhatsApp-webhook}

>[!CONTEXTUALHELP]
>id="ajo_admin_whatsapp_webhook_inbound_keyword_category"
>title="Inbound keyword category"
>abstract="<b>Opt-In</b>: sends your defined auto-response when a user subscribes. <br/><b>Opt-Out</b>: sends your defined auto-response when a user unsubscribes. <br/><b>Help</b>:  sends your defined auto-response when a user requests help or support. <br/><b>Default</b>: sends your fallback auto-response when no keywords match.."

>[!CONTEXTUALHELP]
>id="ajo_admin_whatsapp_webhook_inbound_keyword"
>title="Enter your keywords"
>abstract="You can define keywords to trigger specific auto-responses based on what users text. Keywords are not case-sensitive, e.g., stop and STOP are treated the same."

>[!CONTEXTUALHELP]
>id="ajo_admin_whatsapp_webhook_webhook_url"
>title="Callback URL"
>abstract="The validation request and webhook notifications for this object are sent to the specified URL."

>[!CONTEXTUALHELP]
>id="ajo_admin_whatsapp_webhook_verify_token"
>title="Verify Token"
>abstract="The token that Meta echoes back to confirm and verify the callback URL during the verification process."

>[!NOTE]
>
>Without specified opt-in or opt-out keywords, standard consent messages are not enabled.

After API credentials are created, configure webhooks to:

* **Capture inbound responses** for opt-in and opt-out handling
* **Receive delivery reports** such as read receipts (where available) and delivery status
* **Surface tracking events** for reporting and datasets connected to your Adobe Campaign instance

Webhooks connect Meta's WhatsApp Business Platform to Adobe Campaign so you receive notifications about message events and user interactions.

1. In the Adobe Campaign Web user interface, navigate the left rail to **[!UICONTROL Administration]** `>` **[!UICONTROL Channels]**, open **[!UICONTROL WhatsApp Webhooks]** under **[!UICONTROL WhatsApp settings]**, and click **[!UICONTROL Create Webhook]**.

    ![](assets/webhook-1.png)

1. Enter a **[!UICONTROL Name]** for your webhook.

1. From **[!UICONTROL Select configuration]**, choose the [API credentials](#whatsapp-credentials) you created.

    ![](assets/webhook-2.png)

1. Choose **[!UICONTROL Inbound keyword category]**:

    * **[!UICONTROL Opt-in Keywords]**
    * **[!UICONTROL Opt-out Keywords]**
    * **[!UICONTROL Help Keywords]**
    * **[!UICONTROL Default]** — fallback when no other keyword matches; also used to enable tracking-related events where configured.

1. Enter **[!UICONTROL Keywords]** and click ![add](assets/do-not-localize/Smock_AddCircle_18_N.svg).

    ![](assets/webhook-3.png)

1. In **[!UICONTROL Reply Message]**, enter the auto-reply or pick a predefined option.

    ![](assets/webhook-4.png)

1. Click ![add](assets/do-not-localize/Smock_AddCircle_18_N.svg) to add more **[!UICONTROL Inbound keyword]** rows if needed.

1. Click **[!UICONTROL Submit]** when webhook configuration is complete.

1. In the **[!UICONTROL Webhooks]** list, use ![bin icon](assets/do-not-localize/Smock_Delete_18_N.svg) to delete a webhook.

    ![](assets/webhook-5.png)

1. To edit a webhook and retrieve **[!UICONTROL Webhook URL]** or **[!UICONTROL Verify Token]**, select **[!UICONTROL Edit]** on that row.

1. Copy **[!UICONTROL Verify Token]** into the Meta developer console as part of webhook verification.

    For Meta-side steps, see [Meta documentation](https://developers.facebook.com/docs/graph-api/webhooks/getting-started#configure-webhooks-product).

1. Copy **[!UICONTROL Webhook URL]** from the saved **[!UICONTROL WhatsApp Webhook]** and register it in Meta.

    ![](assets/webhook-6.png)

## Create WhatsApp channel configuration {#whatsapp-configuration}

1. In the Adobe Campaign Web user interface, browse the left rail to **[!UICONTROL Administration]** > **[!UICONTROL Channels]** > **[!UICONTROL General settings]** > **[!UICONTROL Channel configurations]**. Click **[!UICONTROL Create channel configuration]**.

    ![](assets/whatsapp-config-1.png)

1. Enter a name and optional description, then pick the WhatsApp channel.

    >[!NOTE]
    >
    > Names must begin with a letter (A–Z). Use alphanumeric characters and optionally underscore `_`, dot `.`, or hyphen `-`.

1. Select **[!DNL WhatsApp]** as your channel.

    ![](assets/whatsapp-config-2.png){width=80%}

1. If your organization uses **[!UICONTROL Marketing action(s)]** for consent and suppression rules, associate the appropriate actions with this configuration so policies apply to WhatsApp sends.

1. In **[!UICONTROL WhatsApp Settings]**, select the API credential / routing configuration created earlier.

    ![](assets/whatsapp-config-3.png){width=80%}

1. Enter the **[!UICONTROL Sender Phone Number]** for outbound messages.

1. Use **[!UICONTROL WhatsApp Execution Field]** to choose which profile attribute holds the mobile number when multiple numbers exist. This aligns with how Adobe Campaign resolves the address for the delivery. [Learn more about target mappings](../administration/target-mappings.md).

    >[!NOTE]
    >
    >If you do not override execution fields here, Adobe Campaign uses default addressing rules for the channel and target mapping.

1. Click **[!UICONTROL Submit]** to confirm, or save as draft to finish later.

1. New configurations may show **[!UICONTROL Processing]** while checks run.

    >[!NOTE]
    >
    >If validation fails, open the configuration details for the error message and correct API credentials, sender, or webhook linkage.

1. When checks succeed, status becomes **[!UICONTROL Active]** and the configuration is available in delivery templates and sends.

You can now author WhatsApp deliveries in the Adobe Campaign Web user interface.

## Troubleshoot WhatsApp channel setup {#troubleshooting}

### HTTP 500 errors during API credential setup

If you see an HTTP 500 error while saving WhatsApp API credentials:

1. **Verify entitlements**: Confirm your organization is entitled to the WhatsApp channel for Adobe Campaign.

1. **Validate business account fields**: **API Token** must be a valid Meta token with required permissions; **Business Account ID** must match Meta exactly.

1. **Test credentials in Meta tools**: Confirm the token and account outside the Adobe Campaign Web user interface to isolate credential vs. product issues.

1. **Collect diagnostic detail**: If your team uses advanced logging for integrations, capture the failing request window for support.

1. **Contact support**: If entitlements and credentials are correct but the error persists, contact Adobe Customer Care or your account team.

## How-to video {#video}

The video below shows WhatsApp channel setup. Align field names with the **[!UICONTROL Administration]** screens in the Adobe Campaign Web user interface.

+++ See video

>[!VIDEO](https://video.tv.adobe.com/v/3470268/?learn=on)

+++

