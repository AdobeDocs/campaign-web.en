---
audience: end-user
title: Test email rendering
description: Learn how to test your email rendering in Campaign Web UI
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
badge: label="Alpha" type="Positive"
---

# Test the email rendering {#email-rendering}

Before sending your email, make sure your message is displayed to the recipients in an optimal way on a variety of web clients and devices.

To do this, you can leverage your **Litmus** account into [!DNL Adobe Campaign] to instantly preview your email rendering in different contexts and check compatibility in major desktops and applications (webmail, message service, mobile, etc.).

>[!CAUTION]
>
>Using email rendering in Campaign sends a test email to a third-party system (Litmus) that is not under the control of Adobe. To access or delete such data, you will need to contact that third party directly. By using email rendering, you acknowledge Adobe is not responsible for any data you may send to that third-party system.

To access email rendering capabilities, you need to:

* Have a Litmus account
* Select test profiles - Learn how in [this section](preview-content.md)

Then, follow the steps below.

1. In the [Edit content](../content/edit-content.md) screen or in the [Email Designer](../content/get-started-email-designer.md), click the **[!UICONTROL Simulate content]** button.

1. Select the **[!UICONTROL Render email]** button.

    ![](assets/simulate-rendering-button.png)

1. Click **Connect your Litmus account** in the upper right section.

    ![](assets/simulate-rendering-litmus.png)

1. Enter your credentials and sign in.

    ![](assets/simulate-rendering-credentials.png)

1. Click the **Run test** button to generate email previews.

1. Check your email content in popular desktop, mobile and web-based clients.

    ![](assets/simulate-rendering-previews.png)

>[!CAUTION]
>
>When connecting your Litmus account with [!DNL Campaign], you agree that test messages are sent to Litmus. Once sent, these emails are no longer managed by Adobe. As a consequence, Litmus data retention email policy applies to these emails, including personalization data that may be included in these test messages.

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![](assets/render-context.png)

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->
