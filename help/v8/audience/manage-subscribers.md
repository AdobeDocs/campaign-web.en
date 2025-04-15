---
audience: end-user
title: Manage the subscribers
description: Learn how to manage and deliver to the subscribers of a service in Adobe Campaign Web
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
---
# Manage the subscribers {#manage-subscribers}

Once you [created a service](manage-services.md#create-service), you can add subscribers, unsubscribe recipients, and send messages to the subscribers of that service.

Subscribers management is detailed on this page. To learn how to send messages to your subscribers, refer to [this section](../msg/send-to-subscribers.md).

## Add subscribers to your service {#add-subscribers}

To manually add subscribers, follow the steps below.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. Go to the **[!UICONTROL Subscribers]** tab, and click **[!UICONTROL Add subscribers]**.

    ![Screenshot showing the Subscribers tab in the Subscription services interface.](assets/service-subscribers-tab.png){zoomable="yes"}

1. Select the profiles you want to add from the list, and click **[!UICONTROL Confirm]**.

    ![Screenshot showing the profile selection interface for adding subscribers.](assets/service-subscribers-select-profiles.png){zoomable="yes"}

1. Click **[!UICONTROL Send]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> to have the selected recipients receive the subscription [confirmation message](manage-services.md#create-confirmation-message) that you defined when [creating the service](manage-services.md#create-service).

    ![Screenshot showing the confirmation message interface for adding subscribers.](assets/service-subscribers-confirmation-msg.png){zoomable="yes"}

    >[!NOTE]
    >
    >If you select **[!UICONTROL Cancel]**, no confirmation message is sent to the selected profiles, but they are subscribed.

The profiles added are displayed in the **[!UICONTROL Subscribers]** tab. They are now subscribed to your service.

## Remove subscribers from your service {#remove-subscribers}

### Manually unsubscribe profiles {#manual-unsubscription}

Once you [added subscribers](#add-subscribers) to your service, you can manually unsubscribe each of them. Follow the steps below.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. Click the three dots icon next to the desired recipient name, and select **[!UICONTROL Delete]**.

    ![Screenshot showing the delete option for unsubscribing profiles.](assets/service-subscribers-delete.png){zoomable="yes"}

1. Confirm deletion.

1. Click **[!UICONTROL Send]** to have the selected recipient receive the unsubscription [confirmation message](manage-services.md#create-confirmation-message) that you defined when [creating the service](manage-services.md#create-service).

    ![Screenshot showing the confirmation message interface for unsubscribing profiles.](assets/service-subscribers-delete-confirmation.png){zoomable="yes"}

The recipient is removed from the **[!UICONTROL Subscribers]** tab and is no longer subscribed to your service.

### Automatically unsubscribe recipients {#automatic-unsubscription}

A subscription service can have a limited duration. Profiles are automatically unsubscribed when the period of validity expires.

This period is specified when [creating the service](manage-services.md#create-service). From the **[!UICONTROL Additional options]**, disable the **[!UICONTROL Unlimited validity period]** option, and define a validity period for the service.

![Screenshot showing the validity period configuration for a subscription service.](assets/service-create-validity-period.png){zoomable="yes"}

After the specified duration expires, all subscribers are automatically unsubscribed from that service.