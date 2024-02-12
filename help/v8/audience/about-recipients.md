---
title: Get started with profiles
description: Learn how to monitor and manage profiles in Campaign Web.

---
# Get started with profiles {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="360 view of your profiles"
>abstract="Create new profiles, and monitor them through powerful reports and tools. Access your profiles' attributes, interactions and logs. Use the filtering options to browse the profiles list, edit and update their profile."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="See release notes"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360 view of your profiles"
>abstract="Create new profiles, and monitor them through powerful reports and tools. Access your profiles' attributes, interactions and logs. Use the filtering options to browse the profiles list, edit and update their profile."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="See release notes"
<!--TO REMOVE ABOVE-->

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profiles"
>abstract="A profile is an individual who is targeted to receive messages sent by Adobe Campaign. From this list, you can view the profiles' details, based on your permissions. Use the filtering options to browse this list. You can edit and update a small set of your profiles' attributes."

## What is a profile? {#what} 

A **profile**, also known as "recipients" in the client console, represents an individual stored in the Campaign database, serving as a key component to [create audiences](create-audience.md) for deliveries and [add personalization](../personalization/personalize.md) data to your content. Adobe Campaign allows you to seamlessly manage profiles, from creating new entries to accessing a comprehensive view of all your profiles' attributes and services subscriptions, all through the Campaign Web user interface.

Moreover, **[!UICONTROL test profiles]**, identified as "seed profiles" in the client console, allow you to target additional recipients who do not match the targeting criteria of a given delivery. These profiles contain fictitious contact information, or contact information controlled by the sender. They can be added to a message’s audience to detect any fraudulent use of your recipient database or to ensure that the emails arrive in the inboxes. [Learn how to work with test profiles](test-profiles.md)

Both profiles and test profiles can be used to test your deliveries before they reach the intended audience. By doing so, you can preview the message content and personalization, send proofs for testing and validation, evaluate email rendering across various platform and devices, and test your landing pages. [Learn how to preview and test deliveries](../preview-test/preview-test.md)

## Access the list of profiles {#access}

Profiles are accessible and editable in Adobe Campaign Web from the **[!UICONTROL Customer management]** > **Profiles** entry in the left navigation rail. You can also access them in the **[!UICONTROL Explorer]** view, from the **[!UICONTROL Profiles & Targets]** > **[!UICONTROL Recipients]** node. From there you can browse, create and manage folders or subfolders, as well as check associated permissions. [Learn how to create folders](../get-started/permissions.md#folders)

>[!NOTE]
>
>Depending on your permissions, you might not have access to the full list of profiles stored in the database. [Learn more about permissions](../get-started/permissions.md).

You can filter the **[!UICONTROL Profiles]** list using the search field or filters available from the **Show filters** button. You can restrict the results to a specific [folder](../get-started/permissions.md#folders) using the drop-down list, or add rules using the [query modeler](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png){zoomable="yes"}

To access the details of a profiles, click on its name from the list. A detailed view of the profile opens, allowing you to explore its attributes and the services he subscribed to. [Learn how to explore profiles' details](create-profile.md)

To delete a profile, select the corresponding option from the **[!UICONTROL More actions]** menu.
