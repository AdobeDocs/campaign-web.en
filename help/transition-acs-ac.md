---
title: Transition from Adobe Campaign Stand to Adobe Campaign v8
description: Learn how to transition smoothly to Adobe Campaign v8
---

# Transition from Adobe Campaign Standard to Adobe Campaign v8

## Introduction

This guide is designed for Adobe Campaign Standard customers transitioning to Adobe Campaign v8. Adobe Campaign v8 introduces major improvements in infrastructure and performance, tailored for enterprises that require scalable and efficient campaign management solutions.

With Adobe Campign v8, users benefit from enhanced support for managing cross-channel campaigns thanks to powerful features adapted to marketing 
usage. This version integrates smoothly with other Adobe solutions, including Adobe Experience Platform, enabling users to leverage a unified ecosystem for their marketing goals.

In this guide, you can find information on the features and capabilities of Adobe Campaign v8, along with documentation tables, to ensure a successful transition from Adobe Campaign Standard.

## What's new?

Get a glimpse of what you get with Adobe Campaign v8!

### Enhancement with Adobe Campaign v8

* **Web User Interface**

Adobe Campaign v8 offers both a client console and a web user interface, catering to different user preferences and needs. The client console provides a powerful desktop application experience, while the web user interface is designed to be intuitive and accessible, making it an ideal choice for marketers familiar with Adobe Campaign Standard. 

The web user interface shares many similarities with Adobe Campaign Standard, although some terminologies may differ. 

You can [learn more about Adobe Campaign Web User Interface here](v8/campaign-web-home.md).

![](assets/home.png){zoomable="yes"}


* **Performance**

Adobe Campaign v8 takes advantage of advanced cloud-scale database technologies, resulting in significantly improved performance and efficiency. It introduces the concept of Full Federated Data Access (FFDA), where all data is now securely stored on the Cloud Database.

This redesigned architecture offers several key benefits :

* *Increased Storage*: Adobe Campaign v8 provides up to **6TB** in total database storage across production and staging instances, accomodating the needs of large-scale enterprises and complex campaign strategies
* *Enhanced Speed and Scale* : The system now supports a substantial increase in processing capabilities, with batch processing throughput reaching up to **15 million operations per hour** and transactional throughput of up to **180.000 operations per hour**.
* *Snowflake via FDA* : Integration with Snowflake through Federated Data Access enables the offloading of high-volume data, optimizing performance and resource utilization. This results, with increased storage capacity, in faster segmentations, queries, reports and deliveries, allowing timely execution of marketing strategies.

Overall, Adobe Campaign v8's robust architecture provides a powerful foundation for managing extensive and complex marketing campaigns with enhanced speed, storage, and efficiency.

### New features on Adobe Campaign v8

* **Rich push**

Adobe Campaign v8 offers the capability to send rich push notifications, which can capture users' attention and encourage them to take action. These notifications can include a variety of elements such as text, images, buttons, countdown timers, sounds, etc.

![](v8/push/assets/rich_push.png){zoomable="yes"}

To facilitate the creation of these rich notifications, Adobe Campaign v8 provides various templates that enable you to design and customize the content of complex notifications, such as carousels or timers.

You can tailor your notifications based on the customer's system :

* For [Android](v8/push/rich-push.md) users

* For [iOs](v8/push/rich-push.md) users

Push notifications are a crucial tool for engaging mobile app users, allowing you to reach them even when they are not actively using your app.

* **Adobe Experience Manager as a Cloud Service**

Adobe Campaign v8 is seamlessly integrated with Adobe Experience Manager as a Cloud Service, enhancing your ability to deliver personalized and content-rich experiences to your customers. This native integration streamlines content management and leverages Adobe Experience Manager's robust capabilities to optimize your marketing efforts.

Here are the key feature enabled by this integration: 

* *Asset management*: Within Adobe Campaign v8, the email designer provides a picker to access and manage assets. This feature simplifies the integration of elements from Adobe Experience Manager into your delivery, making content management more efficient. 
[Learn more about Asset management](v8/integrations/aem-assets.md)
![](v8/integrations/assets/assets_6.png){zoomable="yes"}

* *Email template import* : Adobe Campaign v8 enables you to browse and import email templates from Adobe Experience Manager directly into Campaign.  
[Learn more about Email template import](v8/integrations/aem-content.md)
![](v8/integrations/assets/aem_6.png){zoomable="yes"}

Adobe Experience Manager as a Cloud Service offers cloud-native agility, allowing you to accelerate your time to value and adapt to evolving business needs. This integration not only enhances your content management capabilities but also enables you to delivery more personalized and engaging experiences to your customers across all touchpoints.

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

The managed services approach enables marketers to take advantage of the operational scale and economics of cloud infrastructure without the need for heavy support from internal IT resources. 

Adobe consulting and implementation teams work with you to assess your marketing plans, existing practices, data requirements, and messaging volume, and then they recommend the most appropriate service, support, and deliverability packages. The Adobe Campaign Managed Cloud Services team can then monitor and report on campaign performance, brand reputation, customer experience metrics, and more.

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

### Marketer experiences

* **The User Interface**

All of your data from Adobe Campaign Standard is imported in Adobe Campaign v8, ensuring a smooth transition with minimal disruption to your ongoing operations. 

You can continue to use your existing credentials to log in and connect to your new Adobe Campaign v8 instance. Once logged in, you can find all your profiles and workflows being migrated, allowing you to continue to work on your campaigns. 

The primary difference is in the user interface. Below a comparison of the same workflow in the 2 interfaces :

![](assets/transition_workflow.png){zoomable="yes"}

[Learn more about the Web User Interface of Adobe Campaign v8](v8/get-started/user-interface.md).

For guidance on using Adobe Campaign v8 as a marketer, please refer to the [Marketer documentations table](transition-acs-ac-marketer.md).

### Administrator experiences

* **The client console**

The major change for administrators is the introduction of the client console, the native application which communicates with the Adobe Campaign application server. 

The Campaign client console centralizes all capabilities and settings. It is stays synchronized with the Campaign Web User Interface, ensuring consitency acrouss both environments.

![](assets/client_console.png){zoomable="yes"}

[Learn more about the client console user interface of Adobe Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access).

For guidance on using Adobe Campaign v8 as an administrator, please refer to the [Administrator documentations table](transition-acs-ac-admin.md).

## Migration video

Video to upload on https://publish.tv.adobe.com/buckets

To check

https://adobe-my.sharepoint.com/personal/ssahai_adobe_com/_layouts/15/stream.aspx?id=%2Fpersonal%2Fssahai%5Fadobe%5Fcom%2FDocuments%2FDocuments%2FFeatures%2FEuropa%20%2D%20ACS%20to%20ACC%2FDemos%2FEuropa%2EDemo%2EApril%2Emov&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Ef947ff92%2Ddbc6%2D4de2%2D99be%2Db8027acba5db&OR=Teams%2DHL&CT=1722944686104&clickparams=eyJBcHBOYW1lIjoiVGVhbXMtRGVza3RvcCIsIkFwcFZlcnNpb24iOiI1MC8yNDA2MjcyNDgxNyIsIkhhc0ZlZGVyYXRlZFVzZXIiOmZhbHNlfQ%3D%3D


## Deprecated items

Adobe constantly evaluates product capabilities to identify older features that should be replaced with more modern alternatives to improve overall customer value, always under careful consideration of backward compatibility.

Please refer to [this documentation for information on deprecated items](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features).