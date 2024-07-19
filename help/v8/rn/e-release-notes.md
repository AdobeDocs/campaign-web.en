---
title: Campaign v8 Web User Interface Early Release Notes
description: Discover new features coming with the next Campaign Web User Interface release
hide: yes
hidefromtoc: yes
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
---
# Early release notes {#e-release}

Adobe Campaign Web User interface continuously delivers new features, enhancements to existing features, and bug fixes. All changes are consolidated at the end of each month in the [release notes](release-notes.md). 

**Early release notes below are subject to change without prior notice until the release availability date**. Links, screens and updated documentation are published in the [release notes](release-notes.md), at the release date.

## July release notes {#24-7-release}

**Release date**: July 30-31, 2024

The following features and improvements are available starting July release.

### Seed lists {#24-7-2}

A seed list, aka. **Trap group**, is a list of seed addresses. It is used to include specific addresses in your deliveries, and then target profiles who do not match the defined target criteria. This way, recipients who are out of the delivery audience can receive the delivery, as any other target recipient would. You can use seed addresses when sending proofs, or to protect your mailing list.

### Rich push notification templates {#24-7.3}

You can now send rich push notifications. A rich push notification is an enhanced form of mobile notification that goes beyond simple text messages by incorporating multimedia elements such as images, interactive buttons, or other rich media content. With this version, a set of templates for rich push notifications are now available for your iOS and Android apps. 

>[!AVAILABILITY]
>
>This capability requires an update to Campaign v8.6.3 or v8.7.2. [Learn more in Campaign Client console release notes](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/release-notes)


### Improvements {#improvements-24-7}

**Folders management** - You can now manage permissions and restrictions on folders.

### New features in Limited Availability {#acs-24-4}

>[!AVAILABILITY]
>
>The following capabilities are in Limited Availability (LA). They are restricted to customers migrating **from Adobe Campaign Standard to Adobe Campaign v8**, and cannot be deployed on any other environment.
>
>Refer to the following documentation pages: [Campaign Standard transition to Campaign v8](../rn/acs-migration.md) and [Features for Campaign Standard users](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

#### Content Fragments {#LA-24-7}

You can now create and use content fragments. A content fragment is a reusable component that can be referenced in one or more messages. When modifying a fragment, every content using it is updated. This functionality allows to prebuild multiple custom content blocks that can be used by marketing users to quickly assemble message contents in an improved design process.

Two types of fragments are available:

* **Expression fragments** are pre-defined expressions that are available from a dedicated entry in the expression editor.
* **Visual fragments** are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](../email/fragments.md)

    >[!AVAILABILITY]
    >
    >**Visual fragments** are in Limited Availability (LA). This capability is restricted to customers migrating **from Adobe Campaign Standard to Adobe Campaign v8**, and cannot be deployed on any other environment.
