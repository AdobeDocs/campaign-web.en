---
audience: end-user
title: Get started with messages and deliveries in Campaign v8 Web
description: Learn how to work with deliveries and send messages with Campaign Web
badge: label="Alpha" 
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
---
# Get started with messages{#gs-messages}

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Deliveries"
>abstract="Browse through your list of deliveries. You can view their status, contact and modification dates, key KPIs. You can filter the list by state, contact date or channel. Click the 'Create delivery' button to add a new delivery. Select a delivery to view its content, audience, and details."
With Adobe Campaign, you can send cross-channel campaigns including emails, SMS, and Push notifications, and measure their effectiveness using various dedicated reports. 

These messages are designed and sent though deliveries, and can be personalized for each recipient. These deliveries can be standalone or included in the context of a marketing campaign.

Adobe Campaign v8 comes with the following delivery channels: Email, SMS and Mobile apps.

<table style="table-layout:fixed">
    <tr style="border: 0;">
    <td>
    <a href="../email/create-email.md">
    <img alt="Email" src="assets/do-not-localize/email.jpg">
    </a>
    <div><a href="../email/create-email.md"><strong>Create emails</strong>
    </div>
    <p>
    </td>
    <td>
    <a href="../push/create-push.md">
      <img alt="Push" src="assets/do-not-localize/push.jpg">
    </a>
    <div>
    <a href="../push/gs-push.md"><strong>Create push notifications</strong></a>
    </div>
    <p>
    </td>
    <td>
    <a href="../sms/create-sms.md">
      <img alt="SMS" src="assets/do-not-localize/sms.jpg">
    </a>
    <div>
    <a href="../sms/create-sms.md"><strong>Create SMS messages</strong></a>
    </div>
    <p>
    </td>
    </tr>
    </table>


## Create a delivery {#create-delivery}


You can create standalone deliveries from the **[!UICONTROL Deliveries]** left menu, or create deliveries in the context of a marketing campaign, from the **[!UICONTROL Campaigns]** left menu. 

Browse the tabs below to learn how to create a delivery:

>[!BEGINTABS]

>[!TAB Create a standalone delivery]

To create a standalone delivery, follow these steps:

1. Browse to the **[!UICONTROL Deliveries]** menu on the left navigation, and click the **[!UICONTROL Create delivery]** button.

    ![](assets/create-a-delivery.png)
    
1. Choose a channel for the delivery. Learn more about delivery channels and how to define a delivery content in these sections: 

    * [Email channel](../email/create-email.md)
    * [Push notification channel](../push/gs-push.md)
    * [SMS channel](../sms/create-sms.md)

1. Define the delivery audience, for the main target and the control group. Learn more about audiences in [this section](../audience/about-audiences.md).
1. Define the message content.
1. (optional) Define the delivery schedule. If no schedule is defined, messages are sent immediatly after clicking the **[!UICONTROL Send]** button.
1. Click the  **[!UICONTROL Review and send]** button to check your settings.
1. Use the  **[!UICONTROL Simulate content]** button to test your delivery, and personalization settings. Learn more about message simulation in [this section](../preview-test/preview-test.md).
1. Click the  **[!UICONTROL Prepare]** button to compute the target population and generate the messages. Preparation step can take a few minutes. When preparation is complete, messages are ready for sending. In case of an error, browse to the **Logs** to check alerts and warning.
1. Check results, and click the  **[!UICONTROL Send]** button to start sending messages.
1. Once messages are sent, browse to the **Reports** section to access key metrics. Learn more about delivery reports in [this section](../reporting/delivery-reports.md).

>[!TAB Create a delivery in a campaign]

To create a delivery in a campaign, follow these steps:

1. Create a campaign or open an existing campaign. Learn more about [marketing campaigns](../campaigns/gs-campaigns.md).
1. Create a workflow or open an existing workflow.
1. Add and configure a **[!UICONTROL Build audience]** activity, and click the `+`button.

    ![](assets/add-delivery-in-wf.png)

    The **[!UICONTROL Build audience]** activity is detailed in [this section](../workflows/activities/build-audience.md).

1. Select a delivery activity: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Push notification (Android)]** or **[!UICONTROL Push notification (iOS)]**. Learn more about delivery channel activities in a workflow, and how to define a delivery content in this [section](../workflows/activities/about-activities.md#channel).
1. Start the workflow, and check logs.

You can also add deliveries in a campaign without creating a workflow. To achieve this, browse to the **[!UICONTROL Deliveries]** tab of your campaign and click the **[!UICONTROL Create delivery]** button.

![](assets/new-campaign-delivery.png)

Configuration steps are similar as for standalone deliveries.

For more information on how to configure a campaign and manage deliveries which belong to a campaign, refer to [this section](../campaigns/gs-campaigns.md).

>[!ENDTABS]


## Add personalization{#personalization}

Messages delivered by Adobe Campaign can be personalized in various ways. [Learn more about personalization capabilities](../personalization/gs-personalization.md).

Use Campaign to create dynamic content and send personalized messages. Personalization capabilities can be combined to improve your messages and create a custom user experience.

You can personalize the message content by:

* Inserting dynamic **personalization fields**

    Personalization fields are used for first-level personalization of your messages. You can select any field available in the database from the personalization editor. For a delivery, you can select any field related to the recipient, the message or the delivery. These personalization attributes can be inserted in the subject line or the body of your messages. [Learn more](../personalization/personalize.md)
    
* Inserting pre-defined **content blocks**
    
    Campaign comes with a set of personalization blocks which contain a specific rendering that you can insert into your deliveries. For example, you can add a logo, a greeting message, or a link to the mirror page of the message. Content blocks are available from a dedicated entry un the personalization editor. [Learn more](../personalization/personalize.md#ootb-content-blocks)

* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true. [Learn more](../personalization/conditions.md)

* Add **personalized offers**
    
    Insert personalized offers in your message content, depending on the recipient location, the current weather, or the last purchase order.


## Preview and test your deliveries

Once your message content has been defined, you can preview it to control the rendering of your messages, and check personalization settings with test profiles. [Learn more](../preview-test/preview-test.md)


## Monitoring and tracking logs{#gs-tracking-logs}

Monitoring your deliveries after they have been sent is a key step to ensure your maketing campaigns are efficient and reach out to your customers. 

You can monitor after sending a delivery, as well as understand how delivery failures and quarantines are managed.

Learn more about monitoring and tracking capabilities in [this section](../reporting/gs-reports.md).

## Duplicate a delivery {#delivery-duplicate}

You can create a copy of an existing delivery, either from the delivery list or from the delivery dashboard. 

To duplicate a delivery from the list of deliveries, follow these steps:

1. Click the three dots button on the right, next to the name of the delivery to duplicate.
1. Select  **[!UICONTROL Duplicate]**.
1. Confirm duplication: the new delivery dashboard opens in the central screen.

To duplicate a delivery from its dashboard, follow these steps:

1. Open the delivery and click the  **[!UICONTROL ...More]** button on the top section of the screen. 
1. Select **[!UICONTROL Duplicate]**. 
1. Confirm duplication: the new delivery replaces the current delivery in the central screen.

## Delete a delivery {#delivery-delete}

Deliveries are deleted from the delivery list - either from the main delivery entry in the left rail, or from the delivery list of a campaign. 

To delete a delivery from the list of deliveries, follow these steps:

1. Click the three dots button on the right, next to the name of the delivery to duplicate.
1. Select  **[!UICONTROL Delete]**.
1. Confirm deletion.

![Delete a delivery from the delivery list](assets/delete-delivery-from-list.png)

All deliveries are available in these lists, but deliveries created in a workflow cannot be deleted from there. To delete a delivery created in the context of a workflow, you must delete the delivery activity from the workflow.

To delete a delivery from a workflow, follow these steps:

1. Select the delivery activity .
1. Click the  **[!UICONTROL Delete]** icon on the right panel.
1. Confirm deletion. If the delivery has child nodes, you can choose to delete them as well, or to keep them.

![Delete a delivery in a workflow](assets/delete-delivery-from-wf.png)
