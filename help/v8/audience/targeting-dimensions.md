---
title: Targeting dimensions
description: Learn more about targeting dimensions in Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
---
# Targeting dimensions {#targeting-dimensions}

>[!CONTEXTUALHELP]  
>id="acw_orchestration_build_audience_dimension"  
>title="Select the targeting dimension"  
>abstract="The targeting dimension lets you define the population targeted by the operation: recipients, contract beneficiaries, operator, subscribers, and more. By default, for emails and SMS, the target is selected from the Recipients built-in table. For Push notifications, the default target dimension is Subscriber applications."

The targeting dimension, also known as target mapping, is the type of data that an operation handles. It defines the targeted population, such as profiles, contract beneficiaries, operators, and subscribers.

## Workflows' targeting dimensions {#workflow}

The targeting dimension of a workflow is defined by the first **[!UICONTROL Build audience]** activity and is used across all subsequent activities until the end of the workflow. For example, when querying profiles from the database, the outbound transition contains data of type 'recipient,' which is transmitted to the next activity.

Switch the targeting dimension in a workflow using a [Change dimension activity](../workflows/activities/change-dimension.md). This allows querying the database on a specific table, such as purchases or subscriptions, and then changing the targeting dimension to Recipients to send deliveries to the corresponding profiles.

When selecting a targeting dimension (in the workflow settings or in activities such as **Build audience**, **Reconciliation**, or **Change dimension**), a list of commonly used schemas is displayed by default. To show all available schemas, toggle the **[!UICONTROL Show all schemas]** button. The option selection is saved for each user.

![Screenshot showing the targeting dimension interface with the "Show all schemas" button enabled.](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Targeting dimensions {#list}

By default, email and SMS delivery templates target profiles. Their target dimension uses the fields of the **nms:recipient** table. For Push notifications, the default target dimension is **Subscriber applications nms:appSubscriptionRcp**, which is linked to the recipients table.

Use other built-in target mappings in workflows and deliveries, as listed below:

| Name                  | Use to deliver to                                      | Schema                  |
|-----------------------|-------------------------------------------------------|-------------------------|
| Recipients            | Profiles / recipients (built-in recipient table)      | nms:recipient           |
| Visitors              | Visitors whose profiles were collected via referral   | mns:visitor             |
| Subscriptions         | Profiles subscribed to an information service         | nms:subscription        |
| Visitor subscriptions | Visitors subscribed to an information service         | nms:visitorSub          |
| Operators             | Adobe Campaign operators                              | nms:operator            |
| External file         | Delivery via a file containing all required information | No linked schema        |
| Subscriber applications | Profiles subscribed to an application               | nms:appSubscriptionRcp  |

Additionally, create new target mappings based on specific needs. Perform this operation from the client console only. Learn more in [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.