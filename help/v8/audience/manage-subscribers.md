---
audience: end-user
title: Manage the subscribers of a service
description: Learn how to manage and deliver to the subscribers of a service in Adobe Campaign Web
badge: label="Beta"
---

# Manage the subscribers of a service {#manage-subscribers}

Once you [created a service](manage-services.md#create-service), you can add subscribers, unsubscribe recipients and deliver to the subscribers of that service.

## Add subscribers to your service {#add-subscribers}

To manually add subscribers, follow the steps below.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. Select the **[!UICONTROL Subscribers]** tab and click **[!UICONTROL Add profiles]**.

    ![](assets/service-subscribers-tab.png)

1. Select the profiles you want to add from the list and click **[!UICONTROL Confirm]**.

    ![](assets/service-subscribers-select-profiles.png)

1. Click **[!UICONTROL Send]**.<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> The selected recipients will receive the subscription [confirmation message](manage-services.md#create-confirmation-message) that you selected when [creating the service](manage-services.md#create-service).

    ![](assets/service-subscribers-confirmation-msg.png)

The profiles added are displayed in the **[!UICONTROL Subscribers]** list. They are now subscribed to your service.

## Remove subscribers from your service {#remove-subscribers}

### Manually unsubscribe recipients {#manual-unsubscription}

Once you [added subscribers](#add-subscribers) to your service, you can manually unsubscribe each of them. Follow the steps below.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. Click the three dots icon next to the desired recipient name and select **[!UICONTROL Delete]**.

    ![](assets/service-subscribers-delete.png)

1. Confirm deletion and click **[!UICONTROL Send]**. The selected recipient will receive the unsubscription [confirmation message](manage-services.md#create-confirmation-message) that you selected when [creating the service](manage-services.md#create-service).

    ![](assets/service-subscribers-delete-confirmation.png)

The recipient is removed from the **[!UICONTROL Subscribers]** list and is no longer subscribed to your service.

### Automatically unsubscribe recipients {#automatic-unsubscription}

A subscription service can have a limited duration. Recipients are automatically unsubscribed when the period of validity expires.

This period is specified when [creating the service](manage-services.md#create-service). From the **[!UICONTROL Additional options]**, disable the **[!UICONTROL  Unlimited validity period]** option and define a validity period for the service.

![](assets/service-create-validity-period.png)

After the specified duration expires, all subscribers are automatically unsubscribed from that service.

## Deliver to the subscribers of a service

Once you [created a subscription service](manage-services.md#create-service), your can target its subscribers in a delivery. Follow the steps below.

1. [Create an audience](../audience/create-audience.md) including the subscribers to the service you created:

    * In the **[!UICONTROL Build audience]** activity, display the advanced attributes and select **[!UICONTROL Recipient]** > **[!UICONTROL Subscriptions]** > **[!UICONTROL Service]**.

    * In this example, select the users who are subscribed to the service that has the **Luma Newsletter** label.

    ![](assets/service-audience-subscribers.png)

1. [Create a delivery](../msg/gs-messages.md#create-delivery) and select the audience that you created above.

    ![](assets/service-delivery-targeting-subscribers.png)

1. Edit your message content as wanted and send the delivery.

    ![](assets/service-delivery-ready.png)

Your delivery is sent to the subscribers of that service only.
