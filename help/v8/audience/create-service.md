---
audience: end-user
title: Work with subscription services
description: Learn how to create services in Adobe Campaign Web
badge: label="Beta" 
---

# Work with subscription services {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Create and manage your services"
>abstract="Use Adobe Campaign to create and monitor your services such as newsletters, and to check the subscriptions/unsubscriptions to these services. Subscriptions only apply to email and SMS delivery."

Use Adobe Campaign web to manage and create your services such as newsletters, and to check the subscriptions/unsubscriptions to these services.

>[!NOTE]
>
>Subscriptions only apply to email and SMS delivery.

Several services can be defined in parallel, for example: newsletters for specific product categories, themes or areas of a web site, subscriptions to various types of alert messages, and real-time notifications.

To learn more on managing subscriptions and unsubscriptions, refer to the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## Access susbscription services {#access-services}

To access subscription services available for your platform, browse to the **[!UICONTROL Subscription services]** menu on the left navigation rail.

![](assets/service-list.png)

The list of all existing subscription services is displayed. You can search the services and filter on the channel, the folder or use advanced filters.

![](assets/service-filters.png)

To edit an existing service, click its name.

## Create your first subscription service {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Subscriptions service properties"
>abstract="Enter the label of the subscription service, and define additional options."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Subscriptions service confirmation messages"
>abstract="When a user subscribes to a service or unsubscribes from a service, you can send a confirmation message. Select the templates to use for these messages."


To create a subscription service, follow these steps:

1. Select the **[!UICONTROL Create subscription service]** button.

    ![](assets/service-create-button.png)

1. Select a channel: **[!UICONTROL Email]** or **[!UICONTROL SMS]**.

1. In the service properties, enter a label and define additional options as wanted.

    ![](assets/service-create-properties.png)

1. By default, subscriptions are unlimited. You can disable the **[!UICONTROL  Unlimited validity period]** option to define a validity duration for the service. <!--The duration can be specified in days or months.TBC-->

    ![](assets/service-create-validity-period.png)

1. When a user subscribes to or unsubscribes from a service, you can send a confirmation message. Select the templates to use for that message according to your use case.

    ![](assets/service-create-confirmation-msg.png)

1. Click **[!UICONTROL Save]**. The new service is added to the **[!UICONTROL Subscription services]** list.

<!--
## Reporting

You can measure the effectiveness of your subscription services for SMS and email channels.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. From the service dashboard, click More > Reports?

1. Check the following indicators:

* Total numbers of subscribers

* Area graph with subscriptions and unsubscriptions. Use the dropwdown to change the time range. (24h, 48h, 1 week, 2 weeks, 1 month, 6 months)

* The breakdown by period. including subs, unsub, evolution in numbers and % and loyalty.
* Last updated / Next refresh time: these values are retrieved from the execution and schedule of the tracking workflow
-->


