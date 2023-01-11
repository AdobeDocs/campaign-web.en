---
audience: end-user
title: Send proofs
description: Campaign v8 Web documentation
exl-id: b2677579-c95d-443d-b207-466af364c208
---
# Send proofs {#send-proofs}

![](../assets/do-not-localize/badge.png)

Sending test emails allows you to validate your email and check various elements like links, opt-out links and mirror pages, images and detect possible errors.

Proofs can be sent to two types of recipients:

* **Test profiles**: send proofs to seed addresses, which are additional and fictitious recipients in the database,
* **Substitution profiles**: send proofs to a specific email address using an existing profile. This allows you to place yourself in the position of the profiles and get an exact representation of the message that the profile will receive.

## Select the proofs recipients {#recipients}

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Test]** button then use the **[!UICONTROL Mode]** drop-down list to choose the type of recipients that will receive the proofs:

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### Send proofs to test profiles

1. Choose the **[!UICONTROL Use test profiles]** mode.

1. Add the test profiles that will receive the test emails.

    <!--FOR BETA: You can also build an audience to select test profiles based on your own criteria using the **[!UICONTROL Add test audience]** button.-->

    ![](assets/test-profiles-audience.png)

### Send proofs to substitution profiles

1. Choose the **[!UICONTROL Substitution from target]** mode.

1. Add the email address(es) that will receive the proofs.

    >[!NOTE]
    >
    >You can specify any email address. This allows you to send proofs to any users, even if they are not users of Adobe Campaign V8.

1. For each email address, select the profile from the target to use. You can also let Adobe Campaign select a random profile from the target.

    ![](assets/substitution.png)

Once the proof recipients have been selected, you can send the test email. [Learn how to send proofs](#send)

>[!NOTE]
>
>If you want to send the final email message to the recipients of the proofs, enable the **[!UICONTROL Include test population in the main target]** option on.

## Send the proofs {#send}

To send the proofs to the selected recipients, click **[!UICONTROL Send test email]** then confirm the sending.

![](assets/send-proof.png)

Send as many proofs as necessary until you have finalized the content of your delivery. Once this is done, you can send the email to the main target. [Learn how to prepare and send your email](../monitor/prepare-send.md)

## Access sent proofs {#access-proofs}

Once the proofs have been sent, you can access dedicated logs from the **[!UICONTROL View test email log]** button. These logs allow you to access all the proofs sent for the selected delivery, and to visualize specific statistics related to their sending.

![](assets/proof-log.png)

You can also access proofs from the deliveries list, like any delivery.

![](assets/delivery-list.png)
