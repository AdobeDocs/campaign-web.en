---
title: Get started with Adobe Campaign v8 for marketers
description: This tutorial gives an overview of the key functionality of Campaign v8. It is for marketers migrating from Campaign Standard to Campaign v8.
role: User
level: Beginner, Experienced
jira: KT-15788
---

# Get started for marketers

This guide gives an overview of the key functionality of Campaign v8. It is for marketers migrating from Campaign Standard to Campaign v8.

You can access Adobe Campaign v8 via the client console or the Web User Interface. The web interface lets you create, manage and execute key marketing actions. 

All of your data from Adobe Campaign Standard is imported in Adobe Campaign v8, ensuring a smooth transition with minimal disruption to your ongoing operations. 

You can continue to use your existing credentials to log in and connect to your new Adobe Campaign v8 instance. Once logged in, you can find all your profiles and workflows being migrated, allowing you to continue to work on your campaigns. 

The primary difference is in the user interface. Below a comparison of the same workflow in the 2 interfaces :

![](_assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Adobe Campaign Web user interface releases operate on a continuous delivery model, which allows for a more scalable, phased approach to feature deployment. Please check the [Release Notes](https://experienceleague.adobe.com/en/docs/campaign-web/v8/release-notes/release-notes) regularly for the latest updates. 

## Discover the Campaign Web User Interface

Learn how to access and navigate the Campaign Web User Interface and how to customize the inventory lists. Discover the AI powered Knowledge Assistant.

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

For more details, please refer to the documentation below :

1. [Discover the Campaign Web User Interface](../../v8/get-started/user-interface.md)
2. [Browse and Filter List](../../v8/get-started/list-filters.md)


## Create and manage profiles and audiences

>[!NOTE]
>
>The general concept of creating and managing profiles and audiences in Campaign v8 is the same as in Adobe Campaign Standard.

### Manage profiles

In Adobe Campaign, a profile is a record stored in the database, serving as a key component to create audiences for deliveries and add personalization data to your content.

1. Learn how to access, manage, and explore profiles using the Campaign Web User Interface.

    >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}
    
    See [Get started with Profiles](../../v8/audience/about-recipients.md){target="_blank"} for more information.

1. [Create and manage test profiles](../../v8/audience/test-profiles.md){target="_blank"}

### Manage audiences

Audiences are sets of profiles who share similar behaviors and/or characteristics. This collection of people can either be generated, selected, or loaded. Once created, audiences can be leveraged as the target population of your deliveries.

Learn how to build and manage audiences, how to select audiences for a delivery, and define control groups.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

See [Get started with Audiences](../../v8/audience/manage-audience.md){target="_blank"} for more information.

A control group is a sub-population excluded from the delivery. You can define a control group to avoid sending messages to a portion of your audience, and compare post-delivery behavior with the main target. This option helps you measure the impact of your campaign.
Learn how to [set a control group](../../v8/audience/control-group.md){target="_blank"}

>[!AVAILABILITY]
>
>1- All audiences created via Adobe Campaign Standard query activity will get transformed into predefined filter in Adobe Campaign v8 during migration. Adobe Campaign also support query activity. 
a. Read audience will get transformed to query activity with [predefined filter](../../v8/query/build-query.md){target="_blank"}.
b. Predefined filter will only take the latest value after audience migration to Adobe Campaign v8. 
2- File Type audiences in Adobe Campaign Standard will be migrated as list type without dimensions.

### Manage subscriptions

Use Adobe Campaign Web to manage and create your services such as newsletters, and to check the subscriptions or unsubscriptions to these services. Learn more: 

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

## Use plans, programs and campaigns 

Adobe Campaign allows you to configure your folder hierarchy for marketing plans and programs.

[Plans and programs documentation](../../v8/administration/plans-programs.md){target="_blank"}


### Create a campaign 

Adobe Campaign allows you to easily orchestrate your targeted marketing initiatives, using the built-in campaign management capability. With the ability to define a schedule, you can plan the duration and timing of your campaigns to align with strategic objectives and maximize audience engagement.

![Campaign flow](_assets/campaign-flow.png)

Follow the documentation below to learn more about campaigns : 

1. [Get started with campaigns](../../v8/campaigns/gs-campaigns.md){target="_blank"}
2. [Access and manage your campaigns](../../v8/campaigns/manage-campaigns.md){target="_blank"}
3. [Create your first campaign](../../v8/campaigns/create-campaigns.md){target="_blank"}


### Create a workflow

With workflows, you can orchestrate the full range of processes and tasks, improve the speed and scale of every aspect of your marketing campaigns, from creating segments and preparing messages to delivery. Plus, you can get your channels in sync with a single, easy-to-use interface for campaign orchestration.

Understand how workflows work and how to create a targeting workflow.

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

Get more details with the [Worklow documentation](../../v8/workflows/gs-workflows.md){target="_blank"}.

Adobe Campaign Web user interface features a query modeler in workflows that simplifies the process of filtering the database based on various criteria.
[Learn more about query modeler](../../v8/query/query-modeler-overview.md){target="_blank"}

To understand the purpose and functionality of each activity within your workflow, explore the detailed information available on [workflow activities](../../v8/workflows/activities/about-activities.md){target="_blank"}.

Maximize your workflow's efficiency by reviewing the [Guardrails and limitations for workflows](https://experienceleague.adobe.com/en/docs/campaign-web/v8/wf/guardrails){target="_blank"}.

>[!AVAILABILITY]
>
>1 - Workflow execution [history and logs](../../v8/workflows/start-monitor-workflows.md#logs-tasks){target="_blank"} are available in Adobe Campaign v8. 
Historical logs for workflows executed on ACS instance will not be migrated to Adobe Campaign v8.
2- Organizational Units will be mapped to concept of folder for mapping and ensuring similar access control.

## Create and manage deliveries

You can create standalone deliveries from the Deliveries left menu, or create deliveries in the context of a workflow, included or not in a campaign. Learn how to create a delivery:
[Delivery creation and management documentation](../../v8/msg/gs-deliveries.md){target="_blank"}

For an accelerated and improved design process, you can create delivery templates to easily reuse custom content and settings across your campaigns. This functionality enables you to standardize the creative look and feel, in order to be quicker in executing and launching campaigns.
[Delivery template documentation](../../v8/msg/delivery-template.md){target="_blank"}

Delivery settings are technical delivery parameters that are defined in the delivery template. They can be overloaded for each delivery. These settings are available from the Settings button available when editing a delivery or a delivery template.
[Delivery settings documentation](../../v8/advanced-settings/delivery-settings.md){target="_blank"}

Adobe Campaign Web dynamic content capabilities allows you to customize your content based on the information you have gathered about your recipients. By utilizing dynamic content, you ensure that your marketing efforts are more relevant, avoiding marketing unwanted or unnecessary products or services.
[Dynamic content documentation](../../v8/personalization/gs-personalization.md){target="_blank"}

Once your delivery content has been defined, you can use profiles and test profiles to preview and test it before sending the message. This is a crucial step to ensure that it is accurate but also free of errors both in content and personalization settings.
[Preview and test documentation](../../v8/preview-test/preview-test.md)

You can set the date and the exact time for sending your messages. By choosing the most appropriate time for your marketing message, you can maximise open rates. 
* Learn how to [schedule a stand-alone delivery](../../v8/msg/gs-deliveries.md#gs-schedule){target="_blank"}
* Learn how to [schedule a delivery in a workflow](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow){target="_blank"}

You can add offers to your deliveries in the Adobe Campaign Web user interface. These offers are available from the Offers left menu which lets you access to the list of offers. 
[Add offers to your messages](../../v8/msg/offers.md){target="_blank"}

>[!AVAILABILITY]
>
>Deliveries in draft state or finished state would be migrated. In transit / In progress / Cancelled / Retry in progress / Preparation error deliveries will be migrated to Adobe Campaign v8 but will have to be prepared again. 
Canceled / Retry in progress will be migrated as canceled deliveries.
Tracking links, mirror page URL links, subscription/un-subscription link will work as per as per AC standard. Read [Tracking and Monitoring](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}, [Branding](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} in Adobe Campaign.

### Email delivery

Learn how to create an email delivery from scratch, define the audience, design the content, simulate preview, and send a proof.
  
>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

Learn how to create your first targeted email. In this use case, you schedule the sending of an email to Silver and Gold loyalty members on a specific date.
[Create your first email documentation](../../v8/email/create-email.md){target="_blank"}

The detailed steps for sending an email delivery :

1. **Design and define content**

   Understand how to navigate the Email Designer. Learn how to structure and design an email from scratch, how to personalize, and test your email.

    >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

    The Email Designer enables you to create captivating, individually tailored emails through an intuitive drag-and-drop interface.
    [Email Designer documentation](../../v8/email/get-started-email-designer.md){target="_blank"}
    <br/>

   Learn how to create an email by uploading HTML, how to make it compatible with the Email Designer and how to convert it to a template.

    >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}
    
    A content fragment is a reusable component that can be referenced in one or more messages. Use [Content fragments](../../v8/content/fragments.md) to simplify the creation of your email delivery.
    <br/>

    For an accelerated and improved design process, you can create standalone templates to easily reuse custom content across Adobe Campaign. 
    [Create email templates](../../v8/email/create-email-templates.md){target="_blank"}

1. **Preview and test**

    Learn how to preview email message content and personalization, send test deliveries (proofs) and check the email rendering in popular desktop, mobile and web-based clients.

    >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **Send email and check logs**
    When you have defined your content, audience, and schedule, you are ready to prepare your email delivery.

   * [Prepare and send an email](../../v8/monitor/prepare-send.md){target="_blank"}
   * [Monitor delivery logs](../../v8/monitor/delivery-logs.md){target="_blank"}

     
### SMS delivery

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

### Create and manage push notifications

Push notifications are essential for reaching out to your mobile app users, even when they're not actively using your app. They serve various purposes like providing updates, driving specific actions, and notifying about deals.

Adobe Campaign v8 supports both Android&trade; and iOS Push Channel. To transition existing workflows and deliveries that are using the Push Channel, please connect with your Adobe Campaign Transition Manager.  

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

### Direct mail

Direct mail is an offline channel that allows you to produce files to mass deliver personalized letters to your customers such as postcards, flyers, or catalogs. When creating a direct mail delivery, Adobe Campaign automatically generates an extraction file containing all the targeted profiles and selected data, such as postal addresses and profile attributes.

1. [Create Direct Mail delivery](../../v8/direct-mail/create-direct-mail.md){target="_blank"} 
2. [Define the extraction file](../../v8/direct-mail/content-direct-mail.md){target="_blank"}  
3. [Preview and send](../../v8/direct-mail/send-direct-mail.md){target="_blank"}


## Create and manage landing pages

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


## Reporting

Adobe Campaign suite of reporting tools provides valuable insights into the effectiveness of your marketing efforts, allowing you to optimize your campaigns for maximum impact.
[Reporting documentation](../../v8/reporting/gs-reports.md){target="_blank"} 

Dynamic Reporting provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks.
[Dynamic reporting documentation](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} 

>[!AVAILABILITY]
>
>1 - [Dynamic reporting](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} can be used for reporting of email deliveries, campaign with email deliveries and transactional messages. Demographic analysis by Profile dimension is also available.  
2- [Adobe Campaign Web User Interface reporting](../../v8/reporting/campaign-reports.md){target="_blank"} is also available for all users transition from Adobe Campaign Standard to Adobe Campaign v8.

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
