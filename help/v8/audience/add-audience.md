---
audience: end-user
title: Select an existing audience
description: Learn how to select an audience
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Beta" 
---

# Select an existing audience {#add-audience}
 
>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Select an existing audience"
>abstract="Browse the list to select an existing audience. Use the 'Show filters' icon to filter the list, or select a specific folder."

This section explains how to select an existing audience, when defining the target population of an email delivery.

You can also:

* Build a new audience. [Learn more](segment-builder.md)
* Load an audience from an external file (for emails only). [Learn more](file-audience.md)
* Use an Adobe Experience Platform audience. [Learn more](aep-audience.md).


To select an existing audience for your message, follow the steps below:

1. From the **Audience** section of the delivery creation assistant, click the **[!UICONTROL Select audience]** button.

   ![](assets/create-audience.png)

1. Choose **[!UICONTROL Select audience]** to use an existing audience. To create a new audience to be used in this email, choose **Create your own**. Refer to this [section](segment-builder.md).

    This screen displays all existing audiences, for the current folder.

    ![](assets/create-audience2.png)

      Audiences are created from the **Audience** left menu. They can also be created in the Client Console.
      
      To use Adobe Experience Platform audiences, you need to configure the integration with Destinations. Refer to the [Adobe Experience Platform Destinations documentation](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html){target="_blank"}.

      >[!IMPORTANT]
      >
      >In that version of the product, when building rules, selecting the audience of a delivery, or when building an audience in a workflow, some predefined filters are not available in the user interface. You can still use them. [Learn more](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

1. Choose an audience and click **Select**.
1. Use the **Show filters** icon to display filtering options. Click **Add rules** to access the rule builder: using the rule builder lets you create advanced filters for the list of audiences. Learn how to use the rule builder in this [section](segment-builder.md).

   ![](assets/create-audience4.png)

1. Click **Save**. 

You can also set a control group to measure the impact of your campaigns. The control group do not receive the message. This allows you to compare the behavior of the population which received the message with the behavior of contacts which did not. Learn more in [this section](control-group.md).