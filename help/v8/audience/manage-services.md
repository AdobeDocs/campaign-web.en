---
audience: end-user
title: Work with subscription services
description: Learn how to access, create and manage subscription services in Adobe Campaign Web
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
---
# Create and manage subscription services {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Create and manage services"
>abstract="Use Adobe Campaign to create and monitor your services, such as newsletters, and to check the subscriptions or unsubscriptions to these services. Subscriptions only apply to email and SMS delivery."

Use Adobe Campaign Web to manage and create your services, such as newsletters, and to check the subscriptions or unsubscriptions to these services.

Several services can be defined in parallel, for example: newsletters for specific product categories, themes, or areas of a website, subscriptions to various types of alert messages, and real-time notifications.

>[!NOTE]
>
>Subscriptions only apply to email and SMS delivery.

## Access subscription services {#access-services}

To access subscription services available for your platform, follow the steps below.

1. Browse to the **[!UICONTROL Subscription services]** menu on the left navigation rail, under **[!UICONTROL Customer management]**.

    ![Screenshot showing the Subscription services menu on the left navigation rail under Customer management](assets/service-list.png){zoomable="yes"}

1. The list of all existing subscription services is displayed. You can search the services and filter by channel, folder, or add rules using the [query modeler](../query/query-modeler-overview.md).

    ![Screenshot showing the list of subscription services with filters for channel, folder, and rules](assets/service-filters.png){zoomable="yes"}

1. To edit an existing service, click its name.

1. Delete or duplicate any service using the three dots icon next to the service name.<!--so all subscribers are unsubscribed - need to mention?-->

## Create your first subscription service {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Define the service properties"
>abstract="Enter the label of the subscription service, and define additional options, such as a validity period for your service."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Select a confirmation message"
>abstract="When a user subscribes to or unsubscribes from a service, you can send a confirmation message. Select the templates to use for that message."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="Default landing page"
>abstract="Select the default landing pages associated with this service."

To create a subscription service, follow the steps below.

1. Select the **[!UICONTROL Create subscription service]** button.

    ![Screenshot showing the Create subscription service button](assets/service-create-button.png){zoomable="yes"}

1. Select a channel: **[!UICONTROL Email]** or **[!UICONTROL SMS]**.

1. In the service properties, enter a label and define **[!UICONTROL Additional options]** as needed.

    ![Screenshot showing the service properties section with label and additional options](assets/service-create-properties.png){zoomable="yes"}

1. By default, services are stored in the **[!UICONTROL Services and Subscriptions]** folder. You can change it by browsing to the desired location. [Learn how to work with folders](../get-started/permissions.md#folders)

1. By default, subscriptions are unlimited. 

    Disable the **[!UICONTROL Unlimited validity period]** option to define a validity duration for the service. Once the validity period ends:
    * No profile can subscribe to this service anymore.
    * All subscribers to this service are automatically unsubscribed.

    ![Screenshot showing the validity period settings for a subscription service](assets/service-create-validity-period.png){zoomable="yes"}

1. When a user subscribes to or unsubscribes from a service, you can send a confirmation message. Select the templates to use for that message according to your use case. These templates must be configured with the **[!UICONTROL Subscriptions]** target mapping. [Learn more](#create-confirmation-message)

    ![Screenshot showing the confirmation message template selection](assets/service-create-confirmation-msg.png){zoomable="yes"}

1. Click **[!UICONTROL Save and review]**. The new service is added to the **[!UICONTROL Subscription services]** list.

1. Select the default subscription and unsubscription landing pages associated with this service.

    ![Screenshot showing the default landing page settings for a subscription service](assets/service-create-default-lp.png){zoomable="yes"}

    Once done, when [inserting a link](../email/message-tracking.md) in an email, select **[!UICONTROL Subscription link]** or **[!UICONTROL Unsubscription link]**. Upon clicking that link, users will be directed to the subscription or unsubscription landing page referenced in the service. <!--After submitting the form, they will be subscribed to / unsubscribed from the service.-->

    ![Screenshot showing the subscription and unsubscription link settings](assets/service-create-default-lp-link.png){zoomable="yes"}

1. Save and review your changes.

You can now:

* Manually add subscribers to this service, and unsubscribe profiles. [Learn more](../audience/manage-subscribers.md)

* Invite your customers to subscribe to this service through a landing page. [Learn more](../landing-pages/lp-use-cases.md#lp-subscription)

* Send messages to the subscribers of this service. [Learn how](../msg/send-to-subscribers.md)

## Create a confirmation message {#create-confirmation-message}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Select the subscriptions delivery template"
>abstract="To send confirmation messages to the users who subscribe to your service, you must select a specific delivery template based on the **[!UICONTROL Subscriptions]** target mapping, without a defined target."

>[!CONTEXTUALHELP]
>id="acw_unsubscriptions_delivery_template"
>title="Select the unsubscriptions delivery template"
>abstract="To send confirmation messages to the users who unsubscribe from your service, you must select a specific delivery template based on the **[!UICONTROL Subscriptions]** target mapping, without a defined target."

To send confirmation messages to the users who subscribe to or unsubscribe from your service, create a delivery template with the **[!UICONTROL Subscriptions]** target mapping, without a defined target. Follow the steps below:

1. Create a delivery template for the subscription confirmation. [Learn how to create a template](../msg/delivery-template.md)

1. Do not select an audience for this delivery. Instead, access the delivery **[!UICONTROL Settings]**, go to the [Audience](../advanced-settings/delivery-settings.md#audience) tab, and select the **[!UICONTROL Subscriptions]** target mapping from the list.

    ![Screenshot showing the target mapping selection for a delivery template](assets/service-confirmation-template-mapping.png){zoomable="yes"}

    >[!NOTE]
    >
    >If you do not select the **[!UICONTROL Subscriptions]** target mapping, your subscribers will not receive the confirmation message. Learn more about target mappings in [this section](../audience/targeting-dimensions.md).

1. Edit the content of your delivery template, save, and close it.

    ![Screenshot showing the content editor for a delivery template](assets/service-confirmation-template.png){zoomable="yes"}

    >[!NOTE]
    >
    >Learn more about delivery channels and how to define delivery content in the [Email channel](../email/create-email.md) and [SMS channel](../sms/create-sms.md) sections.

1. Repeat the steps above to create a delivery template for the unsubscription confirmation.

You can now select these messages when [creating a subscription service](#create-service). Users who subscribe to or unsubscribe from that service will receive the selected confirmation messages.

## Monitor your subscription services {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="Subscribers count"
>abstract="Click **Calculate** to get the total number of subscribers for this service."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers_report"
>title="Total number of subscribers"
>abstract="The Key Performance Indicator (KPI) provides a comprehensive view of the subscriber base, showcasing the total count of individuals who have subscribed to this service."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="Number of subscriptions for the period"
>abstract="Use the drop-down list to change the time range and view the number of subscriptions and unsubscriptions over the selected period."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="Subscriptions overall evolution"
>abstract="This graph shows the breakdown by period, including subscriptions, unsubscriptions, the evolution in numbers, and the loyalty percentage."

To measure the effectiveness of your subscription services for SMS and email channels, access the logs and reports for a given service.

1. Select an existing service from the **[!UICONTROL Subscription services]** list. Click **[!UICONTROL Calculate]** to get the total number of subscribers.

    ![Screenshot showing the total number of subscribers calculation](assets/service-logs-subscribers-count.png){zoomable="yes"}

1. From the service dashboard, select **[!UICONTROL Logs]** to view the list of subscribers to this service.

    You can check the total number of subscribers, the name and address of each recipient, and when they subscribed or unsubscribed. You can also filter them.

    ![Screenshot showing the logs section with subscriber details](assets/service-logs.png){zoomable="yes"}

1. From the service dashboard, select **[!UICONTROL Reports]**. Check the following indicators:

    * The **[!UICONTROL Total numbers of subscribers]** is displayed.

    * View the number of subscriptions and unsubscriptions over a selected period. Use the drop-down list to change the time range.

        ![Screenshot showing the reports section with subscription and unsubscription data](assets/service-reports.png){zoomable="yes"}

    * The **[!UICONTROL Overall evolution of subscriptions]** graph shows the breakdown by period, including subscriptions, unsubscriptions, the evolution in numbers, and the loyalty percentage.<!--what is Registered?-->

1. Use the **[!UICONTROL Reload]** button to retrieve the latest values from the execution and schedule of the tracking workflow.