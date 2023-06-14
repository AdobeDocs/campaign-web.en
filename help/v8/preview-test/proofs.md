---
audience: end-user
title: Send test emails
description: Learn how to define and send test emails
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Alpha" 
---
# Send test emails {#send-test-emails}

**[!UICONTROL Adobe Campaign]** allows you to test a message before sending it to the main audience.

Sending test deliveries is an important step in validating your campaign and identifying potential issues.

The recipients of a test can check various elements such as links, opt-out links, images, or mirror pages, as well as detect any errors in the rendering, content, personalization settings and email configuration.

## Select the test recipients {#test-recipients}

### For emails and SMS deliveries

When working with emails or SMS deliveries, test messages can be sent to two types of recipients: 

* **Test profiles** - send test emails and SMS messages to seed addresses, which are additional and fictitious recipients in the database. They can be created in the [!DNL Campaign] console into the **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** folder. Learn more in [Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}
    
* **Substitute from main target** - send test emails and SMS messages to a specific email address or phone number while impersonating an existing profile. This allows you to experience the message as the recipients would, giving you an accurate representation of the content that the profile will receive.

To select the recipients of the test delivery, follow the steps below.

<!--Access the email [Edit content](../content/edit-content.md) screen or to the [Email Designer](../content/get-started-email-designer.md)-->

1. Browse to the edit content screen of your delivery, then click the **[!UICONTROL Simulate content]** button.

1. Click the **[!UICONTROL Test]** button.

    ![](assets/simulate-test-button-email.png)

1. Use the **[!UICONTROL Mode]** drop-down list to choose the type of recipients that receive the test email or SMS delivery:

    * **Test profiles** to target fictitious recipients
    
    * **Substitute from main target** to send a test to a specific email address while displaying data from an existing profile.

    ![](assets/simulate-profile-mode.png)

    >[!NOTE]
    >
    >By default, the **[!UICONTROL Use test profiles]** mode is selected. If you have already selected profiles to preview the email in the content simulation screen, those profiles are pre-selected as test recipients. You can clear your selection and/or add additional recipients.

1. To send test emails or SMS deliveries to substitution profiles, choose the **[!UICONTROL Substitute from target]** mode, then follow these steps:

    1. Click the **[!UICONTROL Add address]** button and specify the email address or phone number that receives the test delivery.

        You can enter any email address or phone number. This allows you to send test deliveries to any users, even if they are not users of [!DNL Adobe Campaign].

    1. Select the profile from the target to use as substitute. You can also let [!DNL Adobe Campaign] select a random profile from the target. The profile data from the selected profile will be displayed in the test delivery.

    1. Confirm the recipient and repeat the operation to add as many addresses or phone numbers as needed.

        ![](assets/simulate-profile-substitute.png)

1. Once the test recipients have been selected, you can [send the test delivery](#send-test).

    >[!NOTE]
    >
    >To also send the final email message to the recipients of the test email, select the **[!UICONTROL Include test population in the main target]** option.

### For push notifications {#push-notifications}

When working with push notifications, test messages can be sent to only one type of recipient: **Subscribers**, which are fictitious subscribers added to the database. Just as test profiles, they can be created in the [!DNL Campaign] console into the **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** folder. Learn more in [Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

To select the recipients of the test push notification, follow the steps below.

1. Browse to the edit content screen of your delivery, then click the **[!UICONTROL Simulate content]** button.

1. Click the **[!UICONTROL Test]** button.

    ![](assets/simulate-test-button-push.png)

1. If you have already selected subscribers to preview the email in the content simulation screen, those profiles are pre-selected as test subscribers. You can clear your selection and/or add additional subscribers.

    ![](assets/simulate-test-subscribers.png)

1. To also send the final push notification to the test subscribers, select the **[!UICONTROL Include test population in the main target]** option.

## Send the test delivery {#send-test}

To send the test delivery to the selected recipients, follow the steps below.

1. Click the **[!UICONTROL Send test]** button.

1. Confirm the sending.

    ![](assets/simulate-send-test.png)

1. Send as many tests as necessary until you have finalized the content of your delivery.

Once this is done, you can [prepare and send your delivery](../monitor/prepare-send.md) to the main target.

## Access sent test emails {#access-proofs}

Once the test emails have been sent, you can access dedicated logs from the **[!UICONTROL View test log]** button.

These logs allow you to access all the tests sent for the selected delivery, and to visualize specific statistics related to their sending. [Learn how to monitor delivery logs](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

You can also access sent tests from the [deliveries list](../msg/gs-messages.md), like any delivery.

![](assets/simulate-deliveries-list.png)
