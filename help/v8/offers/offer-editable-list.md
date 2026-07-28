---
audience: end-user
title: Add an editable list to the offer schema
description: Learn how to expose a custom collection link as an editable list directly in the offer detail screen.
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
---
# Add an editable list to the offer schema {#offer-editable-list}

When you [extend the [!DNL nms:offer] schema](../administration/schemas.md) with a custom collection link, such as a set of segments linked to an offer, you can expose it as an editable list directly in the offer's **[!UICONTROL Custom options]** section. Instead of managing the related records through a separate screen, the collection is rendered as a list in the offer detail, and you can create new related records inline through a dedicated dialog.

>[!NOTE]
>
>This capability is currently available for the offer schema only.

## Add a collection link field {#add-field}

1. Extend the [!DNL nms:offer] schema with your custom collection, then browse to the **[!UICONTROL Schemas]** menu, open the **[!UICONTROL Marketing offers]** schema, and click **[!UICONTROL Screen edition]**. [Learn more](../administration/schemas-browse-access.md#screen-def).

   ![Screenshot showing the screen definition button.](assets/offers-editable-list.png){zoomable="yes"}

1. In the **[!UICONTROL Detail screen configuration]** section, click the ellipsis icon above the **[!UICONTROL List of custom fields]** table and choose **[!UICONTROL Select attributes]**. [Learn more](../administration/schemas-custom-fields.md).

   ![Screenshot showing the screen definition button.](assets/offers-editable-list-0.png){zoomable="yes"}

1. Browse the attributes and select your custom collection link, identified by its collection icon.

   ![Screenshot showing the attribute picker with a collection link attribute.](assets/offers-editable-list-1.png){zoomable="yes"}

   >[!NOTE]
   >
   >Collection link fields cannot be made mandatory, and do not support sub-attributes. By default, they span two columns in the form.

1. Confirm your selection. The collection link is added to the **[!UICONTROL List of custom fields]** table, with **[!UICONTROL collection]** as its type.

   ![Screenshot showing the attributes added.](assets/offers-editable-list-2.png){zoomable="yes"}

## Configure the collection's editable list {#configure-list}

1. Click the ellipsis icon on the collection field's row and choose **[!UICONTROL Edit]** to open the **[!UICONTROL Collection link settings]** dialog.

   ![Screenshot showing the edit button.](assets/offers-editable-list-3.png){zoomable="yes"}

1. In the **[!UICONTROL General]** tab, optionally set a **[!UICONTROL Visible if]** condition, or enable **[!UICONTROL Read-only]**.

   ![Screenshot showing the edition screen.](assets/offers-editable-list-4.png){zoomable="yes"}

1. In the **[!UICONTROL Screen configuration]** tab, click **[!UICONTROL Select attributes]** and select the attributes to use when adding a new element to the list, for example a segment name and a custom field.

   ![Screenshot showing the screen configuration tab of the collection link settings dialog.](assets/offers-editable-list-5.png){zoomable="yes"}

1. In the **[!UICONTROL Layout]** tab, keep or clear **[!UICONTROL Span two columns]**.

1. Click **[!UICONTROL Confirm]**, then **[!UICONTROL Save]** the screen definition.

## Use the editable list in an offer {#use-list}

1. From the left menu, click **Offers** and open an offer. [Read more](create-offer.md#create)

   ![Screenshot showing the offer screen.](assets/offers-editable-list-7.png){zoomable="yes"}

1. Access the offer properties. The collection is rendered as a list in the **Custom options** section.

   ![Screenshot showing the editable list rendering in the offer detail screen.](assets/offers-editable-list-6.png){zoomable="yes"}

1. Click **[!UICONTROL Add]** to display the attributes you configured, fill them in, and click **[!UICONTROL Confirm]**. The new element is added to the list. 

   You can add multiple elements to the same list, and the offer detail can contain more than one editable list. 
   
1. Click **[!UICONTROL Save]**.

<!--
Each element added through the editable list creates a new related record. For instance, adding a segment to an offer generates the following payload:

```xml
<offer ...>
  <offerSegment segmentName="..." _operation="insert"/>
</offer>
```
-->