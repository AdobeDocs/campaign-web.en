---
audience: end-user
title: Use a trap group
hide: yes
hidefromtoc: yes
description: Learn how to use a trap group for your delivery in Campaign Web user interface

---
# Use a **[!UICONTROL trap group]** {#trap-group}

A **[!UICONTROL trap group]** is used to target recipients who do not match the defined target criteria. This way, recipients who are out of the delivery scope can receive the delivery, as any other target recipient would.
A **[!UICONTROL trap group]** is a group of **[!UICONTROL seed addresses]**.

## Why use **[!UICONTROL trap group]**

You can use **[!UICONTROL trap group]** : 

1. **As a proof** : each member of the **[!UICONTROL Trap group]** will receive the delivery as if they were part of the audience.


1. **To protect your mailing list** : by receiving what the audience will receive, each **[!UICONTROL seed address]** of the **[!UICONTROL Trap group]** will be noticed if the mailing list is used by a third party.

## About **[!UICONTROL Trap group]**

Seed addresses are automatically excluded from reports on the following delivery statistics: **Clicks**, **Opens**, **Unsubscriptions**. The reports are only about the real audience.

For an email delivery, only email address is needed for the **[!UICONTROL Trap group]**, the personalization of other fields will be filled randomly by Campaign.

## How to setup a **[!UICONTROL Trap group]** in the delivery

To setup a **[!UICONTROL Trap group]**, go to the **[!UICONTROL Audience]** settings of your delivery. You will have 2 options :
- [Select test profiles](#select-test-profile)
- [Create condition](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Select test profiles {#select-test-profiles}

When you choose "Select test profiles", you will have the window as below where you are invited to **[!UICONTROL Add test profile(s)]** :

![](assets/trap-no-test-profile.png){zoomable="yes"}

When you click on the button, you will have access to the seed addresses you can add your **[!UICONTROL trap group]**. Check the ones you want to use.
You can create new seed addresses. [Learn more](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

When you confirm your trap addresses, check that you have the correct number under **[!UICONTROL Trap group]**.

![](assets/trap-check.png){zoomable="yes"}

### Create condition {#create-condition}

With the **[!UICONTROL Create condition]** choice, you will get a new window where you can custom a query to define the seed addresses you want to use :

![](assets/trap-create-condition.png){zoomable="yes"}

Your query will be displayed under **[!UICONTROL Trap group]**.

![](assets/trap-custom.png){zoomable="yes"}

## How to create a new **[!UICONTROL seed address]** {#create-seed}

You can create a new **[!UICONTROL seed address]** in **[!UICONTROL Explorer]** > **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed members]**

![](assets/trap-create.png){zoomable="yes"}

You can complete all the details about your seed member as if it was an audience profile :

![](assets/trap-create-contact.png){zoomable="yes"}