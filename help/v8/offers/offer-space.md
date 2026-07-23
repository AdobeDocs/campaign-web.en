---
audience: end-user
title: Create and manage offer spaces
description: Learn how to create, configure, deploy, and preview offer spaces in Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
---
# Create and manage offer spaces {#offer-space}

An **offer space** defines where and how an offer is exposed to a contact: which channel it uses (email, direct mail, SMS, inbound web, etc.), which content fields the offer can use, and how the final representation is built. A single environment can contain multiple offer spaces — one for each exposition point.

>[!NOTE]
>
>An offer space is not a channel by itself: it represents a specific location where the offer is displayed on a channel. Two banners on the same web page typically correspond to two different offer spaces. For the full conceptual model, refer to [Create offer spaces](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"} in the console documentation.

## Access offer spaces {#access}

Offer spaces are stored under the offer environment folder. To browse the offer spaces available on your platform, open the **[!UICONTROL Explorer]** and navigate to the offer environment that contains them. From there you can open an existing offer space or create a new one.

## Create an offer space {#create}

To create a new offer space, follow the steps below.

1. From the offer environment, create a new offer space.

1. Enter a label and an internal name for the space, and select the offer environment in which it should be created.

1. Select the **[!UICONTROL Channel]** that matches the exposition point (email, direct mail, SMS, web, etc.).

1. Open the offer space configuration screen.

## Define the content fields {#content-fields}

The content fields list the attributes that can be edited at offer level and reused by the rendering function. The order in which you add the fields in the offer space drives the order in which they are exposed in the offer **[!UICONTROL Content]** section.

By default, every offer ships with the following out-of-the-box content fields: **[!UICONTROL Title]**, **[!UICONTROL Destination URL]**, **[!UICONTROL Image URL]**, **[!UICONTROL HTML content]**, and **[!UICONTROL Text content]**. You can extend this list with any custom field your rendering needs — for example, a **short content**, a **tracked URL**, or any attribute added through schema extension.

1. In the offer space configuration, open the **[!UICONTROL Content fields]** section.

1. Add a new content field and enter a name and a type for it.

1. Save your changes.

>[!IMPORTANT]
>
>To make a custom attribute editable from the offer **[!UICONTROL Content]** section, the attribute must also be declared in the **[!UICONTROL Offer content]** section of the [!DNL nms:offer] schema. Learn more in [Work with schemas](../administration/schemas.md).

## Configure the rendering function {#rendering}

The rendering function builds the final offer representation from the content fields. You can choose between the default rendering — which simply outputs the content as is — or a custom function that combines the fields with HTML, XML, or text.

1. In the offer space, open the **[!UICONTROL Edit function]** section.

1. Select the rendering type: **[!UICONTROL HTML]**, **[!UICONTROL XML]**, or **[!UICONTROL Text]**.

1. Use the expression editor to write the rendering function. You can reference the content fields defined in the space, the offer attributes, and any function from the [expression editor](../query/expression-editor.md).

1. Save the function. It is reused by every offer that targets this space.

>[!NOTE]
>
>If no rendering function is defined, the offer content is returned as is using the out-of-the-box attributes.

## Configure the storage and proposition status {#storage}

Open the **[!UICONTROL Storage]** section to control how propositions generated through this space are persisted and how their status evolves throughout their lifecycle.

* **[!UICONTROL Status when the proposition is created]** — Status applied to the proposition the moment the Offer engine returns it (typically **[!UICONTROL Presented]** for outbound deliveries).

* **[!UICONTROL Status when the proposition is accepted]** — Status applied when the recipient interacts with the offer (typically **[!UICONTROL Accepted]**).

The available status values match the canonical list used by the Campaign Interaction module: **[!UICONTROL Accepted]**, **[!UICONTROL Scheduled]**, **[!UICONTROL Generated]**, **[!UICONTROL Interested]**, **[!UICONTROL Presented]**, **[!UICONTROL Rejected]**. For the full reference of each status, the schema where the values are stored, and the integer codes used in inbound URLs, refer to [Offer proposition statuses](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#offer-proposition-statuses){target="_blank"} in the console documentation.

>[!NOTE]
>
>Status updates run asynchronously through the tracking workflow. For an outbound delivery containing a tracked link, the status of the proposition is automatically switched to **[!UICONTROL Presented]** when the delivery reaches the **[!UICONTROL Sent]** state. To trigger the **[!UICONTROL Interested]** status from a click, add the `_urlType="11"` attribute to the link. The full **inbound interaction** URL syntax (for example to apply the **[!UICONTROL Rejected]** status from a web app) must be configured in the client console — see [Inbound interaction status update](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#configuring-the-status-when-the-proposition-is-accepted){target="_blank"}.

## Configure advanced settings {#advanced}

The **[!UICONTROL Advanced parameters]** section exposes optional configurations, such as the **[!UICONTROL Target notification]** option. These settings are optional for a basic offer space — for their full reference and behavior, refer to [Create offer spaces](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"} in the console documentation.

Offer spaces created on the **inbound web channel** also require the website to be configured to display the offer and to call the Offer engine. This integration is performed in the client console — see [Present offers in real time](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-present-offers.html){target="_blank"} and [Configure the Offer engine integration](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-integration.html){target="_blank"}.

## Deploy the offer space {#deploy}

An offer space must be deployed before it can be used in a delivery. Save your offer space, then launch the deployment action. The status of the deployment is reflected on the offer space.

## Preview the offer space {#preview}

The preview lets you simulate how an offer is selected and rendered for a given target.

1. From the offer space, open the preview.

1. Select a target profile and run the preview. The matching offers are returned with the representation produced by the rendering function.

>[!NOTE]
>
>If no propositions are returned, check the eligibility rules of the offers and the configuration of the space.

Next, [create an offer](create-offer.md) in the catalog and assign it to this space.
