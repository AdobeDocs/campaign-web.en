---
title: Get started with Adobe Campaign v8 for marketers
description: Discover key functionality of Campaign v8. It is for marketers migrating from Campaign Standard to Campaign v8.
role: User
level: Beginner, Experienced
---

# Get started for marketers {#acs-gs-marketers}

This guide gives an overview of the key functionalities of Campaign v8, for marketers migrating from Campaign Standard to Campaign v8.

You can access Adobe Campaign v8 via the client console or the Web User Interface. The web interface lets you create, manage and execute key marketing actions. The new Adobe Campaign Web interface offers a modern and intuitive user experience to simplify marketing campaign design and delivery. Learn more in this section. [Learn more](user-interface.md)

With the migration, all your data from Campaign Standard is imported in Campaign v8, ensuring a smooth transition with minimal disruption to your ongoing operations. 

You can continue to use your existing credentials to log in and connect to your new Adobe Campaign v8 instance. Once logged in, you can find all your profiles and workflows being migrated, allowing you to continue to work on your campaigns. 

The primary difference is in the user interface. Below a comparison of the same workflow in the 2 interfaces:

![](_assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Adobe Campaign Web user interface releases operate on a continuous delivery model, which allows for a more scalable, phased approach to feature deployment. Please check the [Release Notes](../../v8/rn/release-notes.md) regularly for the latest updates. 

## Discover the Campaign Web User Interface {#acs-gs-marketers-ui}

In the video below, learn how to access and navigate the Campaign Web User Interface and how to customize the inventory lists.

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

For more details, please refer to the documentation below:

1. [Discover the Campaign Web User Interface](../../v8/get-started/user-interface.md)

1. [Browse and Filter List](../../v8/get-started/list-filters.md)


## Create and manage profiles and audiences {#acs-gs-marketers-audiences}

The general concepts for creating and managing profiles and audiences in Campaign v8 is the same as in Adobe Campaign Standard.

### Manage profiles {#acs-gs-marketers-profiles}

In Adobe Campaign, a profile is a record stored in the database, serving as a key component to create audiences for deliveries and add personalization data to your content.

1. Learn how to access, manage, and explore profiles using the Campaign Web User Interface.

    >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}
    
    Learn more in this section: [Get started with Profiles](../../v8/audience/about-recipients.md)

1. Learn how to [create and manage test profiles](../../v8/audience/test-profiles.md)

### Manage audiences {#acs-gs-marketers-audiences}

Audiences are sets of profiles who share similar behaviors and/or characteristics. This collection of people can either be generated, selected, or loaded. Once created, audiences can be leveraged as the target population of your deliveries.

Learn how to build and manage audiences, how to select audiences for a delivery, and define control groups, in this video:

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

Refer to [Get started with Audiences](../../v8/audience/manage-audience.md){target="_blank"} for more information.

A control group is a sub-population excluded from the delivery. You can define a control group to avoid sending messages to a portion of your audience, and compare post-delivery behavior with the main target. This option helps you measure the impact of your campaign.
Learn how to [set a control group](../../v8/audience/control-group.md){target="_blank"}

>[!AVAILABILITY]
>
>* All audiences created via Campaign Standard Query activity is transformed into predefined filter in Campaign v8 during migration. Campaign v8 also support the Query activity. 
>
>* Read audience gets transformed into Query activity with [predefined filter](../../v8/query/build-query.md)
>
>* Predefined filter only takesthe latest value after audience migration to Campaign v8.
>
>* File Type audiences in Campaign Standard are migrated as list type without dimensions.

### Manage subscriptions {#acs-gs-marketers-sub}

Use Adobe Campaign Web User interface to manage and create your services such as newsletters, and to check the subscriptions or unsubscriptions to these services. Learn more: 

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/audiences/work-with-services/manage-services">
<img alt="Infrequent" src="_assets/lp-list.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/audiences/work-with-services/manage-services"><strong>Create subscription services</strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers">
<img alt="Infrequent" src="_assets/workflow-activities.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers"><strong>Manage subscribers<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/send-to-subscribers">
<img alt="Validation" src="_assets/workflow-create.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/send-to-subscribers"><strong>Send messages to the subscribers of a service</strong></a>
</div>
<p>
</td>
</tr>
</table>

## Use plans, programs and campaigns {#acs-gs-marketers-plans}

Adobe Campaign allows you to configure your folder hierarchy for marketing plans and programs.

Learn more in the [Plans and programs documentation](../../v8/administration/plans-programs.md)


### Create a campaign {#acs-gs-marketers-campaign}

Adobe Campaign allows you to easily orchestrate your targeted marketing initiatives, using the built-in campaign management capability. With the ability to define a schedule, you can plan the duration and timing of your campaigns to align with strategic objectives and maximize audience engagement.

![Campaign flow](_assets/campaign-flow.png)

Follow the documentation below to learn more about campaigns: 

1. [Get started with campaigns](../../v8/campaigns/gs-campaigns.md)
1. [Access and manage your campaigns](../../v8/campaigns/manage-campaigns.md)
1. [Create your first campaign](../../v8/campaigns/create-campaigns.md)


### Create a workflow {#acs-gs-marketers-wf}

With workflows, you can orchestrate the full range of processes and tasks, improve the speed and scale of every aspect of your marketing campaigns, from creating segments and preparing messages to delivery. Plus, you can get your channels in sync with a single, easy-to-use interface for campaign orchestration.

Understand how workflows work and how to create a targeting workflow in this video:

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

Get more details with the [Worklow documentation](../../v8/workflows/gs-workflows.md).

Adobe Campaign Web user interface features a query modeler in workflows that simplifies the process of filtering the database based on various criteria.
[Learn more about query modeler](../../v8/query/query-modeler-overview.md)

To understand the purpose and functionality of each activity within your workflow, explore the detailed information available on [workflow activities](../../v8/workflows/activities/about-activities.md)

Maximize your workflow's efficiency by reviewing the [Guardrails and limitations for workflows](../../v8/get-started/guardrails.md).


>[!AVAILABILITY]
>
>* Workflow execution [history and logs](../../v8/workflows/start-monitor-workflows.md#logs-tasks) are available in Adobe Campaign v8. 
>
>* Historical logs for workflows executed on your Campaign Standard instance are not migrated to Campaign v8.
>
>* Organizational Units are mapped to concept of folder for mapping and ensuring similar access control.
>

## Create and manage deliveries {#acs-gs-marketers-deliveries}

You can create standalone deliveries from the **Deliveries** left menu, or create deliveries in the context of a workflow, included or not in a campaign. Learn how to create a delivery in the following section: [Delivery creation and management documentation](../../v8/msg/gs-deliveries.md)

For an accelerated and improved design process, you can create delivery templates to easily reuse custom content and settings across your campaigns. This functionality enables you to standardize the creative look and feel, in order to be quicker in executing and launching campaigns/ Learn more in the [Delivery template](../../v8/msg/delivery-template.md) page.

Delivery settings are technical delivery parameters that are defined in the delivery template. They can be overloaded for each delivery. These settings are available from the Settings button available when editing a delivery or a delivery template. Learn more in the [Delivery settings](../../v8/advanced-settings/delivery-settings.md) section.

Adobe Campaign Web dynamic content capabilities allows you to customize your content based on the information you have gathered about your recipients. By utilizing dynamic content, you ensure that your marketing efforts are more relevant, avoiding marketing unwanted or unnecessary products or services. Learn more in the [Dynamic content](../../v8/personalization/gs-personalization.md) section.

Once your delivery content has been defined, you can use profiles and test profiles to preview and test it before sending the message. This is a crucial step to ensure that it is accurate but also free of errors both in content and personalization settings. See [Preview and test](../../v8/preview-test/preview-test.md).

You can set the date and the exact time for sending your messages. By choosing the most appropriate time for your marketing message, you can maximise open rates. 

* Learn how to [schedule a stand-alone delivery](../../v8/msg/gs-deliveries.md#gs-schedule)
* Learn how to [schedule a delivery in a workflow](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow)

You can add offers to your deliveries in the Adobe Campaign Web user interface. These offers are available from the Offers left menu which lets you access to the list of offers.  Learn how to [add offers to your messages](../../v8/msg/offers.md)

>[!AVAILABILITY]
>
>* Deliveries in draft state or finished state have been migrated.
>
>* In transit / In progress / Cancelled / Retry in progress / Preparation error deliveries have been migrated to Adobe Campaign v8 but must be prepared again. 
>
>* For Canceled / Retry in progress will be migrated as canceled deliveries: Tracking links, mirror page URL links, subscription/un-subscription link will work as per as per Campaign Standard. 
>
>See also: [Tracking and Monitoring](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}, [Branding](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} in Adobe Campaign.

### Email delivery {#acs-gs-marketers-email}

Learn how to create an email delivery from scratch, define the audience, design the content, simulate preview, and send a proofin this video:
  
>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

Learn how to create your first targeted email in the [Create your first email documentation](../../v8/email/create-email.md)

The detailed steps for sending an email delivery are:

1. **Design and define content**

   Understand how to navigate the Email Designer. Learn how to structure and design an email from scratch, how to personalize, and test your email in the following video:
   
   >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}
   
   The Email Designer enables you to create captivating, individually tailored emails through an intuitive drag-and-drop interface. Learn more in the [Email Designer documentation](../../v8/email/get-started-email-designer.md)

   Learn how to create an email by uploading HTML, how to make it compatible with the Email Designer and how to convert it to a template in this video:
   
   >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}
    
    A content fragment is a reusable component that can be referenced in one or more messages. Learn more about [Content fragments](../../v8/content/fragments.md) to simplify the creation of your email delivery.

    For an accelerated and improved design process, you can create standalone templates to easily reuse custom content across Adobe Campaign. See [Create email templates](../../v8/email/create-email-templates.md)

1. **Preview and test**

    Learn how to preview email message content and personalization, send test deliveries (proofs) and check the email rendering in popular desktop, mobile and web-based clients, in this video:

    >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **Send email and check logs**

    When you have defined your content, audience, and schedule, you are ready to prepare your email delivery. Learn more in the following sections:

   * [Prepare and send an email](../../v8/monitor/prepare-send.md)
   * [Monitor delivery logs](../../v8/monitor/delivery-logs.md)

     
### SMS delivery {#acs-gs-marketers-sms}

SMS deliveries provide a practical and efficient way to send text messages to your customers' mobile devices. With this feature, you can create, personalize, and preview text-based messages for effective communication.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/sms/create-sms">
<img alt="Lead" src="_assets/create_sms.png">
</a>
<div><a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/sms/create-sms"><strong>Create an SMS delivery</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/sms/content-sms">
<img alt="Infrequent" src="_assets/design_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/sms/content-sms"><strong>Design an SMS delivery<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/sms/send-sms">
<img alt="Validation" src="_assets/send_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/sms/send-sms"><strong>Preview and send an SMS delivery</strong></a>
</div>
<p>
</td>
</tr></table>

### Create and manage push notifications {#acs-gs-marketers-push}

Push notifications are essential for reaching out to your mobile app users, even when they're not actively using your app. They serve various purposes like providing updates, driving specific actions, and notifying about deals.

Adobe Campaign v8 supports both Android and iOS Push Channel. To transition existing workflows and deliveries that are using the Push Channel, please connect with your Adobe Campaign Transition Manager.  

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/push/create-push">
<img alt="Lead" src="_assets/push_create.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/push/create-push"><strong>Create a push delivery</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/push/content-push">
<img alt="Infrequent" src="_assets/push_design.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/push/content-push"><strong>Design a push delivery<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/push/send-push">
<img alt="Validation" src="_assets/push_send.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/push/send-push"><strong>Preview and send a push delivery</strong></a>
</div>
<p>
</tr></table>

>[!AVAILABILITY]
>
>Adobe Campaign v8 supports both Android and iOS Push Channel. For transitioning of existing workflows and deliveries using Push Channel please connect with your Adobe Campaign Transition Manager. Learn more on [Channel Set up](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.  

### Direct mail {#acs-gs-marketers-direct-mail}

Direct mail is an offline channel that allows you to produce files to mass deliver personalized letters to your customers such as postcards, flyers, or catalogs. When creating a direct mail delivery, Adobe Campaign automatically generates an extraction file containing all the targeted profiles and selected data, such as postal addresses and profile attributes.

1. [Create Direct Mail delivery](../../v8/direct-mail/create-direct-mail.md)
1. [Define the extraction file](../../v8/direct-mail/content-direct-mail.md) 
1. [Preview and send](../../v8/direct-mail/send-direct-mail.md)


## Create and manage landing pages {#acs-gs-marketers-lp}

Adobe Campaign allows you to create, design, and share landing pages. Landing pages enable you to direct your users to online forms where they can update their data, opt-in/out from receiving your communications, or subscribe to a specific service such as a newsletter.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/landing-pages/create-lp">
<img alt="Lead" src="_assets/lp-subscription.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/landing-pages/create-lp"><strong>Create landing pages</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/landing-pages/lp-content">
<img alt="Validation" src="_assets/lp-design.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/landing-pages/lp-content"><strong>Design landing pages</strong></a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/landing-pages/lp-templates">
<img alt="Validation" src="_assets/lp-reporting.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/landing-pages/lp-templates"><strong>Work with landing page templates</strong></a>
</div>
<p>
</td>
</tr></table>


## Reporting {#acs-gs-marketers-reporting}

Adobe Campaign suite of reporting tools provides valuable insights into the effectiveness of your marketing efforts, allowing you to optimize your campaigns for maximum impact. Learn more in the [Reporting documentation](../../v8/reporting/gs-reports.md).

Dynamic Reporting provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. See the [Dynamic reporting documentation](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} 

>[!AVAILABILITY]
>
>* [Dynamic reporting](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} can be used for reporting of email deliveries, campaign with email deliveries and transactional messages. Demographic analysis by Profile dimension is also available.  
>
> * [Adobe Campaign Web User Interface reporting](../../v8/reporting/campaign-reports.md) is also available for all users transition from Adobe Campaign Standard to Adobe Campaign v8.

Adobe Campaign offers three different reports:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports">
<img alt="Validation" src="./_assets/campaign_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports"><strong>Campaign reports</strong></a>
</div>
<p>
<div>
<a>Provide detailed information on the performance, effectiveness, and outcomes of your individual deliveries, providing you with a comprehensive overview.</a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports">
<img alt="Lead" src="_assets/email_report.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports"><strong>Delivery reports</strong>
</div>
<p>
<div>
<a>Offer a thorough analysis of each delivery's performance, per channel: success rates, audience engagement, and other essential metrics. They allow you to evaluate the overall effectiveness and impact of your campaign.</a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports">
<img alt="Global reports" src="_assets/push_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports"><strong> Global reports</strong></a>
</div>
<p>
<div>
<a>Offer a consolidated overall summary of traffic and engagement metrics for each channel within your Campaign instance. These reports consist of various widgets, each offering a distinct perspective on your campaign or delivery performance.</a>
</div>
<p>
</td>
</tr>
</table>
