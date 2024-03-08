---
audience: end-user
title: Send proofs
description: Learn how to define and send proofs
exl-id: b2677579-c95d-443d-b207-466af364c208
---
# Send proofs {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Preview mode"
>abstract="Preview and test the message by including the test population to the main target."

Once your message content has been defined, you can preview and test it by sending proofs to test profiles. If you inserted personalized content, you can check how this content is displayed in the message, using test profile data.

To detect possible errors in the message content or personalization settings, send proofs to test profiles before sending it to the target audience. A proof should be sent each time a change is made, to validate the latest content. Sending proofs is an important step in validating your campaign and identifying potential issues. The proof recipients can check various elements such as links, opt-out links, images, or mirror pages, as well as detect any errors in the rendering, content, personalization settings and delivery configuration.

## Simulate content with test profiles {#simulate-content-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Test population"
>abstract="Select a test population mode."

Before sending a proof, make sure you define a target audience for you delivery. [Learn more](../audience/add-audience.md)

To start testing your message content:

1. Edit the content of your delivery.
1. Click the **[!UICONTROL Simulate content]** button. 
1. Click the **[!UICONTROL Send proof]** button to send proofs.

    ![](assets/simulate-test-button-email.png){zoomable="yes"}

1. Select your proof recipients.

    Depending on the message channel, proofs can be sent to the following types of recipients: 

    * For SMS and emails, you can use [test profiles](#test-profiles), which are specific additional recipients in the database. You can also use the [substitution from main target](#substitution-profiles) mode, which sends the proof to an email test address or phone number, and use personalization data of an existing profile. This allows you to experience the message as the recipients would, giving you an accurate representation of the content that the profile will receive.

    * For push messages, you can use [subscribers](#subscribers), which are fictitious subscribers added to the database. They are created in the [!DNL Campaign] console. Learn more in [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

    Detailed configuration for each mode is available below. 

## Use test profiles {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="Target of the proof"
>abstract="You can upload a second file as 'target of the proof', if you wish to test your delivery before sending to the main target."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="Upload profiles"
>abstract="You can upload a second file with additional profiles if you like to test your delivery with a different set from the set you have used for the main target."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_sample"
>title="Template file"
>abstract="The formatting of the file must be the same as the original file.<br/>Supported file formats: txt, csv. Maximum file size: 15MB. Use first line as column header."

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="Include test profiles in the main audience"
>abstract="Enable this option to also send the final message to the proof recipients."

Test profiles are additional recipients in the database. They are created from the **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]** menu. [Learn more](../audience/test-profiles.md#create-test-profiles)

The steps to send proofs to test profiles are detailed below. 

1. From the content of your delivery, click the **[!UICONTROL Simulate content]** button, and the **[!UICONTROL Send proof]** button.

1. From the **[!UICONTROL Mode]** drop-down list, choose **[!UICONTROL Test profiles]** to target fictitious recipients that will receive the proof or SMS delivery.

    ![](assets/simulate-profile-mode.png){zoomable="yes"}

1. If you have already selected profiles to [preview the message](preview-content.md) in the content simulation screen, those profiles are pre-selected as proofs recipients. You can clear your selection and/or add additional recipients using the **[!UICONTROL Add test profile(s)]** button.

1. When browsing the test profile or profile lists, you can use filters to refine your search. For example, you can define a rule to find all test profiles whith the **[!UICONTROL Prospect]** status. Learn how to add rules using the [query modeler](../query/query-modeler-overview.md).

    ![](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. To also send the final message to the recipients of the proof, select the **[!UICONTROL Include test population in the main target]** option.

    ![](assets/simulate-include-test.png){zoomable="yes"}

1. Once the test profiles are selected, you can [send the proof](#send-test).

## Substitute profile data {#substitution-profiles}

Use profile substitution to send proofs to a specific email address or phone number, while displaying data from an existing profile of the [!DNL Adobe Campaign] database. This mode can only be selected if the audience of the delivery has been defined.

To substitute profile data from the main target, follow the steps below:

1. From the content of your delivery, click the **[!UICONTROL Simulate content]** button, and the **[!UICONTROL Send proof]** button.

1. From the **[!UICONTROL Mode]** drop-down list, choose **[!UICONTROL Substitute from main target]** to send a proof to a specific email address or phone number while displaying data from an existing profile.

    >[!CAUTION]
    >
    >If you have not selected an [audience](../audience/about-recipients.md) for your delivery, the **[!UICONTROL Substitute from main target]** option will be greyed out and you will not be able to select substitution profiles.

1. Click the **[!UICONTROL Add address]** button and specify the email address or phone number that will receive the proof.

    ![](assets/simulate-add-substitution-address.png){zoomable="yes"}

    >[!NOTE]
    >
    >You can enter any email address or phone number. This allows you to send proofs to any recipients, even if they are not users of [!DNL Adobe Campaign].

1. Select the profile from the target you defined for your delivery to use as substitute. You can also let [!DNL Adobe Campaign] select a random profile from the target. The profile data from the selected profile will be displayed in the proof.

1. Confirm the recipient and repeat the operation to add as many email addresses or phone numbers as needed.

    ![](assets/simulate-profile-substitute.png){zoomable="yes"}

1. To also send the final message to the recipients of the proof, select the **[!UICONTROL Include test population in the main target]** option.

1. Once the substitution profiles are selected, you can [send the proof](#send-test).

## Send proofs to app subscribers {#subscribers}

When designing with push notifications, proofs can be only sent to your app subscribers. To select them, follow the steps below.

1. From the content of your push delivery, click the **[!UICONTROL Simulate content]** button, and the **[!UICONTROL Send proof]** button.

    ![](assets/simulate-test-button-push.png){zoomable="yes"}

1. If you have already selected subscribers to [preview the delivery](preview-content.md) in the content simulation screen, those profiles are pre-selected as test subscribers.

    You can clear your selection and/or add additional subscribers using the dedicated button.

    ![](assets/simulate-test-subscribers.png){zoomable="yes"}

1. To also send the final push notification to the test subscribers, select the **[!UICONTROL Include test population in the main target]** option.

1. Once the subscribers are selected, you can [send the proof](#send-test).

## Send the proof {#send-test}

To send the proof to the selected recipients, follow the steps below.

1. Click the **[!UICONTROL Send proof]** button.

1. Confirm the sending.

    ![](assets/simulate-send-test.png){zoomable="yes"}

1. Send as many proofs as necessary until you have finalized the content of your delivery.

Once done, you can prepare and send your delivery to the main target. Learn how in the dedicated sections below:

* [Send your email](../monitor/prepare-send.md)
* [Send your push notification](../push/send-push.md#send-push)
* [Send your SMS delivery](../sms/send-sms.md#send-sms)

## Access sent proofs {#access-test-deliveries}

Once the proofs have been sent, you can access their logs from **[!UICONTROL Simulate content]** screen.

These logs allow you to access all the proofs sent for the selected delivery, and to visualize specific statistics related to their sending. [Learn how to monitor delivery logs](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png){zoomable="yes"}

You can also access sent proofs from the [delivery list](../msg/gs-messages.md), like any delivery.

![](assets/simulate-deliveries-list.png){zoomable="yes"}
