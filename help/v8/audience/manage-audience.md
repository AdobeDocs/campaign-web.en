---
audience: end-user
title: Monitor & manage audiences
description: Learn how to monitor and manage audiences in Adobe Campaign Web
badge: label="Beta" 
---

# Monitor & manage audiences {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Audience error"
>abstract="Audience data is not available. Please wait the end of the workflow execution."

The list of audiences available for use in Campaign Web is accessible from the **[!UICONTROL Audiences]** menu.

![](assets/audiences-list.png)

Audiences can originate from multiple sources. The **[!UICONTROL Origin]** columns indicates where a given audience has been created:

* **[!UICONTROL Adobe Campaign]**: These audiences are created in the Adobe Campaign V8 console. Learn more in [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** These audiences are created within Adobe Experience Platform and are integrated into Campaign Web using the Adobe Sources and Destinations integration. Learn how to set up this integration in [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

>[!NOTE]
>
>To use Adobe Experience Platform audiences in Campaign, you need to configure the integration with Adobe Sources and Destinations. Refer to [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

* **[!UICONTROL Adobe Campaign WebUI]**: These audiences are created using Campaign Web audience workflows. [Learn how to create audiences](create-audience.md)

To get more information on an audience, open it from the list. The audience properties display, alongside with the number of profiles included in the audience. You can refresh the audience count at any time using the **[!UICONTROL Calculate]** button.

The **[!UICONTROL Data]** tab allows you to vizualise the profiles that are part of the audience. You can customize this view by adding more columns or leverage advanced filters to refine the displayed data.

![](assets/audiences-details.png)

To duplicate or delete an audience, click the **[!UICONTROL More action]** button available in the audiences list next to the audience name or inside an audience details screen. 