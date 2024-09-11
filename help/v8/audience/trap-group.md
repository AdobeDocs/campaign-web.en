---
audience: end-user
title: Use a trap group
description: Learn how to use a trap group for your delivery in Campaign Web user interface
exl-id: 48c34581-8825-4798-b24e-c462303f7645
---
# Use a trap group {#trap-group}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Trap group"
>abstract="You can use a trap group to include specific addresses in your deliveries to monitor and verify the distribution process by targeting profiles who do not match the defined target criteria."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"

A **[!UICONTROL trap group]** (also known as **[!UICONTROL Seed list]**) is used to include specific addresses in your deliveries to monitor and verify the distribution process by targeting profiles who do not match the defined target criteria. This way, recipients who are out of the delivery scope can receive the delivery, as any other target recipient would.

A **[!UICONTROL trap group]** is a group of **[!UICONTROL seed addresses]**, named **[!UICONTROL Test profile]** on Campaign web user interface.

## Why use a trap group {#why-trap-group}

You can use **[!UICONTROL trap group]**:

1. **As a proof**: each member of the **[!UICONTROL Trap group]** will receive the delivery as if they were part of the audience.

1. **To protect your mailing list**: by receiving what the audience will receive, each **[!UICONTROL test profile]** of the **[!UICONTROL Trap group]** will be noticed if the mailing list is used by a third party.

>[!NOTE]
>
>In addition to [sending proofs during the creation of the delivery](../email/create-email.md#preview-test) and from [control group](control-group.md), adding a trap group is a good way to test your audience.

## About trap groups {#about-trap-group}

Test profiles are automatically excluded from reports on the following delivery statistics: **Clicks**, **Opens**, **Unsubscriptions**. The reports are only about the real audience.

For an email delivery, only email address is needed for the **[!UICONTROL Trap group]**, the personalization of other fields will be filled randomly by Campaign.

## Add a Trap group in a delivery {#trap-group-in-delivery}

To setup a **[!UICONTROL Trap group]**, go to the **[!UICONTROL Audience]** settings of your delivery. You will have 2 options :

* [Select test profiles](#select-test-profile)
* [Create condition](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Select test profiles {#select-test-profiles}

When you choose **Select test profiles**, you can use the **Add test profile(s)** button as shown below:

![](assets/trap-no-test-profile.png){zoomable="yes"}

When you click on the button, you have access to the test profiles you can add your **[!UICONTROL trap group]**. Select the ones you want to use.

You can also create new test profiles. [Learn more](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

When you confirm your test profiles, check that you have the correct number under **[!UICONTROL Trap group]**.

![](assets/trap-check.png){zoomable="yes"}

### Create condition {#create-condition}

With the **[!UICONTROL Create condition]** option, you can create a query to define the test profiles you want to use:

![](assets/trap-create-condition.png){zoomable="yes"}

Your query is displayed under **[!UICONTROL Trap group]**.

![](assets/trap-custom.png){zoomable="yes"}

## Create a new test profile {#create-seed}

You can create a new **[!UICONTROL test profile]** from the  **[!UICONTROL Explorer]** > **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed members]** folder.

![](assets/trap-create.png){zoomable="yes"}

Configure all settings about your **[!UICONTROL test profile]** as for any profile:

![](assets/trap-create-contact.png){zoomable="yes"}
