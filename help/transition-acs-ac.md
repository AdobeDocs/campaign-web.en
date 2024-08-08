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

Adobe Campaign v8 can send rich push notifications.  

![](v8/push/assets/rich_push.png){zoomable="yes"}

You can define your content using the given templates. According to your customer system, you can design your push accordingly :

* For [Android](v8/push/rich-push.md) users

* For [iOs](v8/push/rich-push.md)

Push notifications are essential for reaching out to your mobile app users, even when they're not actively using your app.

* **Adobe Experience Manager as a Cloud Services**

Adobe Campaign v8 is natively integrated with Adobe Experience Manager as a Cloud Services. It helps you provide your customers with personalized, content-led experiences. 

This feature is available for :
* *Asset management*: The left pane of the email designer gives you a way to find easily assets and customize it. 
[Learn more here](v8/campaign-web-home.md)
![](v8/integrations/assets/assets_6.png){zoomable="yes"}

- *Email template import* : You can browse through AEM templates and select one to import to Campaign. 
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

Most concepts are similar between Adobe Campaign v8 and Adobe Campaign Standard. However, there are a few differences as described below. 

### The terminology

Here are some terminology differences between Campaign Standard and the Campaign v8:

<table style="table-layout:fixed">
  <tr style="border: 1;">
    <td align="center"><strong>Adobe Campaign Standard</strong></td>
    <td align="center"><strong>Adobe Campaign v8</strong></td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Program</td>
    <td align="center">Campaign</td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Real-time events and Transactional events</td>
    <td align="center">Triggers</td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Tracking</td>
    <td align="center">Reporting</td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Profiles</td>
    <td align="center">Recipients (in certain circumstances)</td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Traps</td>
    <td align="center">Seeds</td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Custom resources</td>
    <td align="center">Schemas</td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Messages</td>
    <td align="center">Deliveries</td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Product users</td>
    <td align="center">Operators</td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Roles</td>
    <td align="center">Named Rights</td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Security Groups</td>
    <td align="center">Operator Groups</td>
  </tr>
  <tr style="border: 1;">
    <td align="center">Organizational Units</td>
    <td align="center">Folder Permissions</td>
  </tr>
</table>

### Marketing experiences

[Marketer documentations table](transition-acs-ac-marketer.md)

* **The User Interface**

All the data from Adobe Campaign Standard is imported in Adobe Campaign v8. 

You can use your credentials, and connect to your instance. 
You can find your profiles and your workflows. 

The real difference is in the user interface. You can find here the change here :

![](assets/transition_workflow.png){zoomable="yes"}

[Learn more about the Web User Interface of Adobe Campaign v8](v8/get-started/user-interface.md).

### Administrator experiences

[Administrator documentations table](transition-acs-ac-admin.md)

* **The client console**

The big difference for administrators is the use of the client console. It is a native application which communicates with the Adobe Campaign application server. Campaign client console centralizes all capabilities and settings. It is synchronized with the Campaign Web User Interface.

![](assets/client_console.png){zoomable="yes"}

[Learn more about the client console user interface of Adobe Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access).

## Migration video

Video to upload on https://publish.tv.adobe.com/buckets

To check

https://adobe-my.sharepoint.com/personal/ssahai_adobe_com/_layouts/15/stream.aspx?id=%2Fpersonal%2Fssahai%5Fadobe%5Fcom%2FDocuments%2FDocuments%2FFeatures%2FEuropa%20%2D%20ACS%20to%20ACC%2FDemos%2FEuropa%2EDemo%2EApril%2Emov&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Ef947ff92%2Ddbc6%2D4de2%2D99be%2Db8027acba5db&OR=Teams%2DHL&CT=1722944686104&clickparams=eyJBcHBOYW1lIjoiVGVhbXMtRGVza3RvcCIsIkFwcFZlcnNpb24iOiI1MC8yNDA2MjcyNDgxNyIsIkhhc0ZlZGVyYXRlZFVzZXIiOmZhbHNlfQ%3D%3D


## Deprecated items

https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features 