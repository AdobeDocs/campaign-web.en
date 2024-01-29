---
audience: end-user
title: Sending using waves
description: Learn more about delivery settings in Campaign Web 
badge: label="Limited Availability"

---

# Send using waves {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Waves definition"
>abstract="Define waves to split deliveries into several batches instead of sending high volumes of messages at the same time."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Size of the wave"
>abstract="The size of the wave is required. Enter either a numerical value (number of messages), or a percentage (0-100%) in the size field."

To balance the load, you can divide deliveries into several batches. Configure the number of batches and their proportion with respect to the entire delivery.

>[!NOTE]
>
>You can only define the size and the delay between two consecutive waves. The recipient selection criteria for each wave cannot be configured.

1. Open the [delivery settings](delivery-settings.md#retries) and go to the **[!UICONTROL Delivery]** tab.
1. Select the **[!UICONTROL Send using multiple waves]** option and click the **[!UICONTROL Define waves...]** link.

1. To configure waves, you can either:

    * **[!UICONTROL Schedule multiple waves of the same size]**. For example, if you enter **[!UICONTROL 30%]** in the corresponding field, each wave will represent 30% of the messages included in the delivery, except the last one, which will represent 10% of the messages.

      In the **[!UICONTROL Interval]** section, specify the delay between the start of two consecutive waves. For example, if you enter **[!UICONTROL 2d]**, the first wave will start immediately, the second wave will start in two days, the third wave in four days, and so on.

    * **[!UICONTROL Schedule waves according to a calendar]**.

      In the **[!UICONTROL Start]** column, specify the delay between the start of two consecutive waves. In the **[!UICONTROL Size]** column, enter a fixed number or a percentage.

      In the example below, the first wave represents 25% of the total number of messages included in the delivery and will start immediately. The next two waves complete the delivery and are set to begin at six-hour intervals.

      A specific typology control rule, **[!UICONTROL Wave scheduling check]**, ensures that the last wave is planned before the delivery validity limit. Campaign typologies and their rules are configured in the **[!UICONTROL Typology]** tab of the delivery settings. Learn more on control rules in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html)

      >[!IMPORTANT]
      >
      >Make sure the last waves do not exceed the delivery deadline, which is defined in the **[!UICONTROL Validity]** tab. Otherwise some messages might not be sent. [Learn more](delivery-settings.md#validity)
      >
      >You must also allow enough time for retries when configuring the last waves. [Learn more](delivery-settings.md#retries)

1. To monitor your sends, go to the [delivery logs](../monitor/delivery-logs.md).

  You can see the deliveries that were already sent in the processed waves (**[!UICONTROL Sent]** status) and the deliveries to be sent in the remaining waves (**[!UICONTROL Pending]** status).

The two examples below are the most common use cases for using multiple waves.

* **During ramp-up process**

  When emails are sent using a new platform, Internet service providers (ISPs) are suspicious of IP addresses that are not recognized. If large volumes of emails are suddenly sent, the ISPs often mark them as spam.

  To avoid being marked as spam, you can progressively increase the volume sent using waves. This should ensure smooth development of the start-up phase and enable you to reduce the overall rate of invalid addresses.

  To do so, use the **[!UICONTROL Schedule waves according to a calendar]** option. For example, set the first wave to 10%, the second to 15%, and so on.

* **Campaigns involving a call center**

  When managing a telephone loyalty campaign, your organization has a limited capacity to process the number of calls to contact subscribers.

  Using waves, you can restrict the number of messages to 20 per day, which is the daily processing capacity of a call center.

  To do this, select the **[!UICONTROL Schedule multiple waves of the same size]** option. Enter **[!UICONTROL 20]** as the wave's size and **[!UICONTROL 1d]** in the **[!UICONTROL Period]** field.