---
audience: end-user
title: Get started with offer management
description: Learn how to manage offers in Adobe Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
---
# Get started with offer management {#gs-offer-management}

This capability lets you add personalized offers to your deliveries and present the most relevant one for each profile in a given context. Offers can be a simple communication message or promotions on one or several products. Based on eligibility rules and priority weights, the Offer engine selects the best proposition to present.

The Campaign Web user interface lets you manage offers end-to-end. You can create and configure offer environments, design offer spaces, build your offer catalog, set eligibility rules, edit offer content, and publish offers.

Offers are then presented to recipients through deliveries based on **eligibility rules** and **priority weights**, so that the best offer is selected for each profile in a given context.

>[!NOTE]
>
>The Campaign Web user interface focuses on the most common offer management usage. Advanced configurations remain available in the Campaign Client Console. Refer to the [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"} 

<!--
and check the [Campaign Web and client console capability matrix](../get-started/capability-matrix.md#offer-capabilities) for the current scope.
-->

## Key concepts {#concepts}

Before you start working with offers, get familiar with the main objects involved.

* **Offer environment** — Container that holds an offer catalog and the related offer spaces. There are two types, the **Design** environment, where you create and configure offers, and the read-only **[!UICONTROL Live]** one, which contains the approved and deployed objects available for delivery. [Learn more](offer-environment.md)

* **Offer space** — Defines where and how an offer is exposed (email, direct mail, SMS, inbound web, etc.). The space lists the content fields that can be used in the offer, the rendering function that builds the offer representation, and the storage settings that drive the proposition status. [Learn more](offer-space.md)

* **Offer catalog and categories** — Offers are organized in a hierarchical catalog of **categories** and sub-categories. Each category can share eligibility rules, validity dates, and **application themes**. A default category is provided in the design environment to receive all offers. 

<!--
To configure categories in depth — including sub-categories, fallback categories, and theme management — refer to the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-catalog/interaction-offer-catalog.html){target="_blank"}.
-->

* **Offer** — An individual offer with its own eligibility period, target filter, weight, and content. Offers are approved and deployed before they can be presented to recipients. [Learn more](create-offer.md)

* **Offer proposition** — Result of presenting an offer to a contact in a given space (a banner on a website, an email, a SMS, etc.). The number of propositions per delivery is configured when [setting up offers in a delivery](../msg/offers.md).

* **Arbitrage** — Principle by which the Offer engine ranks eligible offers by priority to select which ones to present. Arbitrage uses the criteria defined on the categories, the offers, and the context offers.

## Offer management flow {#workflow}

The typical end-to-end flow in Campaign Web UI is the following:

1. **Review the offer environment settings** — Check the design / live mapping, eligibility and weight management settings. [Learn more](offer-environment.md)

1. **Create an offer space** — Define the content fields, the rendering function, and the advanced parameters that match your channel. [Learn more](offer-space.md)

1. **Create offers in the catalog** — Set the eligibility period, the target filter, the weight, and the content for each offer. [Learn more](create-offer.md)

1. **Approve and deploy** — Submit the offer for approval, approve its content and eligibility, then let the deployment process publish it to the live environment. [Learn more](create-offer.md#approve-deploy)

1. **Add the offer to a delivery** — Reference the offer space and the propositions in your email, SMS, push, or direct mail delivery. [Learn more](../msg/offers.md)

## Access offers in the Web UI {#access}

Offers are available from the **[!UICONTROL Offers]** left menu. From there you can browse the catalog, open an offer for edition, and monitor its approval and deployment status.

![Screenshot showing the Offer menu.](assets/offers-gs.png){zoomable="yes"}

Offer environments and offer spaces are accessed through the **[!UICONTROL Explorer]**, by navigating to the corresponding folder.


## Console-only complements {#console-complements}

Some offer features are not yet exposed in the Web user interface and must still be configured from the client console:

* **Offer simulation** — The **Simulation** module that lets you test the distribution of offers before sending. See [Offer simulation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html#offer-simulation){target="_blank"}.

* **Predefined filters** management — Reusable filter rules that can be referenced from any offer. See [Manage predefined filters](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}.

* **Offer tracking** — Configuring tracking for offer propositions to feed the proposition history. See [Track offer propositions](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-tracking.html){target="_blank"}.

* **Operator roles** — Assigning Offer manager / Delivery manager rights. See [Operators of the Interaction module](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html){target="_blank"}.

* **Interaction best practices and arbitrage rules**. See [Campaign Interaction best practices](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

* **Reporting** — Dedicated offer and proposition reports are not yet available in the Web user interface.