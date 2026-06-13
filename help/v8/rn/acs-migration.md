---
audience: end-user
title: Transition from Campaign Standard to Adobe Campaign Web
description: Discover Campaign Web User Interface
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
TQID: https://experienceleague.adobe.com/nD7hOr0bHeBrGYrxutHio-M2EEJM4mYPVoaPelYzJXs
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: b12f6872-9271-4369-85e5-86969a0b99a2
    internal-label: APIs
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
subfeature_v2:
  - id: bf97c196-a4d1-4fa3-a151-e68a114c8ac0
    internal-label: REST API
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
---
# Campaign Standard transition to Campaign v8 {#acs-to-ac}

Adobe Campaign Standard users are now eligible to transition to Adobe Campaign Managed Cloud Services v8. This transition offers several benefits:

* **Robust IT Infrastructure**: Managed Cloud Services v8 provides a more robust IT infrastructure, ensuring enhanced performance, reliability, and scalability for campaigns.
* **Enhanced Support**: The Managed Cloud Services team offers top-notch assistance to ensure a smooth transition and ongoing platform monitoring. Support includes troubleshooting and proactive maintenance.
* **Integration with Adobe Experience Platform**: Managed Cloud Services v8 connects seamlessly with Adobe Experience Platform, enabling users to leverage their data fully and deliver personalized, impactful campaigns across channels.
* **Consistent User Interface and Experience**: Transitioning to Managed Cloud Services v8 does not disrupt workflows. Users continue to enjoy the familiar interface and experience, minimizing the learning curve for teams.

**As a Campaign Standard user transitioning to Campaign v8, learn how to start [in this document](../../adoption/home.md).**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Key capabilities {#key-features}

Campaign v8 users have access to both the new Campaign Web interface and the v8 console. Data and settings synchronize between environments. All data and settings available in the client console are visible in the Campaign Web user interface, accessible from the Explorer left navigation. [Learn more](../get-started/user-interface.md#user-interface-explorer)

The Campaign Web user interface is designed for marketers to easily build and orchestrate campaigns. Key capabilities of the Campaign v8 Web user interface include:

* **Modern, friendly, and unified experience**. [Learn more](../get-started/connect-to-campaign.md).
* **New powerful capabilities and seamless processes**. [Learn more](../get-started/user-interface.md).
* **Simplified and intuitive query modeler**. [Learn more](../query/query-modeler-overview.md).
* **Built-in cross-channel campaign management capabilities**. [Learn more](../msg/gs-messages.md).
* **Redesigned campaign workflow activities**. [Learn more](../workflows/gs-workflows.md).
* **Easy profile creation and management**. [Learn more](../audience/about-recipients.md).
* **Predefined filters**. [Learn more](../get-started/predefined-filters.md).
* **HTML converter for email design**. [Learn more](../email/existing-content.md).
* **SMS with offers**. [Learn more](../msg/offers.md).

The Campaign client console is designed for administrators and developers to configure and customize their environment. Key capabilities available in the Campaign client console are detailed in [this documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Learn more about supported and unsupported capabilities, and interoperability between the Campaign Web user interface and the Campaign client console [in this page](../get-started/capability-matrix.md).

<!--
## Terminology {#terminology}
Most concepts are similar between Campaign v8 and Campaign Standard. However, there are a few terminology differences. Examples include:
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## Specific features {#new-features}

To ensure a smooth transition to Campaign v8, key Campaign Standard capabilities have been added to Campaign v8:

* **Dynamic Reporting**: Dynamic Reporting provides customizable, real-time reports to measure the impact of marketing activities. It includes access to profile data for demographic analysis by dimensions such as gender, city, and age, alongside functional email campaign data like opens and clicks. [Learn more](../reporting/dynamic-reporting/get-started-reporting.md).

* **Centralized Branding**: Adobe Campaign allows companies to define brand visual and technical guidelines. Users can present a consistent brand to customers, from logos to technical aspects such as email sender, URL, or domains. [Learn more](../administration/branding/branding-gs.md).

* **REST APIs**: Campaign Standard migrated users can use REST APIs to create integrations for Adobe Campaign and build ecosystems by interfacing Adobe Campaign with other technologies. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html){target="_blank"}.

* **Landing Pages**: Campaign v8 landing pages include improvements to ensure feature parity with Campaign Standard. Learn more in the [release notes](../rn/release-notes.md#new-24-4) and the landing page [documentation](../landing-pages/get-started-lp.md).

* **Visual Fragments**: Visual fragments are reusable visual components referenced in one or more email deliveries or content templates. Modifying a fragment updates all content using it. This functionality allows marketing users to prebuild multiple custom content blocks for quick message assembly in an improved design process. [Learn more](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->