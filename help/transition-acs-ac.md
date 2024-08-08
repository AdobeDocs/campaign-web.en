---
title: Transition from Adobe Campaign Stand to Adobe Campaign v8
description: Learn how to transition smoothly to Adobe Campaign v8
---

# Transition from Adobe Campaign Standard to Adobe Campaign v8

## Introduction
This is a guide for Adobe Campaign Standard customers about the transition to Adobe Campaign v8. 

Adobe Campaign v8 brings significant infrastructure and performance for enterprise scale. It provides robust support for cross-channel campaign management, and communicates with other Adobe solutions, including Adobe Experience Platform.

## What's new?

Get a glimpse of what you get with Adobe Campaign v8!

### Enhancement with Adobe Campaign v8

* **Web User Interface**

Adobe Campaign v8 is available both with client console and web user interface. With the client console, Adobe Campaign v8 has a Web User Interface that will give a better experience and easier adoption to Adobe Campaign Standard users.

[Learn more about Adobe Campaign Web User Interface](v8/campaign-web-home.md)

![](assets/home.png){zoomable="yes"}


* **Performance**

Adobe Campaign v8 can leverage cloud scale database technologies and dramatically improves its performance. It brings the concept of Full Federated Data Access (FFDA): all data is now remote on the Cloud Database.

This redesigned architecture allows :

* *More Storage*: Up to **6TB in total database storage** across production and staging instances
* *More Speed and Scale*
    * Increase batch throughput: up to **15M/h**
    * Increase transactional throughput: up to **180K/h**
* *Snowflake via FDA*
    * Permit offload high-volume data 
    * Increase storage, faster segmentations, queries, reports and deliveries

### New features on Adobe Campaign v8

* **Rich push**

Rich push notifications can be handled with Adobe Campaign v8.  

![](v8/push/assets/rich_push.png){zoomable="yes"}

You can define your content using the given templates. According to your customer system, you can design your push accordingly.

For [Android](v8/push/rich-push.md) users, you have :

* *Default* allows you to send notifications with a simple icon and an accompanying image.

* *Basic* can include text, images, and buttons in your notifications.

* *Carousel* enables you to send notifications with text and multiple images that users can swipe through.

* *Icon buttons* allows you to send notifications with an icon and a corresponding image.

* *Input box* gathers user input and feedback directly through the notification.

* *Product catalog* displays a variety of product images.

* *Product rating* allows users to give feedback and rate products. 

* *Timer* includes a live countdown timer in your notifications.

* *Zero Bezel* uses the entire background surface for an image, with text overlaid seamlessly.

For [iOs](v8/push/rich-push.md), you have :

* *Default* allows you to send notifications with a simple icon and an accompanying image.

* *Basic* can include text, images, and buttons in your notifications.

* *Carousel* enables you to send notifications with text and multiple images that users can swipe through.

* *Timer* includes a live countdown timer in your notifications.

Push notifications are essential for reaching out to your mobile app users, even when they're not actively using your app.

* **Adobe Experience Manager as a Cloud Services**

Adobe Campaign v8 is natively integrated with Adobe Experience Manager as a Cloud Services. It helps you provide your customers with personalized, content-led experiences. 

This feature is available for :
* Asset management : The left pane of the email designer gives you a way to find easily assets and customize it. 
[Learn more here](v8/campaign-web-home.md)
![](v8/integrations/assets/assets_6.png){zoomable="yes"}

- Email template import : You can browse through AEM templates and select one to import to Campaign. 
![](v8/integrations/assets/aem_6.png){zoomable="yes"}

Adobe Experience Manager as a Cloud Services provides cloud-native agility to accelerate time to value and is extensible to meet your unique business requirements.

### AI assistant (bêta)

Adobe Campaign v8 provides an AI assistant to help you generate impactful content in an efficient and quick manner. 

![](v8/email/assets/full-email-1.png){zoomable="yes"}

AI Assistant revolutionizes the way you create professional and brand-consistent content across channels. With advanced GenAI models and deep understanding of your brand guidelines, AI Assistant auto-generates personalized, engaging, and effective content based on the marketing objective with content optimized for brand outlined styles, layouts, tone, and more.

AI Assistant makes the creation and execution of marketing campaigns intuitive, simple and hassle-free while saving time, improving efficiency, and driving better results.

![](v8/email/assets/full-email-2.png){zoomable="yes"}

It provides variant of email templates and generates and re-generates images.

Adobe Campaign v8 has AI assistant available for [Email](v8/email/generative-email.md), [SMS](v8/email/generative-sms.md), and [Push](v8/email/generative-push.md).

### Managed Services

Adobe Campaign v8 is available as a Managed Cloud Service, providing proactive oversight, timely alerting, and service governance. Adobe Managed Cloud Service provides marketers with a more agile, secure and scalable cross-channel campaign management solution with a low total cost of ownership. The new offering combines services with proactive oversight and timely alerting.

The managed services approach enables marketers to take advantage of the operational scale and economics of cloud infrastructure without the need for heavy support from internal IT resources. Adobe consulting and implementation teams work with you to assess your marketing plans, existing practices, data requirements, and messaging volume, and then they recommend the most appropriate service, support, and deliverability packages. The Adobe Campaign Managed Cloud Services team can then monitor and report on campaign performance, brand reputation, customer experience metrics, and more.

Read out this whitepaper to [learn more about the business value of Adobe Campaign Managed Cloud Services](https://experienceleague.adobe.com/docs/campaign/assets/IDC-Report-BusinessValueOfAdobeCampaign.pdf?lang=en).


## Brief experiences differences between Campaign Standard and Campaign v8

### Marketer experiences

* **The UI**

Adobe Campaign v8 VS web UI

* **The terminology**



### Administrator experiences

* **The client console**

## Migration video

Video to upload on https://publish.tv.adobe.com/buckets

To check

https://adobe-my.sharepoint.com/personal/ssahai_adobe_com/_layouts/15/stream.aspx?id=%2Fpersonal%2Fssahai%5Fadobe%5Fcom%2FDocuments%2FDocuments%2FFeatures%2FEuropa%20%2D%20ACS%20to%20ACC%2FDemos%2FEuropa%2EDemo%2EApril%2Emov&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Ef947ff92%2Ddbc6%2D4de2%2D99be%2Db8027acba5db&OR=Teams%2DHL&CT=1722944686104&clickparams=eyJBcHBOYW1lIjoiVGVhbXMtRGVza3RvcCIsIkFwcFZlcnNpb24iOiI1MC8yNDA2MjcyNDgxNyIsIkhhc0ZlZGVyYXRlZFVzZXIiOmZhbHNlfQ%3D%3D

## Marketer documentations table

<table style="table-layout:fixed">
  <tr style="border: 1;">
    <td align="center"><strong>Activity</strong></td>
    <td align="center"><strong>Documentation link</strong></td>
    <td align="center"><strong>Notes</strong></td>
  </tr>
  <tr style="border: 1;">
    <td>
        Discover the interface
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web-learn/tutorials/getting-started/explore-the-web-ui">Interface tutorial video</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/start/user-interface">Interface documentation</a>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Use plans, programs, campaigns</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/campaigns/plans-programs">Plans and programs documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/campaigns/gs-campaigns">Campaigns documentation</a>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Create and manage profiles and audiences </div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web-learn/tutorials/profiles-and-audiences/explore-profiles">Profiles tutorial video</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web-learn/tutorials/profiles-and-audiences/manage-and-build-audiences">Audiences tutorial video</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/audiences/gs-audiences-recipients">Profiles and audiences documentation</a>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Configure workflows </div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web-learn/tutorials/workflows/create-a-targeting-workflow">Targeting workflow tutorial video</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview">Query modeler documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/wf/gs-workflows">Workflows documentation</a>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Work with deliveries</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/gs-deliveries">Delivery creation and management documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/delivery-template">Delivery template documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/delivery-settings">Delivery settings documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/dynamic-content/gs-personalization">Dynamic content documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/preview-test/preview-test">Preview and test documentation</a>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Send email</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web-learn/tutorials/messages-and-deliveries/create-an-email-delivery">Email creation tutorial video</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/email/create-email">Email creation documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/email-design/get-started-email-designer">Email designing documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web-learn/tutorials/messages-and-deliveries/preview-and-proof-an-email-delivery">Email preview and proof tutorial video</a>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Send SMS</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/sms/gs-sms">SMS documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Send push notification</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/push/gs-push">Push notification documentation</a><br/>
        Rich push documentation:<br/>
        - <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/push/rich-push/rich-push">For Android</a><br/>
        - <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/push/rich-push/rich-push-ios">For iOS</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Send direct mail</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/msg/direct-mail/gs-direct-mail">Direct mail documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Create landing page</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/landing-pages/get-started-lp">Landing page documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Use reporting</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/gs-reports">Reporting documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports">Delivery reports documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting">Dynamic reporting documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
</table>

## Administrator documentations table

<table style="table-layout:fixed">
  <tr style="border: 1;">
    <td align="center"><strong>Activity</strong></td>
    <td align="center"><strong>Documentation link</strong></td>
    <td align="center"><strong>Notes</strong></td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Understand general architecture</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/general-architecture">Global principles documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/fda-deployment">Campaign FDA deployment documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/ffda/enterprise-deployment">Enterprise FFDA deployment documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/ac-components">Campaign components and processes documentation</a>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Know implementation steps</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/implement/implement">Campaign implementation guidelines documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Install client console</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-learn/tutorials/getting-started/install-and-set-up-the-adobe-campaign-client-console">Install and setup tutorial video</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect">Client console installation documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Administate environment</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect#create-your-connection">Connection to the application server documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/privacy/security ">Security best practices</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions">User permissions documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/control-panel-learn/tutorials/control-panel-overview">Control panel tutorials</a>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Discover console client interface</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-learn/tutorials/getting-started/explore-the-adobe-campaign-user-interface">Console client interface tutorial video</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui">Client console interface documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Set up user interface</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings">User interface settings documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/conf/custom-fields">Custom fields configuration documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Understand data model creation</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/datamodel">Data model documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas">Schemas creation documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/forms">Input forms creation documentation</a>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Understand data management</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/workflows">Workflows documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/import">Import data documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>About delivery management</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies">Typology rules documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates">Campaign template documentation</a><br/>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-learn/tutorials/sending-messages/configure-and-manage-subscription-services">Subscription services tutorial video</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Manage Adobe Campaign integrations</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/integrations/integration">Campaign connection to other solutions documentation</a><br/>
        Integration with:<br/>
        - <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aa">Adobe Analytics</a><br/>
        - <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-triggers">Adobe Experience Cloud triggers</a><br/>
        - <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aem">Adobe Experience Manager</a><br/>
        - <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aep/ac-aep">Adobe Experience Platform</a><br/>
        - <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-ajo">Adobe Journey Optimizer</a><br/>
        - <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-at">Adobe Target</a><br/>
        - <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-workfront">Adobe Workfront</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Use transactional messages</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional">Transactional messages documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
  <tr style="border: 1;">
    <td>
        <div>Use reporting</div>
    </td>
    <td>
        <a href="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/analytics/reports/gs-reporting">Reporting configuration documentation</a><br/>
    </td>
    <td>
        <div></div>
    </td>
  </tr>
</table>

## Deprecated items

https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features 