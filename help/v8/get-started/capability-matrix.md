---
audience: end-user
title: Campaign Web user interface/client console capability matrix
description: List of features supported in Campaign Web user interface
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
---
# Campaign Web and Campaign Client Console {#capabilities-matrix}

Key Campaign capabilities are available in Campaign Web user interface. This interface was primary designed for marketers to plan, launch and measure their marketing campaigns. All capabilities are listed [in this page](../rn/whats-new.md). 

Campaign platform customization based on business and data needs, and connection to other systems are managed in the Campaign client console. As a consequence, some settings and features can only be accessed, created, or managed from Campaign client console. Some will be available in a later update of Campaign Web user interface. 

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Campaign Management {#campaign-mgt-capabilities}

With Campaign Web user interface, you can create cross channel campaigns as detailed [in this section](../campaigns/gs-campaigns.md). The following capabilities are only available in Campaign client console. They are not accessible in the Campaign Web user interface - but some can be visible from the [Explorer menu](user-interface.md#user-interface-explorer).

Use the provided links to browse the Campaign v8 (client console) documentation and learn how to use these capabilities.

* **Marketing calendar**. The campaign calendar shows all programs, plans, campaigns and deliveries in a global timeline. This capability is only available in the client console. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#campaign-calendar){target="_blank"}
* **Programs and Plans**. Each campaign belongs to a program which belongs to a plan. In Campaign Web user interface, all campaigns are associated to a default built-in plan and program. You can only create and manage plans and programs in the client console. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#work-with-plan-and-program){target="_blank"}
* **Providers, budget and cost management**. You can configure service providers involved in the jobs carried out within your campaigns, including cost structures, and manage your budgets within each program and campaign. This capability is only available in the client console. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html){target="_blank"}
* **Distributed marketing** (Central/Local marketing). Adobe Campaign offers a Distributed Marketing app for implementing cooperative campaigns between central entities (headquarters, marketing departments, etc.) and local entities (sales points, regional agencies, etc.). This capability is only available in the client console. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html){target="_blank"}
* **Marketing Resource Management** (MRM), goals, simulations, and cost control. Adobe Campaign offers a Marketing Resource Management (MRM) app which lets you control marketing actions in a collaborative mode by providing complete management and real-time tracking of the tasks, budgets and marketing resources involved. This capability is only available in the client console. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html){target="_blank"}
* **Task management**. As part of the MRM app, Campaign tasks can be created, assigned, tracked, and monitored from the campaign dashboard. This capability is only available in the client console. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html){target="_blank"}

## Communication channels {#channels-capabilities}

With Campaign Web user interface, you can create, design and send **email**, **SMS**, **push notifications**, **direct mail** and measure their impact using various dedicated reports, as detailed [in this section](../msg/gs-messages.md). However, the following channels are currently **not** available: in-app, LINE, Call center/Custom channel, Social marketing with X (Twitter).

Use the provided links to browse the Campaign v8 (client console) documentation and learn more about these channels.

* **LINE messaging**. LINE is an application for free instant messaging, voice and video calls, available on all mobile devices and on PC. Adobe Campaign allows you to send LINE messages from the client console only. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html){target="_blank"}
* **Call center and Custom channels**. Call center and other custom channels can be implemented in your Campaign environment. These channels can only be available in the client console. [Learn more in Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html#other-channels){target="_blank"}
* **Social marketing** with X (Twitter). You interact with your customers via X (Twitter) by posting messages and sending direct messages. This capability, coming with the Social Marketing add-on, is only available from the client console - [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html){target="_blank"}

## Landing pages and web applications {#Webapps-capabilities}

Adobe Campaign allows you to create, design, and share landing pages. The landing pages experience has been entirely reimagined in the new interface. Discover how to create, design, and publish landing page in Campaign Web user interface [in this section](../landing-pages/get-started-lp.md).

As a consequence, in Campaign client console, you cannot edit, update nor modify a landing page created in the Web interface - and conversely. The following types of web applications are not available in Campaign Web user interface. However, they are visible in the list of landing pages. Use the provided links to browse the Campaign Classic v7 documentation and learn more about these web apps:

* **Web applications**. Adobe Campaign lets you create and publish dynamic and interactive Web applications with preloaded data from the database and content adapted to the rights of the connected user. This capability is only available in the client console. [Learn more in Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html){target="_blank"}
* **Web forms**. Web and landing pages designed in the client console are visible in the Campaign Web user interface but cannot be edited or modified. Some options may differ between the client console web page designer and the landing page designer coming with Campaign Web user interface. [Learn more in Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html){target="_blank"}
* **Online surveys**. You can create online surveys and collect answers from the client console only. This capability is not available in Campaign Web user interface.  [Learn more in Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html){target="_blank"}


## Profiles, test profiles, and audiences {#profiles-audiences-capabilities}

You can create, manage, and update profiles and test profiles in both Campaign client console and Campaign Web user interface. All changes performed in one UI is visible in the other. However, some specific recipient settings and advanced parameters can be missing from the new Campaign Web user interface. 

Note that the term of 'recipient' has been changed to 'profile' in the new Web user interface, and 'Seed addresses' are now 'Test profiles'

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

All audiences created in Campaign client console or in Adobe Experience Platform are available in Campaign Web user interface.

One-shot import/export jobs as described in [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html#import-jobs){target="_blank"} are not available in Campaign Web user interface. <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

## Transactional messaging {#mc-capabilities}

Transactional messaging capabilities coming with the Message Center product package are currently not available in the new Campaign Web user interface. 

Browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} and learn more about real-time messaging capabilities, such as:

* Realtime message authoring and execution on email, SMS and push
* Message enrichment and personalization
* Reporting and monitoring on transactional messaging

## Content design {#content-capabilities}

The new Email Designer coming with Adobe Campaign Web user interface lets you easily create captivating, individually tailored emails through an intuitive drag-and-drop interface. Whether you're starting from a blank slate, importing an existing content or leveraging existing templates, you can design and refine all content for every email. [Learn more](../email/edit-content.md)

With this new user interface, you canmanage email template synchronization from Adobe Experience Manager, and integrate with Adobe Experience Manager as a Cloud Service.

Note that the following capabilities are not available for now in Campaign Web user interface. Use the provided links to browse the Campaign v8 (client console) documentation and learn more about these features.

* **Custom personalization block creation**. In addition to the default personalization blocks, you can create custom blocks from the client console. This capability is not available in Campaign Web user interface. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}
* **Content from custom forms**. The Content management module lets you create and manage forms to assist your users when creating content in Campaign. This capability is only available with the client console. [Learn more in Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html){target="_blank"}
* **AMP for emails**. The AMP for Email new format lets you include AMP components in your messages and improve the email experience with a rich and actionable content. This capability is only available in the client console. [Learn more in Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## Typologies and typology rules {#rules-capabilities}

Typologies are sets of typology rules that are executed during the preparation phase in order to easily apply multiple filtering rules to a delivery at once. They allow marketers to standardize business practices across all deliveries as they let them control, filter, and prioritize the sending of deliveries.

Typology rules can be selected for a delivery, or a delivery template, in Campaign Web user interface, as detailed [in this section](../advanced-settings/delivery-settings.md#typology). However rules and typology rules creation, management, and customzation are only available in Campaign client console.

Use the provided links to browse the Campaign v8 (client console) documentation and learn more about typology rules:

* Control rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html){target="_blank"}
* Fatigue / Pressure rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}
* Filtering rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html){target="_blank"}
* Typology rules management. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html){target="_blank"}
* Campaign simulation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html){target="_blank"}
* JavaScript coding for typology rules authoring. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html#use-cases-on-pressure-rules){target="_blank"}

## Workflows {#wf-capabilities}

The new Campaign Web user interface brings a reimagined workflow canvas interface to design and manage your processes. Key workflow activities are already available in their new design, some will come in a future update. Learn more about workflow capabilities, including guardrails and limitations [in this section](../get-started/guardrails.md).

Note that the following capabilities are only available in the Campaign client console:

* Scripting in workflows
* ETL activities: Export, Edit schema, Data loading, Data extract, SQL code

Learn more about available workflow activities in Adobe Campaign v8 (console) workflow documentation [here](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html){target="_blank"}.

## Offer management {#offer-capabilities}

You can send offers in your deliveries created in the Adobe Campaign Web user interface. These offers must have been created in the client console using the **[!UICONTROL Interaction]** module. Offer design, eligibility rules, and offer management is only available in the Campaign client console. [Learn more](../msg/offers.md)

Learn how to manage an offer catalog in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

## Integrations with Adobe Experience Cloud solutions {#exc-capabilities}

The new Campaign modern UI simplifies marketing campaign design and delivery, and brings consistency, along with other Adobe solutions, including Adobe Experience Platform and Adobe Experience Manager.

The following integrations are available from Adobe Campaign client console, and not yet available in Campaign Web user interface. Use the provided links to browse the Campaign v8 (client console) documentation and learn more about these integrations:

* Adobe Analytics data usage and KPI sharing. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html){target="_blank"}
* Audience sharing with Adobe Experience Cloud (Adobe Audience Manager). [Learn more](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html){target="_blank"}
* Integration with Adobe Target. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html){target="_blank"}
* Integration with Adobe Experience Cloud Triggers. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html){target="_blank"}

## Reporting {#reporting-capabilities}

The new Campaign Web user interface comes with a set of new reports and KPIs, for all channels: delivery reports, campaign reports and global reports. Learn more [in this section](../reporting/gs-reports.md)

Some capabilities are only available from the client console. Browse the provided links to browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html){target="_blank"} and learn more.

* Built in deliverability report and inbox rendering. [Learn more](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html){target="_blank"}
* Reporting customizations. [Learn more](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html){target="_blank"}
* Descriptive analysis. [Learn more](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html){target="_blank"}
* Campaign analysis / Cube reports. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html){target="_blank"}
* Report sharing on schedule as a PDF and CSV, or link. [Learn more](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html){target="_blank"}

## Data modeling and data ingestion {#data-capabilities}

Campaign Web user interface does not surface the following capabilities. They are only available in the client console:

### External accounts {#external}

Adobe Campaign comes with a set of pre-defined external accounts to connect with external systems. As a Campaign System Administrator, you can create and manage external accounts from the client console only.[Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/external-accounts.html){target="_blank"}

### Schema creation and extension {#schema}

Schema creation, modification, and extension are restricted to advanced users. These capabilities are only available from the client console. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html){target="_blank"}

### Workflows data management capabilities {#data}

Data Management combines a set of activities for solving complex targeting issues by offering more efficient and flexible tools such as Data loading, Extraction (file), Update data, Edit schema, or Import/export technical workflows. [Discover workflows data management capabilities in the client console](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#data-management){target="_blank"}
    
>[!NOTE]
>
>While some of these activities are available in the client console only, some are available in Campaign Web user interface such as the **Enrichment**, **Load file**, **Change data source** or **Change dimension** activities. [Learn more on targeting and data management activites in Campaign Web user interface](../workflows/activities/about-activities.md#targeting)

### Federated Data Access configuration {#fda}

Campaign configuration and connection to external systems are restricted to advanced users and only available from the client console. [Learn more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html){target="_blank"}

## Approvals {#approvals-capabilities}

Campaign Web user interface does not surface approval management for content, deliveries, workflows, campaigns and targets. They are only available in the client console.

Learn how to manage approvals in workflows in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html){target="_blank"}.


Learn how to manage delivery, content and target approvals in campaigns in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html){target="_blank"}.


## Permissions {#permissions-capabilities}

Campaign users can only access Campaign Web user interface with their Adobe ID, through Adobe Identity Management System (IMS). Permissions granted to users apply also in the Campaign Web user interface.

Permissions are defined in Adobe Admin Console and Adobe Campaign client console as detailed [in this section](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html). No action on permissions is possible from Adobe Campaign Web user interface.


## Monitoring {#monitoring-capabilities}

Campaign platform monitoring capabitilies are only available in the client console and Campaign Control panel. They do not surface in Campaign Web user interface.

Browse the provided links to the Campaign v8 (client console) documentation and Control panel documentation to learn more.

* [Workflow monitoring](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html){target="_blank"}
* [Workflow heat map](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html){target="_blank"}
* [Performance monitoring](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html){target="_blank"}
* [Deliverabiltiy monitoring](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html){target="_blank"}




