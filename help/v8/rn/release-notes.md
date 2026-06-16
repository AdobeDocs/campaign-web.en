---
title: Campaign v8 Web User Interface Release Notes
description: Discover new features coming with the latest Campaign Web User Interface release
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
---
# Release notes {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Release notes"
>abstract="Adobe Campaign Web user interface releases operate on a continuous delivery model which allows for a more scalable, phased approach to feature deployment. Accordingly, Campaign release notes get updated several times a month, with latest features, improvements, and fixes. We recommend you to check them regularly."

Adobe Campaign Web user interface releases operate on a continuous delivery model which allows for a more scalable, phased approach to feature deployment. Accordingly, these release notes get updated several times a month. Please check them regularly.

## June '26 release {#26-6-release}

_June 16, 2026_

### Improvements {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->
* You can now export data from any list screen including tracking logs. Find your list and simply click the export button. The export includes the rows currently loaded and takes into account the columns displayed on screen and any active search or filters. <!-- [Learn more](../get-started/list-filters.md) -->
* The **Deduplication** and **End** workflow activities now support multiple inbound transitions. When 
more than one inbound transition is available, use the **Sets to join** section in the activity 
properties to select which transitions to connect. <!-- Learn more in these pages: [Deduplication](../workflows/activities/deduplication.md), [End](../workflows/activities/end.md) -->
* Advanced parameters are now exposed in the **Enrichment data** section of the **Build audience** (query type) and **Enrichment** workflow activities. These parameters let you fine-tune how enrichment data is built, including grouping, deduplication, primary-key handling, and inbound event data. <!-- [Learn more](../workflows/activities/enrichment.md) -->
<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
