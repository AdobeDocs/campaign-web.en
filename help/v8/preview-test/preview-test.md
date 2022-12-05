---
audience: end-user
title: Preview and test your email
description: Campaign v8 Web documentation
exl-id: ce10c89d-d9b8-4529-84cb-f58f8c71c733
---
# Preview and test your email {#preview-test-send}

>[!NOTE]
>
>This documentation is under construction and frequently updated. The final version of this content will be ready in January 2023.

Once the email content has been defined, you can check how it will display before sending it. This allows you to test the email in order to detect possible errors in content or personalization settings.

To do this, Adobe Campaign allows you to:

* [Preview the email content and personalization](#preview) using profile data,
* [Check the email rendering](#rendering) of the email in popular desktop, mobile and web-based clients,
* [Send proofs](#send-proofs) to specific recipients in order to test and validate the email.

These actions are performed from the **[!UICONTROL Simulate content]** button which is accessible when creating the content of your email:

![](assets/simulate.png)

## Preview your content {#preview}

Adobe Campaign allows you to use profiles to preview the content of your email before sending in order to check personalization and how your recipients will see them.

Messages preview can be performed using:

* **Test profiles**: send proofs to additional recipients in the database that are not part of the email target,
* **Profiles from the email audience**: test the email by placing yourself in the position of one of the targeted profiles. This allows you to get an exact representation of the message that the profile will receive like custom fields, personalized information...

To preview the content of your email, follow these steps:

1. Choose the profile(s) to use to preview your email content. To do this, click the **[!UICONTROL Select profile(s)]** button then use the **[!UICONTROL Test profiles]** and **[!UICONTROL Profiles]** tab to select one or multiple profile(s). 

    ![](assets/preview-profile.png)

1. Once your profiles have been selected, a preview of the email displays in the right pane. Personalized elements are replaced by the data from the selected profile.

    If you have added multiple profiles, you can switch between each of them in the list to preview the corresponding email.

    ![](assets/preview.png)

## Rendering {#rendering}

Before sending your email, make sure that your message will be displayed to the recipients in an optimal way on a variety of web clients, web mails and devices.

To do this, Adobe Campaign allows you to preview the sent message in the different contexts in which it may be received and check the compatibility in major desktops and applications (webmail, message 
service, mobile, etc.).

To test your email rendering, follow these steps:

1. Click the **[!UICONTROL Render email]** button.

    ![](assets/render.png)

1. The left pane provides various desktop, mobile and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![](assets/render-context.png)

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

## Send proofs {#send-proofs}

Sending proofs allows you to validate your email and check various elements like links, opt-out links and mirror pages, images and detect possible errors.

Proofs can be sent to two types of recipients:

* Test profiles / audiences: send proofs to additional recipients in the database that are not part of the email target,

* Substitution profiles: send proofs to a specific email address using a profile from the email audience. This allows you to place yourself in the position of one of the targeted profiles and get an exact representation of the message that the profile will receive.
 
To send proofs, follow these steps:

## Select the proofs recipients {#recipients}

Click the **[!UICONTROL Test]** button then use the **[!UICONTROL Mode]** drop-down list to choose the type of recipients that will receive the proofs:

>[!BEGINTABS]

>[!TAB Send proofs to test profiles]

1. Click the **[!UICONTROL Test]** button then choose the **[!UICONTROL Use test profiles]** mode.

1. Add the test profiles that will receive the test emails.

    You can also build your own audience to select test profiles based on your own criteria using the **[!UICONTROL Add test audience]** button.

![](assets/test-profiles-audience.png)

>[!TAB Send proofs to substitution profiles]

1. Click the **[!UICONTROL Test]** button then choose the **[!UICONTROL Substitution from target]** mode.

1. Add the email address(es) that will receive the proofs.

1. For each email address, select the profile from the target to use. You can also let Adobe Campaign select a random profile from the target.

![](assets/substitution.png)

>[!ENDTABS]

<!--

### Send proofs to test profiles {#proofs-test-profiles}

1. Click the **[!UICONTROL Test]** button then choose the **[!UICONTROL Use test profiles]** mode.

1. Add the test profiles that will receive the test emails.

    You can also build your own audience to select test profiles based on your own criteria using the **[!UICONTROL Add test audience]** button.

    ![](assets/test-profiles-audience.png)

### Send proofs to substitution profiles {#proofs-substitution}

1. Click the **[!UICONTROL Test]** button then choose the **[!UICONTROL Substitution from target]** mode.

1. Add the email address(es) that will receive the proofs.

    For each email address, select the profile from the target to use. You can also let Adobe Campaign select a random profile from the target.

    ![](assets/substitution.png)

    -->

## Send the proofs {#send}

1. Once the proofs recipients have been selected, click **[!UICONTROL Send test email]** then confirm the sending.

    >[!NOTE]
    >
    >The **[!UICONTROL Include test population in the main target]** allows you to send the final email message to the recipients of the proofs.

1. After the proofs have been sent, you can access dedicated logs from the **[!UICONTROL View test email log]** button. 

    These logs allow you to access the sent proofs, and specific statistics related to the proof sending.

    ![](assets/proof-log.png)


1. Send as many proofs as necessary until you have finalized the content of your delivery. Once this is done, you can send the delivery to the main target.




<!--
By default, the subject of the proof is prefixed by ‘Proof #’, where # is the number of the proof. You can change this prefix in the Label prefix field.

Use address substitution in proof
Instead of selecting dedicated recipients in the database, you can use the Substitution of the address option.
This option lets you use the recipient profiles of the delivery and replace their email addresses with one or more other addresses that will receive the proof.
When this option is selected, the proof addresses will be filled in via a special editor that lets you configure the substitution(s).
Configuration is performed as follows:
Click the Add icon to define a substitution.
Enter the recipient address to be used, or select it from the list.
Select the profile to use in the proof: save the Random value in the Profile to use column to use the data of any profile of the target in the proof.
Click the Detail icon to select a profile from the main target, as in the following example:
You can define as many substitution addresses as necessary.



Click the profile selection button to display the list of profiles targeted by the message.
Select the profile to use for testing, then enter in the Address field the desired substitution address, then click Confirm. All proofs targeting the profile will be sent to this email address, rather than to the one defined in the database for this profile.
If you want to add a specific prefix to the proofs’ subject line, fill in the Subject line prefix field.
The profile is added to the list, with its associated substitution address and prefix. Repeat the above steps for all the profiles that you want to use for testing, then click Confirm.
f you want to send a proof to multiple substitution addresses for a same profile, you must add this profile as many times as required.
In the example below, the proof based on the profile John Smith will be sent to two different substitution addresses:
Once all profiles and substitution addresses are defined, you can send a proof to test the message. To do this, click the Test button, then select the type of test to perform.
Note that if no test profile has been added to the message target, the Email rendering and Proof + Email rendering options are not available. For more information on proofs sending, refer to this section.

-->


