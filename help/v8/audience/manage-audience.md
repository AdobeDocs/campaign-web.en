---
audience: end-user
title: Monitor & manage audiences
description: Learn how to monitor and manage audiences in Adobe Campaign Web
badge: label="Beta"
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
---
# Monitor & manage audiences {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Audience error"
>abstract="Audience data is not available. Please wait the end of the workflow execution."

The audience is the main target of your delivery: the recipients who receive the messages. The type of audience depends on the target mapping defined in the delivery template. Learn more about delivery templates in [this page](../msg/delivery-template.md). 

To define the population of an audience, you can:

* [Create new audiences](create-audience.md) from the **[!UICONTROL Audiences]** menu,
* [Select an existing audience](add-audience.md) created as a list in the client console or coming from Adobe Experience Platform,
* [Build a new audience](../query/query-modeler-overview.md) with the rule builder by defining and combining filtering criteria,
* [Use an audience from an external file](file-audience.md). This option is only available for standalone email deliveries, and cannot be used in campaign deliveries.

When targeting an audience, you can also define **control groups** to avoid sending messages to a portion of your audience, and measure the impact of your campaigns. [Learn how to set a control group](control-group.md)

>[!NOTE]
>
>When sending messages in the context of a campaign workflow, the audience is defined in a specific **Build audience** workflow activity. In this context, you cannot load an audience from a file for an email delivery, and the audience is defined only in this dedicated activity. Learn how to define the audience of your delivery in a campaign workflow in [this section](../workflows/activities/build-audience.md)

The list of audiences available for use in Campaign Web is accessible from the **[!UICONTROL Audiences]** menu.

![](assets/audiences-list.png)

Audiences can originate from multiple sources. The **[!UICONTROL Origin]** columns indicates where a given audience has been created:

* **[!UICONTROL Adobe Campaign]**: These audiences are created in the Adobe Campaign V8 console. Learn more in [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** These audiences are created within Adobe Experience Platform and are integrated into Campaign Web using the Adobe Sources and Destinations integration. Learn how to set up this integration in [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

>[!NOTE]
>
>To use Adobe Experience Platform audiences in Campaign, you need to configure the integration with Adobe Sources and Destinations. Refer to [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

* **[!UICONTROL Adobe Campaign WebUI]**: These audiences are created using Campaign Web audience workflows. [Learn how to create audiences](create-audience.md)

To get more information on an audience, open it from the list. The audience properties display, alongside with the number of profiles included in the audience. You can refresh the audience count at any time using the **[!UICONTROL Calculate]** button.

The **[!UICONTROL Data]** tab allows you to vizualise the profiles that are part of the audience. You can customize this view by adding more columns or leverage advanced filters to refine the displayed data.

![](assets/audiences-details.png)

To duplicate or delete an audience, click the **[!UICONTROL More action]** button available in the audiences list next to the audience name or inside an audience details screen.
