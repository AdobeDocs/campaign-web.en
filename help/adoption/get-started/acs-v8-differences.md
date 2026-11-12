---
title: Differences between Campaign Standard and Campaign v8
description: Learn what changes when you transition from Campaign Standard to Campaign v8, and where to find the details
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
---
# Differences between Campaign Standard and Campaign v8 {#acs-v8-differences}

Most concepts are the same in Campaign Standard and Campaign v8. This page gathers the differences that affect you after the transition, and links to the page that explains each one. It complements the guides for [marketers](marketers.md) and for [administrators and developers](admin-developers.md).

* For the terminology changes, see [Key differences between Campaign Standard and Campaign v8](overview.md#experiences).
* For the checks to run and the issues reported after a transition, see [Checks and troubleshooting after the transition](post-transition-checks.md).
* For the capabilities that are available only in the client console, see [Campaign Web and Campaign client console](../../v8/get-started/capability-matrix.md).

## Channels and content {#channels}

The steps to create and send messages are similar in both products, as described in the [guide for marketers](marketers.md). The differences below concern channel availability, test deliveries, landing pages and direct mail workflows.

| What changes | Learn more |
|---|---|
| The In-App channel is not available in Campaign v8. | [In-App channel](marketers.md#acs-gs-marketers-in-app) |
| To transition existing push workflows and deliveries, contact your Adobe Campaign Transition Manager. | [Push notifications](marketers.md#acs-gs-marketers-push) |
| In Campaign Standard, a test profile could be marked as a **Trap** to receive the final send. In Campaign v8, add a **Trap group** in the Audience settings of the delivery. | [Trap group](../../v8/audience/trap-group.md) |
| Landing pages created in the Campaign Web user interface do not support hidden input fields or custom JavaScript. | [Landing pages](../../v8/landing-pages/get-started-lp.md) |
| In Campaign Standard, the outbound transition of a direct mail activity also carried the generated file. In Campaign v8, it carries only the targeted population. To send the file to a server, add a **Data extraction** activity, then a **File transfer** activity. | [Direct mail](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## Audiences, workflows and deliveries {#data-and-workflows}

These differences affect the audiences and workflows migrated from Campaign Standard, some options of recurring deliveries and of the **File transfer** activity, and the scope of dynamic reporting.

| What changes | Learn more |
|---|---|
| Audiences are transformed during the transition. For example, audiences created with the Query activity become predefined filters, and file-type audiences become List-type audiences without dimensions. | [Manage audiences](marketers.md#acs-gs-marketers-audiences) |
| Historical logs of workflows executed in Campaign Standard are not migrated. | [Create a workflow](marketers.md#acs-gs-marketers-wf) |
| In Campaign Standard, you could select the aggregation period of a recurring email. This option is not available in Campaign v8. | [Channel activities](../../v8/workflows/activities/channels.md) |
| Dynamic reporting covers email deliveries, campaigns with email deliveries, and transactional messages. | [Reporting](marketers.md#acs-gs-marketers-reporting) |

## Access and security {#access}

Campaign Standard security groups, roles and organizational units are mapped to operator groups, named rights and folder permissions during the transition. Review the points below, in particular if some users have broader or narrower rights than before.

| What changes | Learn more |
|---|---|
| Security groups, roles and organizational units are mapped to operator groups, named rights and folder permissions. Custom roles are not migrated. | [User access management](user-management-acs.md) |
| Users with the **Data Model** role but not the **Administration** role gain **Administration** access. | [User access management](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| Users assigned to security groups with parallel organizational units can have broader access in Campaign v8. | [Parallel organizational unit assignment](user-management-acs.md#parallel-assignments) |
| Accessing transactional APIs from the execution instance requires a new product profile. | [Product profile mapping](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Privacy requests can arrive in both Campaign Standard and Campaign v8 during the period when your Campaign Standard environment remains active. | [Privacy and consent](admin-developers.md#privacy-and-consent) |

## APIs and integrations {#apis-and-integrations}

These differences affect the integrations that call Campaign through its REST API, and the integrations with other Adobe solutions and tools.

| What changes | Learn more |
|---|---|
| PKEY values change after the migration. If you store PKEYs outside Campaign, follow the hrefs returned by the API instead. | [REST APIs](admin-developers.md#acs-gs-admin-apis) |
| Some migrated profile fields, such as time zone and `ccpaOptOut`, are returned only by the `profileAndServicesExt/profile` API. | [REST APIs](admin-developers.md#acs-gs-admin-apis) |
| Adobe migrates your Adobe Analytics and Audience Manager configurations. You must set up the Triggers and Adobe Target integrations again. | [Manage Adobe Campaign integrations](admin-developers.md#acs-gs-integrations) |
