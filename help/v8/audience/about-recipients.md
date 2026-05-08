---
title: Get started with profiles
description: Learn how to monitor and manage profiles in Campaign Web.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
---
# Get started with profiles {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profiles"
>abstract="A profile is a record targeted to receive messages sent by Adobe Campaign. From this list, you can view the profiles' details, based on your permissions. Use the filtering options to browse this list. You can edit and update a small set of your profiles' attributes."

## What is a profile? {#what} 

A **profile**, also known as a "recipient" in the client console, represents a record stored in the Campaign database. It serves as a key component to [create audiences](create-audience.md) for deliveries and [add personalization](../personalization/personalize.md) data to your content. Adobe Campaign enables seamless management of profiles, including creating new entries and accessing a comprehensive view of all profiles' attributes and service subscriptions, through the Campaign Web user interface.

Additionally, **[!UICONTROL test profiles]**, identified as "seed profiles" in the client console, allow targeting of additional recipients who do not match the targeting criteria of a given delivery. These profiles contain fictitious contact information or contact information controlled by the sender. Test profiles are proof recipients used to test messages by sending proofs. [Learn how to work with test profiles](test-profiles.md)

Both profiles and test profiles are useful for testing deliveries before they reach the intended audience. This allows previewing of message content and personalization, sending proofs for testing and validation, evaluating email rendering across various platforms and devices, and testing landing pages. [Learn how to preview and test deliveries](../preview-test/preview-test.md)

➡️ [Discover this feature in video](#video) 

## Access the list of profiles {#access}

Profiles are accessible and editable in Adobe Campaign Web from the **[!UICONTROL Customer management]** > **Profiles** entry in the left navigation rail. They can also be accessed in the **[!UICONTROL Explorer]** view, from the **[!UICONTROL Profiles & Targets]** > **[!UICONTROL Recipients]** node. From there, browse, create, and manage folders or subfolders, as well as check associated permissions. [Learn how to create folders](../get-started/permissions.md#folders).

>[!NOTE]
>
>Depending on your permissions, you might not have access to the full list of profiles stored in the database. [Learn more about permissions](../get-started/permissions.md)

Filter the **[!UICONTROL Profiles]** list using the search field or filters available from the **Show filters** button. Restrict the results to a specific [folder](../get-started/permissions.md#folders) using the drop-down list, or add rules using the [query modeler](../query/query-modeler-overview.md).

![Filters available in the profiles list](assets/profiles-list-filters.png){zoomable="yes"}

To access the details of a profile, click on its name from the list. A detailed view of the profile opens, allowing exploration of its attributes and the services the profile subscribed to. [Learn how to explore profiles' details](create-profile.md)

To delete a profile, select the corresponding option from the **[!UICONTROL More actions]** menu.

## How-to video {#video}

Learn how to access, manage, and explore profiles using the Campaign Web user interface.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)