---
audience: end-user
title: Prepare and send an email
description: Learn how to prepare and send an email with Campaign Web user interface
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
---
# Prepare and send your email {#prepare-send}

## Prepare the send {#prepare}

When you define your [content](../email/edit-content.md), [audience](../audience/add-audience.md), and [schedule](../msg/gs-messages.md#schedule-the-delivery-sending-gs-schedule), you are ready to prepare your email delivery.

During the delivery preparation, the target population is calculated, and the message content is generated for each profile included in the target. Once the preparation finishes, the messages are ready to be sent, either immediately or at the scheduled date and time.

The validation rules used during delivery preparation are described in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/send.html){target="_blank"}.

The main steps to prepare the send are listed below.

1. From the delivery dashboard, click **[!UICONTROL Review and send]**.

    ![Review and send button in the delivery dashboard](assets/email-review-and-send.png){zoomable="yes"}

1. Click the **[!UICONTROL Prepare]** button located in the top right corner, and confirm.

    ![Prepare button in the delivery dashboard](assets/email-prepare.png){zoomable="yes"}

    >[!NOTE]
    >
    >If you schedule your delivery and disable the **[!UICONTROL Enable confirmation before sending]** option, the preparation and sending steps are grouped together under the **[!UICONTROL Prepare and send]** button. [Learn more about scheduling](../msg/gs-deliveries.md#gs-schedule)

1. The preparation progress is displayed. Depending on the size of the targeted population, this operation may take some time.

    You can stop the preparation at any time using the **[!UICONTROL Stop preparation]** button.

    ![Stop preparation button in the delivery dashboard](assets/email-stop-preparation.png){zoomable="yes"}

    >[!NOTE]
    >During the preparation phase, no messages are sent. You can start or stop this without risk of impacting anything.

1. When the preparation finishes, check the KPIs. If the number of messages to send does not match your expectations, modify your audience and restart the preparation.

    ![Preparation complete screen showing KPIs](assets/email-preparation-complete.png){zoomable="yes"}
    
    Here are the different KPIs displayed:

    * **[!UICONTROL Targeted]**: the number of recipients targeted.
    * **[!UICONTROL To deliver]**: the number of messages that will be sent.
    * **[!UICONTROL To exclude]**: the number of messages excluded by a [typology rule](../advanced-settings/delivery-settings.md#typology).

1. Click the **[!UICONTROL Logs]** button, and check that there are no errors. The last log message displays any error messages and the number of errors. [Learn more](delivery-logs.md)

    ![Logs button in the delivery dashboard](assets/email-prepare-logs.png){zoomable="yes"}

1. If the preparation detects a critical error preventing the delivery from being sent, the preparation status appears as failed in the delivery dashboard.

    ![Error status in the delivery dashboard](assets/email-prepare-error.png){zoomable="yes"}

1. If you make any changes to your delivery after the preparation, restart the preparation for those changes to be taken into account.

Once the preparation is complete with no errors, your message is ready to be sent.

## Send the message {#send}

Once the [preparation](#prepare) is complete, you can send your email.

If the message is scheduled, it is sent at the defined date and time. [Learn more about scheduling](../msg/gs-deliveries.md#gs-schedule)

### Send immediately {#send-immediately}

To immediately send an email, follow the steps below.

1. From the delivery dashboard, click the **[!UICONTROL Send]** button in the top right corner.

    ![Send button in the delivery dashboard](assets/email-send.png){zoomable="yes"}

1. Confirm this action to immediately send the message to the main target.

1. The sending progress is displayed.

### Schedule the send {#schedule-the-send}

If you schedule your email to send it at a later date and time, follow the steps below.

1. Before you click the **[!UICONTROL Review and send]** button, ensure you define a schedule for your email. [Learn more about scheduling](../msg/gs-deliveries.md#gs-schedule)

1. From the delivery dashboard, click the **[!UICONTROL Send as scheduled button]** in the top right corner.

    ![Send as scheduled button in the delivery dashboard](assets/email-send-as-scheduled.png){zoomable="yes"}

1. Click **[!UICONTROL Confirm sending]**. The delivery is sent on the scheduled date to the main target.

    >[!NOTE]
    >
    >If you disable the **[!UICONTROL Enable confirmation before sending]** option, the preparation and sending steps are grouped together under the **[!UICONTROL Prepare and send]** button. [Learn more about scheduling](../msg/gs-deliveries.md#gs-schedule)

## Pause or stop the sending {#pause-stop-sending}

Whether your delivery is scheduled or not<!--TBC-->, two actions can be performed at any time during the sending process:

* Click **[!UICONTROL Pause sending]** to interrupt the sending of the messages. You can resume sending at any time.

* Click **[!UICONTROL Stop sending]** to immediately interrupt sending. Neither preparation nor sending can be resumed once stopped.

![Pause or stop sending buttons in the delivery dashboard](assets/email-send-pause-or-stop.png){zoomable="yes"}

## Check the KPIs {#check-kpis}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Delivered"
>abstract="The number of messages successfully delivered. This indicator is updated every 5 minutes. The percentage displayed is based on the total number of sent messages."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="Understand KPIs"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Opens"
>abstract="The number of opened messages. This indicator is updated every 5 minutes. The percentage displayed is the ratio of the number of distinct opens compared with the number of delivered messages."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="Understand KPIs"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Clicks"
>abstract="The number of recipients who clicked at least once in the email. This indicator is updated every 5 minutes. The percentage displayed is the ratio of the number of distinct clicks compared with the number of delivered messages."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="Understand KPIs"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Sent"
>abstract="Total number of messages processed during the delivery analysis."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="Understand KPIs"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Errors"
>abstract="Total of errors cumulated during delivery and automatic return processing in relation to the total number of sent messages."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="Understand KPIs"

Once the send is complete, you can check the KPIs displayed:

![KPIs displayed after sending](assets/email-send-kpis.png){zoomable="yes"}

* **[!UICONTROL Sent]**: the number of messages delivered. The percentage displayed is based on the total number of messages to deliver.

* **[!UICONTROL Delivered]**: the number of messages successfully delivered. The percentage displayed is based on the total number of sent messages.

* **[!UICONTROL Opens]**: the number of opened messages. The percentage displayed is the number of distinct opens compared with the number of delivered messages.

* **[!UICONTROL Clicks]**: the number of recipients who clicked at least once in the email. The percentage displayed is the number of distinct clicks compared with the number of delivered messages.

* **[!UICONTROL Errors]**: the number of emails with the error status. The percentage displayed is based on the total number of sent messages.

>[!NOTE]
>
>All the indicators are updated every 5 minutes after the delivery starts. The delivery preparation indicators are real-time.

Learn more about KPIs on [this page](../reporting/kpis.md).

You can also check the logs. [Learn more](delivery-logs.md)