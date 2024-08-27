---
title: Get started with Adobe Campaign v8 for administrators and developers.
description: This tutorial gives an overview of the key administrative and data management functionality of Campaign v8. It is targeted for administrators and the technical marketer migrating from Campaign Standard to Campaign v8.
role: Admin, Developer
level: Beginner, Experienced
jira:  KT-15787
---

# Get started for administrators and developers

This tutorial gives an overview of the key administrative and data management functionality of Campaign v8. It is for administrators and technical marketers migrating from Campaign Standard to Campaign v8.

The major change for you is the introduction of the client console, the native application which communicates with the Adobe Campaign application server. 

The Campaign client console centralizes all capabilities and settings. It is stays synchronized with the Campaign Web User Interface, ensuring consitency acrouss both environments.

![](_assets/client_console.png){zoomable="yes"}

[Learn more about the client console user interface of Adobe Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access).

## Understand the Campaign v8 Architecture

See [Get Started with Campaign architecture](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture){target="_blank"} to understand the Campaign architecture before starting to structure and organize your instance.

Review the [Campaign implementation guidelines](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/implement/implement){target="_blank"} to learn how to adjust Adobe Campaign to the requirements of your company and structure and organize your implementation.

## Install the client console

The main administration and configuration tasks are performed in the [Admin Console]. The first step is to set up your environment. The following video explains how to download and install the Adobe Campaign Client Console and manage your connection to your instance.

>[!VIDEO](https://video.tv.adobe.com/v/335375?quality=12&learn=on){transcript=true}

For more information, see [Connect to Campaign with the client console](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect){target="_blank"}.

## Discover the client console interface

Learn about the Adobe Campaign V8 user interface and how to navigate the main features with this tutorial video.

>[!VIDEO](https://video.tv.adobe.com/v/334496?quality=12&learn=on){transcript=true}

See [Work with the client console](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui){target="_blank"} for more details.

## Administrate the environment 

Once the client console is installed, follow the steps in this documentation to create the connection to the application server.<br/>
[Connection to the application server documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect#create-your-connection){target="_blank"}

Adobe Campaign lets you define and manage the rights assigned to users. These permissions are defined by combining operator group permissions, named rights and permissions on folders.
[User permissions documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}

The Adobe Campaign Control Panel allows Adobe Campaign administrators to monitor key assets and perform administrative tasks, such as managing the SFTP storage by instance, managing GPG keys, or subdomains and certificates.
[Control panel tutorials](https://experienceleague.adobe.com/en/docs/control-panel-learn/tutorials/control-panel-overview){target="_blank"}

Control Panel allows you to set up new connections to your instances by adding IP addresses ranges to the allow list.
[IP allow listing documentation](https://experienceleague.adobe.com/en/docs/control-panel/using/instances-settings/ip-allow-listing-instance-access){target="_blank"}

Subdomain configuration allows you to configure a sub-section of your domain (technically a "DNS zone") for use with Adobe Campaign.
[Subdomain delegation documentation](https://experienceleague.adobe.com/en/docs/control-panel/using/subdomains-and-certificates/subdomains-branding){target="_blank"}

In the Control Panel, you can interact with all SFTP servers that are connected to Campaign instances that you have access to.
[SFTP management documentation](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/about-sftp-management){target="_blank"}

In Adobe Campaign Web User Interface, the Audit trail feature provides users with full visibility into all modifications made to important entities within your instance, typically those that significantly impact a smooth operation of the instance.
[Audit trail documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/audit-trail){target="_blank"}

You can use data packages to export and import your platform custom settings and data. A package can contain different types of configurations and components, filtered or not.
[Package import/export](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/packages){target="_blank"}

Rest API
**TO BE CHANGED** 
1. PKEYs values will change between existing ACS instance Vs migrated ACC instance.  In case  PKEYs are being stored in external DB then the implementation needs to change in a way that they need to call AC v8 main APIs which provides pkeys / hrefs links with pkeys and sub sequent API calls need to be dynamically formed by consuming the pkeys /hrefs from previous API calls​

1. Administrator product profile + Message center product profile, a new product profile needed for accessing transactional APIs from RT instance which is different from ACS. This will be added to ACS existing or pre-created technical accounts. Post migration ACS users should review product profile mapping and assign to the needed product profile if they don't want Admin product profile mapping with their technical account. After migration, any future new integrations we recommend customer to use AC v8 tenant id in the REST URL instead of the previous ACS tenant id.​

1. In AC v8 for the same same body where vehicle linked to profile​
we would get an error firstName property is not valid for cusVehicle but a request body with just the attributes without link works fine!​

{ "vehicleNumber": "20009", "vehicleName": "Model E", "vehicleOwner":{   "firstName":"tester 11", "lastName":"Smith 11" } }​

1. Timezone will only be shown to user as part of profileAndServicesExt/profile rest api call and not profileAndServices/profile rest api call since it is being added in an extended schema as part of data migration.​

1. ccpaOptOut will only be shown to user as part of profileAndServicesExt/profile rest api call and not profileAndServices/profile rest api call since it is being added in an extended schema as part of data migration. 

## Set up user interface

Guidelines for managing user interface settings like lists, units, or data display.[User interface settings documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings){target="_blank"}

Custom fields are additional attributes added to the out-of-the-box schemas through the Adobe Campaign console. These custom fields are displayed in various screens, for example the details of a profile or a test profile.
[Custom fields configuration documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/conf/custom-fields){target="_blank"}

## Set up the branding data management

Every company has brand guidelines that define both visual elements and technical details. Adobe Campaign helps you manage these guidelines centrally, so you can present a consistent brand image to your customers in everything you do, from logos in emails to the URLs and domains used in your campaigns.
[Branding documentation](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"}

## Understand data model creation

Adobe Campaign comes with a pre-defined data model. This section gives some details on the built-in tables of the Adobe Campaign data model and their interaction. Adobe Campaign relies on a Cloud database containing tables that are linked together.
[Data model documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/datamodel){target="_blank"}

A schema is an XML document associated with a database table. It defines data structure and describes the SQL definition of the table.<br/>
[Schemas creation documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

Learn how to create a schema and how to extend an existing schema.

>[!VIDEO](https://video.tv.adobe.com/v/337939?quality=12&learn=on){transcript=true}

When you create or extend a schema, you need to create or modify the associated input forms to make those changes visible to end-users. An input form lets you edit an instance associated with a data schema from the Adobe Campaign client console. The form is identified by its name and namespace.<br/>
[Input forms creation documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/forms){target="_blank"}

## Understand data management

Learn what targeting dimensions and working tables are, and how Adobe Campaign manages data across different data sources.

>[!VIDEO](https://video.tv.adobe.com/v/339992?quality=12&learn=on){transcript=true}

Use Adobe Campaign workflows to improve the speed and scale of every aspect of your marketing campaigns, from creating segments and preparing messages to delivery.
[Workflows documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/workflows){target="_blank"}
    
Campaign helps you add contacts to the Cloud database. You can load a file, schedule and automate multiple contact updates, collect data on the Web, or enter profile information directly into the recipient table.
[Import data documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/import){target="_blank"}

You can easily export your different reports to PDF or CSV format, which enables you to share, manipulate, or print them.
[Export data documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/export-reports){target="_blank"}

Quarantine is the way to manage the invalid addresses in deliveries.
[Quarantine documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/audiences/quarantine){target="_blank"}

## About delivery management

Campaign Optimization is the Adobe Campaign module which lets you control, filter and monitor the sending of deliveries. To avoid conflicts between campaigns, Adobe Campaign can test various combinations by applying specific constraint rules. This guarantees that the messages sent meet the needs and expectations of customers and company communication policies.
[Typology rules documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

All marketing campaigns are based on a template, which stores main characteristics and capabilities. Campaign comes with a built-in template to create campaigns. This template has all functionalities enabled: Documents, Seed addresses, Approvals, Delivery outlines, etc.
[Campaign template documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates){target="_blank"}

Learn how to setup and manage subscriptions and target subscribers.
[Subscription services tutorial video](https://experienceleague.adobe.com/en/docs/campaign-learn/tutorials/sending-messages/configure-and-manage-subscription-services){target="_blank"}

## Working with templates

Campaign templates contain pre-configured settings which can be reused for creating new campaigns. A set of built-in templates is available to help you get started.
[Campaign templates documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/campaigns/manage-campaigns#manage-campaign-templates){target="_blank"}

For an accelerated and improved design process, you can create delivery templates to easily reuse custom content and settings across your campaigns. This functionality enables you to standardize the creative look and feel, in order to be quicker in executing and launching campaigns.
[Delivery template documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/delivery-template){target="_blank"}

Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows.
[Workflow template documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/wf/create-workflow/create-workflow){target="_blank"}

Learn how created dynamic content blocks and how to use them to personalize the content of your email delivery.
[Dynamic content block template documentation](https://experienceleague.adobe.com/en/docs/campaign-learn/tutorials/content-creation/email/personalize-using-dynamic-content-blocks){target="_blank"}

Once you designed your landing page content, you can save it for future reuse.
[Landing page template documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/landing-pages/lp-templates){target="_blank"}

A content fragment is a reusable component that can be referenced in one or more messages. When modifying a fragment, every content using it is updated.
[Content fragments documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments){target="_blank"}

Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message.
[Transactional messaging template documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional-template){target="_blank"}

Using a workflow template is a best practice if you need to regularly import files with the same structure.<br/>
[Import template documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/use-cases/data-management/recurring-import-workflow){target="_blank"}
    

## Use subscription services

Use Adobe Campaign Web to manage and create your services such as newsletters, and to check the subscriptions or unsubscriptions to these services.<br/>
[Subscription services documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/audiences/work-with-services/manage-services){target="_blank"}


## Send deliveries

External accounts are used by technical processes such as technical workflows or campaign workflows. For example, when setting up a file transfer in a workflow or a data exchange with any other application (Adobe Target, Experience Manager, etc.), you need to select an external account.
[External account configuration](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts){target="_blank"}

Learn how to create your first targeted email. In this use case, you schedule the sending of an email to Silver and Gold loyalty members on a specific date.
[Create your first email](https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/email/create-email){target="_blank"}

SMS might be limited to sending short text messages with no formatting but its simplicity makes it a valuable communication channel.
[SMS connector protocol and settings](https://experienceleague.adobe.com/en/docs/campaign-classic/using/sending-messages/sending-messages-on-mobiles/sms-protocol#sending-messages){target="_blank"}

Direct mail is an offline channel that allows you to produce files to mass deliver personalized letters to your customers such as postcards, flyers, or catalogs.
[Get started with Direct Mail deliveries](https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/direct-mail/gs-direct-mail){target="_blank"}

## Manage Adobe Campaign integrations

You can connect your Campaign environment with Adobe Experience Cloud solutions and apps to combine capabilities.
[Campaign connection to other solutions documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/integrations/integration){target="_blank"}

Adobe Campaign v8 comes with several connectors that allow you to communicate with external applications, connect to database engines, share and synchronize data. These connections are configured by Adobe.

>[!AVAILABILITY]
>
>Analytics & Audience configurations and data will be automated migration.
        
Here are the possible integrations:

* [Adobe Analytics](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aa){target="_blank"}: This integration sends indicators and attributes of email campaigns delivered by Adobe Campaign to Adobe Analytics
        
* [Adobe Experience Cloud triggers](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-triggers){target="_blank"}: You can use Experience Cloud Triggers to connect data between Adobe Campaign and Adobe Analytics using the pipeline. The pipeline retrieves user's actions or triggers from your website. A cart abandonment is an example of trigger. Triggers are processed in Adobe Campaign to send emails in near real time.
        
* [Adobe Experience Manager](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aem){target="_blank"}: Integration between Adobe Campaign and Adobe Experience Manager allows you to manage the content of your email deliveries as well as your forms directly in Adobe Experience Manager.

* [Adobe Experience Platform](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aep/ac-aep){target="_blank"}: With this integration, you can: send Adobe Experience Platform audiences over to Adobe Campaign, and send back delivery and tracking logs into Adobe Experience Platform for analysis purpose, bring Adobe Experience Platform profile attributes into Adobe Campaign and have a sync process in place so that they can be updated on a regular basis.
        
* [Adobe Journey Optimizer](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-ajo){target="_blank"}: Integration between Adobe Campaign and Adobe Journey Optimizer allows you orchestrate customer journeys in Adobe Journey Optimizer and send emails, push notifications and/or SMS using Adobe Campaign Transactional Messaging capabilities.
        
* [Adobe Target](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-at){target="_blank"}: This integration helps to include an offer from Adobe Target in an Adobe Campaign email delivery.

* [Adobe Workfront](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-workfront){target="_blank"}: Speed up campaign delivery by pairing Campaign with Adobe Workfront. This integration make it easy for cross-channel teams to intake, collaborate, and execute.
        
>[!AVAILABILITY]
>
>Analytics & Audience will be automated migration.

## Use transactional messages

Transactional messaging (Message Center) is a Campaign module designed for managing trigger messages. These notifications are generated from events triggered from information systems, and can be: invoice, order confirmation, shipping confirmation, password change, product unavailability notification, account statement, website account creation, etc.
TO BE CHANGED New Web UI – Not console: [Transactional messages documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional){target="_blank"}


## Use reporting

Adobe Campaign provides a set of reporting tools [Reporting configuration documentation](../../v8/reporting/gs-reports.md){target="_blank"}
    
TO BE CHANGED : Dynamic Reporting provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks.
[Dynamic reporting documentation](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}
