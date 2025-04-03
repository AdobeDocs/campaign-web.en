---
audience: end-user
title: Use a trap group
description: Learn how to use a trap group for your delivery in Campaign Web user interface
exl-id: 48c34581-8825-4798-b24e-c462303f7645
---
# Use a trap group {#trap-group}

A **[!UICONTROL trap group]** (also known as **[!UICONTROL Seed list]**) is used to include specific addresses in your deliveries to monitor and verify the distribution process by targeting profiles who do not match the defined target criteria. This way, recipients who are outside the delivery scope can receive the delivery, just like any other target recipient.

A **[!UICONTROL trap group]** is a group of **[!UICONTROL seed addresses]**, named **[!UICONTROL Test profile]** on the Campaign web user interface.

## Why use a trap group {#why-trap-group}

You can use a **[!UICONTROL trap group]**:

1. **As a proof**: Each member of the **[!UICONTROL trap group]** receives the delivery as if they were part of the audience.

1. **To protect your mailing list**: By receiving what the audience will receive, each **[!UICONTROL test profile]** of the **[!UICONTROL trap group]** will notice if the mailing list is used by a third party.

>[!NOTE]
>
>In addition to [sending proofs during the creation of the delivery](../email/create-email.md#preview-test) and from [control group](control-group.md), adding a trap group is a good way to test your audience.

## About trap groups {#about-trap-group}

Test profiles are automatically excluded from reports on the following delivery statistics: **Clicks**, **Opens**, **Unsubscriptions**. The reports focus only on the real audience.

For an email delivery, only the email address is required for the **[!UICONTROL trap group]**. The personalization of other fields is filled randomly by Campaign.

## Add a Trap group in a delivery {#trap-group-in-delivery}

To set up a **[!UICONTROL trap group]**, go to the **[!UICONTROL Audience]** settings of your delivery. You will have two options:

* [Select test profiles](#select-test-profiles)
* [Create condition](#create-condition)

[Trap group settings interface screenshot](assets/trap-group.png){zoomable="yes"}

### Select test profiles {#select-test-profiles}

When you choose **Select test profiles**, use the **Add test profile(s)** button as shown below:

[Add test profile button screenshot](assets/trap-no-test-profile.png){zoomable="yes"}

When you click the button, you can access the test profiles to add to your **[!UICONTROL trap group]**. Select the ones you want to use.

You can also create new test profiles. [Learn more](#create-seed)

[Select test profiles interface screenshot](assets/trap-select-test-profiles.png){zoomable="yes"}

After confirming your test profiles, check that the correct number appears under **[!UICONTROL trap group]**.

[Trap group confirmation screenshot](assets/trap-check.png){zoomable="yes"}

### Create condition {#create-condition}

With the **[!UICONTROL Create condition]** option, create a query to define the test profiles you want to use:

[Create condition interface screenshot](assets/trap-create-condition.png){zoomable="yes"}

Your query is displayed under **[!UICONTROL trap group]**.

[Trap group query display screenshot](assets/trap-custom.png){zoomable="yes"}

## Create a new test profile {#create-seed}

You can create a new **[!UICONTROL test profile]** from the **[!UICONTROL Explorer]** > **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed members]** folder.

[Create test profile navigation screenshot](assets/trap-create.png){zoomable="yes"}

Configure all settings for your **[!UICONTROL test profile]** as you would for any profile:

[Test profile configuration screenshot](assets/trap-create-contact.png){zoomable="yes"}