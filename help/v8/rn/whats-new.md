---
audience: end-user
title: What's new in Campaign Web v8
description: Discover new feature coming with Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Beta" 
---

# What's new? {#new}

We are thrilled to introduce the BETA version of Adobe Campaign web UI. Our latest release is packed with intuitive features designed to simplify the creation of personalized cross-channel campaigns, drive exceptional results, and give you a competitive advantage across all channels.

## Key capabilities {#key-features}

This new Campaign web interface is currently only available to **Beta practitioners** with the following capabilities:

**Modern, intuitive and unified experience**

Campaign new Web UI offers a new user experience, aligned with all Adobe Experience Cloud solutions and apps. It offers:

* Access to the new interface, and your other Adobe solutions with a single and shared user session
* New navigation experience, with all menus and folders available from the left rail
* Solution and organization switchers from the top bar
* Unified Shell integration, with a direct access to community, help center, and support

**New powerful capabilities and seamless processses**

* Reimagined workflow canvas interface to design and manage your processes
* Dynamic content to deliver highly targeted and personalized experiences to your audience
* Native integration with Adobe Experience Platform audiences
* Template management for workflows, deliveries, campaigns and content

Learn more about the new UI in [this page](../get-started/user-interface.md).

**Create, launch and measure your campaign**

Use the new Campaign Web UI to:

* Design personalized email content with the email designer - [Learn more](../content/edit-content.md)
* Send cross cannel campaigns, including SMS and push notifications - [Learn more](../workflows/activities/channels.md)
* Define target audiences with the rule builder - [Learn more](../audience/about-recipients.md)
* Preview, test and send your messages - [Learn more](../monitor/prepare-send.md)
* Monitor send and measure results with built-in reports - [Learn more](../reporting/delivery-reports.md)


## Beta release updates {#beta-release}

Key capabiities coming with Campaign Web Beta are listed below.

* **More Campaign Workflow activities**

    Supercharge your marketing campaigns with our **expanded set of workflow activities**. Unlock new possibilities for automation and optimization, allowing you to create more dynamic and personalized customer journeys. From advanced segmentation to conditional triggers, our additional workflow activities empower you to deliver targeted messages and drive better campaign performance.

    Learn more in [this section](../workflows/gs-workflows.md).

* **Gen AI for Email content**

    Say goodbye to manual content creation and hello to efficient, data-driven campaigns with the power of Gen AI.  Our Gen AI technology utilizes advanced algorithms to **generate highly engaging and personalized content**. Drive higher open rates, click-through rates, and conversions with Gen AI's intelligent content generation. Stay ahead of the competition and elevate your email marketing game with Gen AI on email content. This capability will be available starting early October.

    Learn more in [this section](../content/generative-gs.md).

* **Predefined Filters**
    
    Introducing Predefined Filter Management. Campaign web UI now offers you an user-friendly interface to effortlessly **manage and customize predefined filters** to meet your specific needs. Create once and save for future use.

    Learn more in [this section](../get-started/predefined-filters.md).

* **Target Audience with the rule builder**

    Building a delivery target has never been easier! With our **latest rule builder**, you now have the ability to define filtering criteria for recipients or any other targeting dimension from the database. What's more, you can take advantage of your AEP (Adobe Experience Platform) audience to further refine your target audience and maximize your campaign's impact.

    Learn more in [this section](../audience/segment-builder.md).

* **SMS with offers**

    The new web UI now enables you to **integrate offers with SMS** in addition to Email. Reach your audience on their mobile devices, delivering promotions, and timely notifications. Elevate your marketing efforts by harnessing the power of integrated offers through SMS on our advanced web platform.
   
    Learn more in [this section](../content/offers.md).

<!--
* Adobe Experience Manager (AEM) Integration
    
    With our AEM integration extended to web UI, you can easily manage assets and synchronize full HTML templates, empowering you to create captivating digital experiences without any hassle. 
    
    Elevate and streamline your content management capabilities on the web UI with this integration to boost productivity.
-->

* **Knowledge Assistant with Gen AI**

    Ask questions and find guidance directly from the product user interface. The new **AI-powered Knowledge Assistant**, embedded in the contextual help popovers, helps you learn and grow your expertise on new Campaign features. Based on the latest product documentation, it assists you to find help and get step-by-step guidance instantly, as you are building your use cases. This capability will be available starting early October.
       
    Learn more in [this section](../get-started/using-ai.md).

* **HTML Converter for email design**

    You can now **import and convert any HTML content** in Campaign's email editor. Content blocks are automatically identified, and available in the email designer: use its powerful design capabilities to update and personalize it!

    Learn more in [this section](../content/existing-content.md).


## Transition to Campaign Web UI

As a Campaign user, you can still access the client console to build and manage Campaign resources and components. Data and settings are synchronized from an environment to another. Learn more in [this section](../get-started/get-started.md#about-campaign-client-consoleac-client).

In addition, all your data and settings already available in the client console are visible in the Campaign Web UI, from the Explorer left navigation. Learn more about the Explorer view in [this section](../get-started/user-interface.md#explorer-user-interface-explorer).

With Campaign Web Beta release, the user interface reflects the user's permissions. Learn more about permissions in [this page](../get-started/permissions.md)

## Terminology updates {#terminology-updates}

As an existing Campaign user, note that some concepts have been renamed to align with the latest terminology standards. These changes only apply to Campaign Web UI and are not reflected in the client console. They are summarized below.

* Proofs are now **Test emails**: to send a proof, use the **Test** button in the email delivery UI. The target of the proofs is now refered as **Test profiles**. [Learn more](../preview-test/test-deliveries.md).
* Seed addresses are now used as **Test profiles**: send the test email to seed addresses, which are additional recipients in the database. [Learn more](../preview-test/test-deliveries.md).
* Delivery analysis is now the **delivery preparation**. When you need to launch the message preparation, click the **Prepare** button. [Learn more](../monitor/prepare-send.md).
* Email Preview is now available throught the **Simulate content** button. [Learn more](../preview-test/preview-test.md)
* Lists are now **Audiences**. [Learn more](../audience/about-recipients.md).

## Limitations{#limitations-beta}

The limitations below apply to this Beta version:

* Editable objects are: Deliveries, Campaigns, Workflows, Audiences, Subscription Services, Predefined Filters, and Templates. The others are read-only. Use filters and create rules to browse them all.
* The Administration user interface is not available.
* Reporting metrics (such as opens and tracking data) are updated every hour.
* Delivery dashboard KPIs are updated every 5 min. - but the Delivery preparation is real-time.
* Adobe Experience Cloud Notifications and Unified Help available in the top bar are not yet integrated.

More guardrails and limitations are available in [this page](../get-started/guardrails.md).