---
audience: end-user
title: Send your first email
description: Learn how to send your first email with Campaign Web user interface
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
---

# Create your first email {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card3"
>title="Get started with emails"
>abstract="You can create a standalone email delivery, or create an email in the context of a campaign workflow. Learn how to create the delivery, select the audience, and design the email content."

Learn how to create your first targeted email. In this use case, you schedule the sending of an email to Silver and Gold loyalty members on a specific date.

Based on a predefined [design template](../email/create-email-templates.md), the email also features personalized content based on customer profile attributes.

➡️ [Discover this feature in video](#video) 

## Create the email delivery {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Select an email template"
>abstract="An email template is a specific delivery configuration that contains predefined settings, such as typology rules, personnalization or routing parameters. Templates are defined in the Campaign client console."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Define your email properties"
>abstract="The properties are the common delivery parameters that helps you to name and classify your delivery. The additional settings are optional. If your delivery is based on an extended schema defined in the Adobe Campaign v8 console, some specific **Custom Options** fields are available."

You can create a standalone email delivery, or create an email in the context of a campaign workflow. The steps below detail the procedure for a standalone (one-shot) email delivery. Learn more about delivery creation steps in Adobe Campaign in [this page](../msg/gs-deliveries.md).

To create a new standalone email delivery, follow the steps below.

1. Browse to the **[!UICONTROL Deliveries]** menu on the left rail, and click the  **[!UICONTROL Create delivery]** button.

    ![](../msg/assets/create-a-delivery.png)

1. Select **[!UICONTROL Email]** as the channel and choose an email delivery template from the list.

    >[!NOTE]
    >
    >Templates are pre-configured delivery settings saved for future use. [Learn more](../msg/delivery-template.md)

    ![](assets/channel-template.png){zoomable="yes"}

1. Click the **[!UICONTROL Create delivery]** button to confirm.
1. Enter a label for the delivery and configure additional options based on your needs:

    * **[!UICONTROL Internal name]**: assign a unique identifier to the delivery.
    * **[!UICONTROL Folder]**: store the delivery in a specific folder.
    * **[!UICONTROL Delivery code]**: use this field to organize your deliveries based on your own naming convention.
    * **[!UICONTROL Description]**: specify a description for the delivery.
    * **[!UICONTROL Nature]**: specify the nature of the email for classification purposes.<!--The content of the list is defined in the delivery template selected when creating the email.-->

    >[!NOTE]
    >
    >If you have extended your schema with specific custom fields, you can access them in the **[!UICONTROL Custom options]** section.

    ![](assets/email-properties.png){zoomable="yes"}

1. Additionally, advanced settings, such as typology rules and target mappings, can be accessed via the **[!UICONTROL Settings]** button located on the top right of the screen. These settings are pre-configured in the selected template, but can be edited as needed for this specific email. [Learn more](../advanced-settings/delivery-settings.md)

## Define the audience {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Select an audience for your delivery"
>abstract="Select the best audience for your marketing message. You can choose an existing audience (already defined in a Campaign v8 instance or from Adobe Experience Platform), create a new audience using the query modeler, or upload a file containing your audience. Control groups are not enabled for the **Select from file** option and vice versa."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html" text="Select the main audiences"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Set a control group"

In this use case, you send the email to an existing audience.

Additional instructions on how to work with audiences are available in [this section](../audience/about-recipients.md).

1. To select the audience for the email, click the **[!UICONTROL Select audience]** button and choose an existing audience from the list.

    In this example, we want to use an existing audience targeting customers belonging to the silver and gold loyalty points levels.

    ![](assets/create-audience.png){zoomable="yes"}

    >[!NOTE]
    >
    >Audiences available in the list originate either from your Campaign v8 instance, or from Adobe Experience Platform if the Destination/Source integration has been configured on your instance. This integration allows you to send Experience Platform segments to Adobe Campaign, and to send Campaign delivery and tracking logs over to Adobe Experience Platform. Learn how work with Campaign and Adobe Experience Platform in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

1. Once the audience is selected, you can further refine the target by applying additional rules.

    ![](assets/audience-selected.png){zoomable="yes"}

1. You can also set a control group to analyze the behavior of the email recipients compared to those who were not targeted. [Learn how to work with control groups](../audience/control-group.md)

## Define the email content {#create-content}

To start creating your email content, follow the steps below. In this use case, you use a predefined email [delivery template](../msg/delivery-template.md) to design your email.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. From the email delivery dashboard, click the **[!UICONTROL Edit content]** button.

    ![](assets/email-edit-content.png){zoomable="yes"}

   This brings you to a dedicated interface where you can configure the email content and access the Email Designer. [Learn more](edit-content.md)

    ![](assets/edit-content.png){zoomable="yes"}

1. Enter the subject line of your email and personalize it using the Expression Editor. [Learn how to personalize your content](../personalization/personalize.md)

    ![](assets/subject-line.png){zoomable="yes"}

1. To design the content of the email, click the **[!UICONTROL Edit email body]** button.

    Choose the method to use to create your email content. In this example, use a [predefined content template](create-email-templates.md).

    ![](assets/select-template.png){zoomable="yes"}

1. Once you have selected the template, it is displayed in the [Email Designer](create-email-content.md), where you can make any necessary edits and add personalization.

    For example, to add personalization to the email title, select the component block and click **[!UICONTROL Add Personalization]**.

    ![](assets/add-perso.png){zoomable="yes"}

1. Once you are satisfied with the content, save and close your design. Click **[!UICONTROL Save]** to return to the email creation screen.

    ![](assets/save-content.png){zoomable="yes"}

## Schedule the sending {#schedule}

When a delivery is sent in the context of a workflow, you must use the **Scheduler** activity. Learn more in [this page](../workflows/activities/scheduler.md). Steps below only apply to standalone deliveries.

1. Browse to the **[!UICONTROL Schedule]** section of the delivery properties.

1. Use the **[!UICONTROL Enable scheduling]** toggle to activate it.

1. Set the desired date and time for sending.

    ![](assets/schedule.png){zoomable="yes"}

Once you send the delivery, the actual sending starts on the contact date you have defined.

Learn more about delivery scheduling in [this section](../msg/gs-deliveries.md#schedule-the-delivery-sending).

## Preview an email & send proofs {#preview-test}

Before sending your email, you can preview and test it to ensure it meets your expectations.

In this use case, you preview the email and send proofs to specific email addresses while impersonating some of the targeted profiles.

Additional information on how to preview an email and send proofs are available in [this section](../preview-test/preview-test.md).

1. To review your email, click **[!UICONTROL Review and send]**. This displays a preview of your email, along with al the configured properties, audience and schedule. You can edit any of these elements by clicking the modify button.

1. To preview the email and send proofs, click the **[!UICONTROL Simulate content]** button. 

    ![](assets/review-email.png){zoomable="yes"}

    >[!NOTE]
    >
    >The **[!UICONTROL Simulate content]** button is disabled in specific contexts. Limitations are detailed [in this section](#content-simulation-limitations).

1. On the left-hand side, select the profile(s) you want to use to preview the email.

    The right pane displays a preview of the email based on the selected profile. If you have added multiple profiles, you can switch between them to preview the corresponding email.

    ![](assets/preview.png){zoomable="yes"}

    <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. To send proofs, click the **[!UICONTROL Send proofs]** button then choose the mode you want to use.

    In this example, use the **[!UICONTROL Substitute from main target]** mode, which sends proofs to specific email addresses while impersonating some of the profiles targeted by the email.

    ![](assets/proof-mode.png){zoomable="yes"}

1. Click **[!UICONTROL Add address]** and specify the email address(es) which receive the proofs.

    For each email address, select the profile to impersonate. You can also let Adobe Campaign select a random profile from the target.

    ![](assets/proof-test-profile.png){zoomable="yes"}

1. Click **[!UICONTROL Send proof]** and confirm the sending.

    Proofs are sent to the specified email addresses using the selected profile with the **[Proof x]** prefix.

    ![](assets/proof-sent.png){zoomable="yes"}

    You can check the status of the sending and access the sent proofs  at any time by clicking the **[!UICONTROL View proofs]** button in the simulate content screen.

### Content simulation limitations {#content-simulation-limitations}

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_multilingual"
>title="Content simulation is not supported"
>abstract="The **Simulate content** button is disabled because the multilingual delivery contains only one locale."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_reconcilied_deliveries"
>title="Content simulation is not supported"
>abstract="The **Simulate content** button is disabled because it is not compatible with reconciled deliveries in this phase."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_ffda"
>title="Content simulation is not supported"
>abstract="The **Simulate content** button is disabled because not supported in Campaign Enterprise Full Federated Access (FFDA) mode."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_no_file"
>title="Content simulation is not supported"
>abstract="The **Simulate content** button is disabled because no content has been uploaded."

In some cases, you cannot perform content simulation, and the **[!UICONTROL Simulate content]** button is disabled.

Content simulation is not supported in these cases:

<!--* When a multilingual delivery contains only one locale,-->
* With reconciled deliveries,
* When your Campaign deployment model is [Adobe Campaign Enterprise Full Federated Access (FFDA)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/ffda/enterprise-deployment){target="_blank"}
* When no file has been uploaded.

## Send and monitor the email {#prepare-send}

After reviewing and testing your email, you can launch its preparation and send it.

1. To launch the preparation of the email, click **[!UICONTROL Prepare]**. [Learn how to prepare an email](../monitor/prepare-send.md)

    ![](assets/preparation.png){zoomable="yes"}
 
1. Once your email is ready to be sent, click the **[!UICONTROL Send]** button (or **[!UICONTROL Send as scheduled]** if you have scheduled its sending) and confirm the sending.

1. During the sending process, you can track its progress and view statistics in real-time directly in this screen.

    ![](assets/sending-email.png){zoomable="yes"}

    <!--
    ![](assets/sent-email.png){zoomable="yes"}-->

    You can also access detailed information on the sending by clicking the **[!UICONTROL Logs]** button. [Learn how to monitor delivery logs](../monitor/delivery-logs.md)     

1. After the email has been sent, you can access dedicated reports for further analysis by clicking the **[!UICONTROL Reporting]** button.

![](assets/reports.png){zoomable="yes"}

## How-to video {#video}

Learn how to create an email delivery from scratch, define the audience, design the content, simulate preview, and send a proof.

>[!VIDEO](https://video.tv.adobe.com/v/3425866/?quality=12)
