---
title: Targeting dimensions
description: Learn more about targeting dimensions in Adobe Campaign Web
badge: label="Limited Availability"
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
---
# Targeting dimensions {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Select the targeting dimension"
>abstract="The targeting dimension lets you define the population targeted by the operation: recipients, contract beneficiaries, operator, subscribers, etc. By default, the target is selected from the recipients."

The targeting dimension, aka. target mapping, is the type of data that an operation is handling. It lets you define the targeted population: profiles, contract beneficiaries, operators, subscribers, etc.

## Workflows' targeting dimensions {#workflow}

The targeting dimension of a workflow is defined by the first **[!UICONTROL Build audience]** activity and is used across all further activities until the end of the workflow. For example, if you perform a query on the profiles from the database, the outbound transition will contain data of type 'recipient' and it will be transmitted to the next activity.

Note that you can switch the targeting dimension in a workflow using a [Change dimension activity](../workflows/activities/change-dimension.md). This allows you, for example, to query the database on a specific table such as purchases or subscriptions, and then change the targeting dimension to Recipients in order send deliveries to the corresponding profiles.

When selecting a targeting dimension (in the workflow settings, or in activites such as **Build audience**, **Reconciliation** or **Change dimension**), a selection of commonly used schemas is displayed by default in the list. To show all available schemas, toggle on the **[!UICONTROL Show all schemas]** button. The option selection is saved for each user.

![](assets/targeting-dimension-show-all.png)

## Targeting dimensions {#list}

By default, email and SMS delivery templates target profiles. Their target dimension therefore uses the fields of the **nms:recipient** table. For Push notifications, the default target dimension is **Subscriber applications nms:appSubscriptionRcp**, which is linked to the recipients table. 

You can also use other built-in target mappings in your workflows and deliveries that are listed below: 

|  Name  | Use to | Schema  |
|---|---|---|
|  Recipients  | Deliver to recipients (built-in recipient table)  | nms:recipient  |
|  Visitors  | Deliver to visitors whose profiles have been collected via referral (viral marketing) for ex.  | mns:visitor  |
|  Subscriptions  | Deliver to recipients who are subscribed to an information service such as a newsletter | nms:subscription  |
|  Visitor subscriptions  | Deliver to visitors who are subscribed to an information service  | nms:visitorSub  |
|  Operators  | Deliver to Adobe Campaign operators  | nms:operator  |
|  External file  | Deliver via a file that contains all information needed for delivery  | No linked schema, no target entered  |
|  Subscriber applications  | Deliver to recipients who are subscribed to an application | nms:appSubscriptionRcp  |

In addition, you can create a new target mapping depending on your needs. This is performed from the client console. Learn more in [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
