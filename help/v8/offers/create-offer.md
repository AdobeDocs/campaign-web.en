---
audience: end-user
title: Create and publish an offer
description: Learn how to create, configure, approve, and deploy an offer in Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
---
# Create and publish an offer {#create-offer}

An **offer** is an individual proposition with its own eligibility period, target filter, weight, and content. Offers are organized in the offer catalog through **categories** and are presented to recipients through an **offer space**.

Before creating an offer, make sure that the offer environment is configured and that at least one offer space is published. Learn more in [Configure an offer environment](offer-environment.md) and [Create and manage offer spaces](offer-space.md).

## Access the offer catalog {#access}

To browse and create offers, select **[!UICONTROL Offers]** from the left navigation rail. The list displays the existing offers. Use the search field, the folder selector, or the [query modeler](../query/query-modeler-overview.md) to filter the list.

Click an offer name to open it for edition, or use the three dots next to it to **[!UICONTROL Duplicate]** or **[!UICONTROL Delete]** it.

## Create an offer {#create}

To create a new offer:

1. From the offers list, click **[!UICONTROL Create offer]**.

1. Enter a label and select the **[!UICONTROL Category]** in which the offer will be stored.

1. (Optional) Configure the approval workflow by assigning one or several approvers to the **[!UICONTROL Content]** and **[!UICONTROL Eligibility]** approval groups. The selected approvers are notified when the offer is submitted.

1. Click **[!UICONTROL Create]** to open the offer for edition.

## Define the eligibility {#eligibility}

The **[!UICONTROL Eligibility]** section controls when and to whom the offer can be presented.

1. **[!UICONTROL Eligibility period]** — Set the start and end dates between which the offer can be presented.

1. **[!UICONTROL Target filter]** — Use the rule builder to restrict the offer to a specific audience. Leave the filter empty to make the offer eligible for the whole environment audience. To reuse a **predefined filter** declared at platform level, refer to [Manage predefined filters](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"} — predefined filters are created from the client console.

1. **[!UICONTROL Offer weight]** — Add one or several weights to influence the priority of the offer when several offers are eligible at the same time. Each weight is defined by a label, an eligibility window, an optional filter, and the expression used to compute the weight value.

1. (Optional) Restrict the offer to specific offer spaces. By default, the offer is available on every offer space of the environment.

>[!NOTE]
>
>The Offer engine sorts eligible offers by decreasing weight and returns the highest weighted propositions first. The selection logic — referred to as **arbitrage** — also takes into account the eligibility rules and weights configured on the parent category and on the environment. Learn more about the arbitrage principle in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

## Define the content {#content}

The **[!UICONTROL Content]** section defines the values that will be exposed by the rendering function.

1. Fill in the out-of-the-box attributes — **[!UICONTROL Title]**, **[!UICONTROL Destination URL]**, **[!UICONTROL Image URL]** — and any custom attribute declared in the offer schema.

1. Use the [expression editor](../query/expression-editor.md) to personalize the values with profile data, offer attributes, or proposition fields.

1. For HTML and text payloads, use the embedded editor to design the content. An image preview is displayed for image fields, and a content definition preview lets you check the final rendering.

>[!IMPORTANT]
>
>The attributes available in the **[!UICONTROL Content]** section depend on the [!DNL nms:offer] schema. To expose custom attributes, extend the schema and select them in the **[!UICONTROL Offer content]** section. Learn more in [Work with schemas](../administration/schemas.md).

## Preview the offer {#preview}

You can preview the offer before submitting it.

1. From the offer, click the **[!UICONTROL Preview]** button.

1. Select a target profile and, if relevant, the offer space against which the preview should be run.

1. The rendering function defined on the offer space is applied to the offer content, and the resulting representation is displayed.

>[!NOTE]
>
>If the preview returns an error or no content, check the rendering function of the offer space, the eligibility rules of the offer, and that all required content fields are filled.

## Approve and deploy the offer {#approve-deploy}

Offers are not immediately available in deliveries: they go through an approval and deployment cycle.

1. From the offer, click **[!UICONTROL Submit]**.

1. The offer is now in the **[!UICONTROL Pending approval]** state. The configured approvers can review the **[!UICONTROL Content]** and the **[!UICONTROL Eligibility]** approvals from their notification list or from the offer dashboard.

1. Once both approvals are granted, the offer enters the **[!UICONTROL Pending deployment]** state. The deployment workflow runs in the background and the offer becomes available in the live environment a few seconds later.

1. Refresh the offer view to confirm the **[!UICONTROL Live]** representation is up to date. From the live offer, you can review the deployed properties, but no edition is possible — go back to the design offer to change any setting.

>[!CAUTION]
>
>Approving an offer's eligibility and content are two distinct actions. An offer can be partially approved (content only, for example) and remain unavailable for delivery until the eligibility approval is also granted.

## Monitor the offer dashboard {#dashboard}

The offer dashboard summarizes the offer status, the approval state, and the deployment progress. From there you can review the current state of the offer, the configured eligibility rules, and access the deployment logs and the audit journal of every action performed on the offer.

Once an offer is live, modifying any setting switches the design offer back to an editable state. The live representation remains untouched until the next approval and deployment cycle.

## Disable an offer {#disable}

When you need to remove a live offer from circulation without deleting it, use the **[!UICONTROL Disable offer]** action.

1. Open the offer from the offer catalog.

1. Click **[!UICONTROL Disable offer]** in the dashboard action bar.

1. Confirm the action. The offer is unpublished and is no longer returned by the Offer engine. Its content and configuration are preserved and you can re-enable it later by submitting it again for approval.

>[!NOTE]
>
>The **[!UICONTROL Disable offer]** action is only available on a deployed offer. A live offer has no other action buttons — every edition must be done on the design offer.

## Use the offer in a delivery {#use-in-delivery}

When the offer is live, it can be selected from any delivery that targets the matching offer space. Learn how to set up offers in a delivery in [Add offers to your messages](../msg/offers.md). For the full outbound delivery integration — including how the engine call is built and how tracking is applied to offer links — refer to [Send offers in outbound deliveries](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-send-offers.html){target="_blank"}.

## Console-only complements {#console-complements}

Some offer features are not yet exposed in the Web user interface and must still be configured from the client console:

* **Offer simulation** — The **Simulation** module that lets you test the distribution of offers before sending. See [Offer simulation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html#offer-simulation){target="_blank"}.

* **Predefined filters** management — Reusable filter rules that can be referenced from any offer. See [Manage predefined filters](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}.

* **Offer tracking** — Configuring tracking for offer propositions to feed the proposition history. See [Track offer propositions](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-tracking.html){target="_blank"}.

* **Operator roles** — Assigning Offer manager / Delivery manager rights. See [Operators of the Interaction module](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html){target="_blank"}.

* **Interaction best practices and arbitrage rules**. See [Campaign Interaction best practices](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.
