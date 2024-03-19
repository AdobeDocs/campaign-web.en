---
title: Get started with profiles
description: Learn how to monitor and manage profiles in Campaign Web.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
---
# Get started with profiles {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profiles"
>abstract="A profile is a record who is targeted to receive messages sent by Adobe Campaign. From this list, you can view the profiles' details, based on your permissions. Use the filtering options to browse this list. You can edit and update a small set of your profiles' attributes."

## What is a profile? {#what} 

A **profile**, also known as a "recipient" in the client console, represents a record stored in the Campaign database, serving as a key component to [create audiences](create-audience.md) for deliveries and [add personalization](../personalization/personalize.md) data to your content. Adobe Campaign allows you to seamlessly manage profiles, from creating new entries to accessing a comprehensive view of all your profiles' attributes and services subscriptions, all through the Campaign Web user interface.

Moreover, **[!UICONTROL test profiles]**, identified as "seed profiles" in the client console, allow you to target additional recipients who do not match the targeting criteria of a given delivery. These profiles contain fictitious contact information, or contact information controlled by the sender. Test profiles are proof recipients: they are used to test your messages by sending proofs. [Learn how to work with test profiles](test-profiles.md)

Both profiles and test profiles can be used to test your deliveries before they reach the intended audience. By doing so, you can preview the message content and personalization, send proofs for testing and validation, evaluate email rendering across various platform and devices, and test your landing pages. [Learn how to preview and test deliveries](../preview-test/preview-test.md)

➡️ [Discover this feature in video](#video) 

## Access the list of profiles {#access}

Profiles are accessible and editable in Adobe Campaign Web from the **[!UICONTROL Customer management]** > **Profiles** entry in the left navigation rail. You can also access them in the **[!UICONTROL Explorer]** view, from the **[!UICONTROL Profiles & Targets]** > **[!UICONTROL Recipients]** node. From there you can browse, create and manage folders or subfolders, as well as check associated permissions. [Learn how to create folders](../get-started/permissions.md#folders)

>[!NOTE]
>
>Depending on your permissions, you might not have access to the full list of profiles stored in the database. [Learn more about permissions](../get-started/permissions.md).

You can filter the **[!UICONTROL Profiles]** list using the search field or filters available from the **Show filters** button. You can restrict the results to a specific [folder](../get-started/permissions.md#folders) using the drop-down list, or add rules using the [query modeler](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png){zoomable="yes"}

To access the details of a profiles, click on its name from the list. A detailed view of the profile opens, allowing you to explore its attributes and the services he subscribed to. [Learn how to explore profiles' details](create-profile.md)

To delete a profile, select the corresponding option from the **[!UICONTROL More actions]** menu.

## How-to video {#video}

Learn how to access, manage, and explore profiles using the Campaign Web user interface.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)
