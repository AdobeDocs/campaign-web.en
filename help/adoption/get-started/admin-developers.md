---
title: Get started with Adobe Campaign v8 for administrators and developers.
description: This tutorial gives an overview of the key administrative and data management functionality of Campaign v8. It is targeted for administrators and the technical marketer migrating from Campaign Standard to Campaign v8.
role: Admin, Developer
level: Beginner, Experienced
---

# Get started for admin/developers {#acs-gs-admin}

This page gives an overview of the key administrative and data management functionality of Campaign v8. It is for administrators and technical marketers transitioning from Campaign Standard to Campaign v8.

The major change for you is the introduction of the client console, the native application which communicates with the Adobe Campaign application server. 

The Campaign client console centralizes all capabilities and settings. It is stays synchronized with the Campaign Web User Interface, ensuring consitency acrouss both environments.

![](_assets/client_console.png){zoomable="yes"}

[Learn more about the client console user interface of Adobe Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access){target="_blank"} .

## Understand the Campaign v8 architecture {#acs-gs-admi-archi}

Campaign architecture is detailed in Campaign v8 (console) documentation. Learn basics in [this page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/general-architecture){target="_blank"}.

Useful link for you to start:

* Adobe Campaign components and global architecture are described in [this page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/ac-components){target="_blank"}.

* Refer to [Get Started with Campaign architecture](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture){target="_blank"} to understand the Campaign architecture before starting to structure your instance.

    Two deployment models are available: **Campaign FDA deployment** (P1-P3) and **Campaign Enterprise (FFDA)** deployment (P4). As a customer transitioning from Campaign Standard, your deployment model is **Campaign FDA**.

* Transactional messaging (Message Center) is the Campaign v8 module designed for managing triggered messages. It relies on a specific architecture model which is detailed in [this section](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture#transac-msg-archi){target="_blank"}.


## Install the client console {#acs-gs-admin-console}

Administration and configuration tasks are performed in the client console. The first step is to set up your environment. 

Campaign client console is a native application which communicates with the Adobe Campaign application server through standard internet protocols, such as SOAP and HTTP. Campaign client console centralizes all capabilities and settings, and requires minimal bandwidth as it relies on a local cache. Designed for easy deployment, Campaign client console can be deployed from an internet browser, updated automatically, and does not require any specific network configuration as it only generates HTTP(S) traffic.

The following video explains how to download and install the Adobe Campaign Client Console and manage your connection to your instance.

>[!VIDEO](https://video.tv.adobe.com/v/335375?quality=12&learn=on){transcript=true}

For more information, see [Connect to Campaign with the client console](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect){target="_blank"}.

Note that the client console must be installed in a supported environment. Learn more in [Campaign v8 (console) compatibility matrix](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/compatibility-matrix#ClientConsoleoperatingsystems){target="_blank"}.

## Discover the client console interface  {#acs-gs-ui}

Learn about the Adobe Campaign V8 user interface and how to navigate the main features with this tutorial video.

>[!VIDEO](https://video.tv.adobe.com/v/334496?quality=12&learn=on){transcript=true}

See [Work with the client console](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui){target="_blank"} for more details.

## Administrate the environment {#acs-gs-admin-env}

**TO UPDATE > Explain changes for ACS users**


Once the client console is installed, follow the steps in this documentation to create the connection to the application server: [Connection to the application server documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect#create-your-connection){target="_blank"}

Security practices are deeply ingrained into our internal software development and operations processes and tools and are rigorously followed by our cross-functional teams to prevent, detect, and respond to incidents in an expedient manner. Learn more in [Campaign Security best practices](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/privacy/security){target="_blank"}.

Adobe Campaign lets you define and manage the rights assigned to users. These permissions are defined by combining operator group permissions, named rights and permissions on folders. See the [User permissions documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.


### Campaign Control Panel {#acs-gs-admin-cp}

As for Campaign Standard, you can use the Control Panel to administrate your environment. Note that for v8, the Control Panel provides additional capabilities.

Campaign Control Panel helps you increase efficiency in your work as a product admin of Adobe Campaign, by allowing you to manage settings and track usages for each of your instances. Its intuitive interface lets you easily monitor usage of key assets, as well as perform administrative tasks such as IP addresses allow list addition, SFTP storage monitoring, key management, and more.

Learn more in the [Control panel tutorials](https://experienceleague.adobe.com/en/docs/control-panel-learn/tutorials/control-panel-overview){target="_blank"} and the [Control panel documentation](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html){target="_blank"}.

* **Add IP addresses** - Campaign Control Panel allows you to set up new connections to your instances by adding IP addresses ranges to the allow list. Learn more in the [IP allow listing documentation](https://experienceleague.adobe.com/en/docs/control-panel/using/instances-settings/ip-allow-listing-instance-access){target="_blank"}

* **Subdomain configuration** - You can configure a sub-section of your domain (technically a "DNS zone") for use with Adobe Campaign. 
Learn more in the [Subdomain delegation documentation](https://experienceleague.adobe.com/en/docs/control-panel/using/subdomains-and-certificates/subdomains-branding){target="_blank"}

* **Manage SFTP servers** - In the Control Panel, you can interact with all SFTP servers that are connected to Campaign instances that you have access to. Learn more in the [SFTP management documentation](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/about-sftp-management){target="_blank"}


### Audit trail {#acs-gs-admin-audit-trail}

As already available in Campaign Standard, the Audit trail can be used in Campaign v8 to access the complete history of changes made within your instance.

In Adobe Campaign Web User Interface, the Audit trail capability provides users with full visibility into all modifications made to important entities within your instance, typically those that significantly impact a smooth operation of the instance. Learn more in the [Audit trail documentation](../../v8/reporting/audit-trail.md)

### Data packages {#acs-gs-admin-audit-packages}

Similar to what can be achieved in Campaign Standard, administrators can define packages to exchange resources between different Adobe Campaign instances through structured XML files. These can be configuration parameters or data.

You can use data packages to export and import your platform custom settings and data. A package can contain different types of configurations and components, filtered or not. Learn how to work with data packages in Campaign v8 in [this documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/packages){target="_blank"}.

<!--
MISSING LINKS: 

- System options
- Data Encryption/Decryption-->

## Set up user interface {#acs-gs-admin-ui}

Several options are available to you to customize the user interface in the client console, such as:

* **List and data display** - Guidelines for managing user interface settings like lists, units, or data display are available in this document: [User interface settings documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings){target="_blank"}

* **Folder management** - Folders are objects in Adobe Campaign that allow you to organize your components and data. Learn how to [work with folders](../../v8/get-started/work-with-folders.md).

* **Custom fields** - Custom fields are additional attributes added to the out-of-the-box schemas through the Adobe Campaign console. These custom fields are displayed in various screens, for example the details of a profile or a test profile. Learn more in the [custom fields configuration documentation](../../v8/administration/custom-fields.md).

## Set up the branding {#acs-gs-admin-branding}

Every company has brand guidelines that define both visual elements and technical details. As for Adobe Campaign Standard, Adobe Campaign v8 helps you manage these guidelines centrally, so you can present a consistent brand image to your customers in everything you do, from logos in emails to the URLs and domains used in your campaigns.

Learn more in the [Branding documentation](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"}

## Understand data model creation {#acs-gs-admin-data-model-creation}

Similar to Campaign Standard, Adobe Campaign v8 comes with its pre-defined data model. Adobe Campaign relies on a Cloud database containing tables that are linked together. Learn more in the [Data model documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/datamodel){target="_blank"}.

A schema is an XML document associated with a database table. It defines data structure and describes the SQL definition of the table. See the [Schemas creation documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

Learn how to create a schema and how to extend an existing schema in Campaign v8 in this video:

>[!VIDEO](https://video.tv.adobe.com/v/337939?quality=12&learn=on){transcript=true}

Similar to the capabilities available in Campaign Standard, you can create custom resources. IN Campaign v8, custom resources are custom or extended **schemas**. 

+ Learn how to work with schema in [this page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.

* Learn how to extend an existing schema in [this page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema){target="_blank"}.

* Learn how to create an new schema in [this page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/create-schema){target="_blank"}.

* When you create or extend a schema, you need to create or modify the associated input forms to make those changes visible to end-users. An input form lets you edit an instance associated with a data schema from the Adobe Campaign client console. The form is identified by its name and namespace. See the [Input forms creation documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/forms){target="_blank"}.

## Understand data management {#acs-gs-admin-data-management}

Same as with Adobe Campaign Standard, Adobe Campaign v8 includes a workflow module that empowers you to orchestrate the full range of processes and tasks across the different modules of the application server. This comprehensive graphical environment lets you design processes including segmentation, campaign execution, file processing, human participation, etc. The workflow engine executes and tracks these processes. Learn how to start with workflows in Campaign v8 in [this documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/workflows){target="_blank"}. 

See links to other useful resources below:

* Learn what targeting dimensions and working tables are, and how Adobe Campaign manages data across different data sources in this video:

    >[!VIDEO](https://video.tv.adobe.com/v/339992?quality=12&learn=on){transcript=true}

* Campaign helps you add contacts to the Cloud database. You can load a file, schedule and automate multiple contact updates, collect data on the Web, or enter profile information directly into the recipient table.  Learn more in the [Import data (console) documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/import){target="_blank"}.

* You can easily export your different reports to PDF or CSV format, which enables you to share, manipulate, or print them. Learn more in the [Export data documentation](../../v8/reporting/export-reports.md).

## REST APIs {#acs-gs-admin-apis}

Campaign REST APIs are aimed at letting you create integrations for Adobe Campaign and build your own ecosystem by interfacing Adobe Campaign with the panel of technologies that you use.

As a Campaign Standard user transitioning to Campaign v8, REST APIs are available to you. 

Learn more in the [Rest API documentation](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/get-started-apis){target="_blank"}.

Note that some recommendations and limitations apply to REST APIs when transitioning from Campaign Standard to Campaign v8. They are listed in [this page](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/limitations){target="_blank"}.

>[!AVAILABILITY]
>
>* PKEYs values change between existing Campaign Standard instance and migrated Campaign v8 instance. In case PKEYs are being stored in external database then the implementation needs to change in a way that they need to call Adobe Campaign v8 main APIs which provides pkeys / hrefs links with PKEYs and sub sequent API calls need to be dynamically formed by consuming the pkeys /hrefs from previous API calls​
>
>* Administrator product profile and Message center product profile: a new product profile needed for accessing transactional APIs from Real-Time instance which is different from Campaign Standard. This is added to Campaign Standard existing or pre-created technical accounts. Post transition, as an administrator, you should review product profile mapping and assign to the needed product profile if you do not want Administrator product profile mapping with your technical account. After the transition, for any future new integrations, use Campaign v8 tenant ID in the REST URL instead of the previous Campaign Standard tenant ID.​
>
>TO REMOVE?? :
>
>* In Campaign v8, for the same body where vehicle linked to profile,​ we would get an error firstName property is not valid for `cusVehicle` but a request body with just the attributes without link works fine. `{ "vehicleNumber": "20009", "vehicleName": "Model E", "vehicleOwner":{   "firstName":"tester 11", "lastName":"Smith 11" } }​`
>
>* Timezone is shown to user as part of `profileAndServicesExt/profile` REST API call and not `profileAndServices/profile` REST API call since it is being added in an extended schema as part of data migration.​
>
>* The `ccpaOptOut` is only shown to user as part of `profileAndServicesExt/profile` REST API call and not `profileAndServices/profile` REST API call since it is being added in an extended schema as part of data migration. 
>

## About delivery management - TO REMOVE?

Same as in Adobe Campaign Standard, in Campaign v8, typology rules are business rules that allow you to perform checks and filtering on your message before sending it. 

Campaign Optimization is the Adobe Campaign module which lets you control, filter and monitor the sending of deliveries. To avoid conflicts between campaigns, Adobe Campaign can test various combinations by applying specific constraint rules. This guarantees that the messages sent meet the needs and expectations of customers and company communication policies. Learn more in the [Typology rules documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}


Quarantine is the way to manage the invalid addresses in deliveries. See [Quarantine documentation](../../v8/audience/quarantine.md)


## Working with templates - TO REMOVE?

Campaign templates contain pre-configured settings which can be reused for creating new campaigns. A set of built-in templates is available to help you get started.
See [Campaign templates documentation in Web User Interface](../../v8/campaigns/manage-campaigns.md#manage-campaign-templates) and [Campaign templates documentation in Client Console](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates){target="_blank"}

For an accelerated and improved design process, you can create delivery templates to easily reuse custom content and settings across your campaigns. This functionality enables you to standardize the creative look and feel, in order to be quicker in executing and launching campaigns.
[Delivery template documentation](../../v8/msg/delivery-template.md)

Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows.
[Workflow template documentation](../../v8/workflows/create-workflow.md)

Learn how created dynamic content blocks and how to use them to personalize the content of your email delivery in this video:

>[!VIDEO](https://video.tv.adobe.com/v/342088?quality=12&learn=on){transcript=true}

You can design your landing page content, and save it for future reuse. See the [landing page template documentation](../../v8/landing-pages/lp-templates.md).

Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message. See the [Transactional messaging template documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional-template)

Using a workflow template is a best practice if you need to regularly import files with the same structure. See the [Import template documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/use-cases/data-management/recurring-import-workflow){target="_blank"}

## Use subscription services - TO REMOVE?

Learn how to setup and manage subscriptions and target subscribers.

>[!VIDEO](https://video.tv.adobe.com/v/334305?quality=12&learn=on){transcript=true}

Manage and create your services such as newsletters, and check the subscriptions or unsubscriptions to these services. See the [subscription services documentation](https://experienceleague.adobe.com/en/docs/campaign-web/v8/audiences/work-with-services/manage-services){target="_blank"}


## Configure delivery channels - TO REMOVE?

External accounts are used by technical processes such as technical workflows or campaign workflows. For example, when setting up a file transfer in a workflow or a data exchange with any other application (Adobe Target, Experience Manager, etc.), you need to select an external account. See [External account configuration](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts){target="_blank"}

<!--
**Email**

MISSING LINKS :
- general email channel parameters 
- email routing accounts 
- email processing rules 
- email properties
-->

**SMS** might be limited to sending short text messages with no formatting but its simplicity makes it a valuable communication channel. See [how to configure SMS channel](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/config-sms/sms-mid-sourcing){target="_blank"}

TO BE CHANGED WHEN NEW DOC RELEASED

**Direct mail** is an offline channel that allows you to produce files to mass deliver personalized letters to your customers such as postcards, flyers, or catalogs.
[Get started with Direct Mail deliveries](../../v8/direct-mail/gs-direct-mail.md)
<!--
MISSING LINKS: 
- Setting external account 
- Adding vender details etc. -->

<!--
**Mobile app**
MISSING LINKS: 
- Configuring a mobile application using AEP SDKs 
- Sync Mobile app AEPSDK  
- Setting up your application in Adobe Campaign 
- Channel-specific application configuration
-->

## Manage Adobe Campaign integrations

**TO UPDATE > Explain changes for ACS users**

You can connect your Campaign environment with Adobe Experience Cloud solutions and apps to combine capabilities. See [Campaign connection to other solutions documentation](../../v8/integrations/integration.md)

Adobe Campaign v8 comes with several connectors that allow you to communicate with external applications, connect to database engines, share and synchronize data. These connections are configured by Adobe.
        
Here are the available integrations and related links into Campaign (console) documentation:

* [Adobe Analytics](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aa){target="_blank"}: This integration sends indicators and attributes of email campaigns delivered by Adobe Campaign to Adobe Analytics
        
* [Adobe Experience Cloud triggers](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-triggers){target="_blank"}: You can use Experience Cloud Triggers to connect data between Adobe Campaign and Adobe Analytics using the pipeline. The pipeline retrieves user's actions or triggers from your website. A cart abandonment is an example of trigger. Triggers are processed in Adobe Campaign to send emails in near real time.
        
* [Adobe Experience Manager](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aem){target="_blank"}: Integration between Adobe Campaign and Adobe Experience Manager allows you to manage the content of your email deliveries as well as your forms directly in Adobe Experience Manager.

* [Adobe Experience Platform](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aep/ac-aep){target="_blank"}: With this integration, you can: send Adobe Experience Platform audiences over to Adobe Campaign, and send back delivery and tracking logs into Adobe Experience Platform for analysis purpose, bring Adobe Experience Platform profile attributes into Adobe Campaign and have a sync process in place so that they can be updated on a regular basis.
        
* [Adobe Journey Optimizer](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-ajo){target="_blank"}: Integration between Adobe Campaign and Adobe Journey Optimizer allows you orchestrate customer journeys in Adobe Journey Optimizer and send emails, push notifications and/or SMS using Adobe Campaign Transactional Messaging capabilities.
        
* [Adobe Target](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-at){target="_blank"}: This integration helps to include an offer from Adobe Target in an Adobe Campaign email delivery.

* [Adobe Workfront](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-workfront){target="_blank"}: Speed up campaign delivery by pairing Campaign with Adobe Workfront. This integration make it easy for cross-channel teams to intake, collaborate, and execute.

>[!AVAILABILITY]
>
>Analytics & Audience configurations and data will be automated migration.


## Use transactional messages

**TO UPDATE > Explain changes for ACS users**


Transactional messaging (Message Center) is a Campaign module designed for managing trigger messages. These notifications are generated from events triggered from information systems, and can be: invoice, order confirmation, shipping confirmation, password change, product unavailability notification, account statement, website account creation, etc.

See the [Transactional messages documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional){target="_blank"}


## Use reporting

**TO UPDATE > Explain changes for ACS users __ NO CHANGE?**

Adobe Campaign provides a set of reporting tools [Reporting configuration documentation](../../v8/reporting/gs-reports.md){target="_blank"}
    
Dynamic Reporting provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. See the [Dynamic reporting documentation](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}

Reports can also be created and managed based on profile data created during the recipient schema extension. Learn more in the following documentation: [Creating a profile dimension](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/customizing-reports/creating-a-custom-profile-dimension){target="_blank"}

