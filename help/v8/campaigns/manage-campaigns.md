---
audience: end-user
title: Get started with campaigns
description: Learn how to start with cross-channel campaigns
badge: label="Beta" 
---

# Access and manage your campaigns{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Campaign schedule"
>abstract="Set or modify your campaign schedule."

To create a new campaign, or manage your existing campaigns, click the **[!UICONTROL Campaigns]** menu on the left navigation. 

## List of campaigns {#access-campaigns}

In the campaign list, two tabs are available:

* The **Browse** tab lists all existing campaigns. You can click a campaign to open its dashboard or create a new campaign by clicking the **Create campaign** button. See this [section](create-campaigns.md#create-campaigns).

* The **Templates** tab lists all available campaign templates. You can view an existing template or create a new one. [Read more](manage-campaign-templates.md).

![Campaign list](assets/campaign-list.png)

By default, each campaign in the list displays information about its current status, creation date, the last time it was modified, etc.

You can customize the displayed columns by clicking the **Configure column for a custom layout** icon located in the upper-right corner of the list. This allows you to add additional information to the list. In addition, a search bar and filters are available to facilitate easy searching within the list. [Learn more](../get-started/user-interface.md#list-screens).

For example, you can filter on your campaign schedule. Open the filter panel and use the **Start - End Date** section:

![Campaign filter](assets/campaign-filter-on-dates.png)

## Campaign dashboard{#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="List of deliveries in the campaign"
>abstract="The **Deliveries** tab lists all deliveries linked to the current campaign. Click the name of a delivery to edit it. Use the Create delivery button to add a new delivery for this campaign."

In the **Browse** tab of the campaign list, click a campaign to display its details. 

![Campaign dashboard](assets/campaign-dashboard.png)

The status and schedule of the campaign is displayed at the top of the screen. You can use the **Configure campaign settings** icon to modify the campaign's properties that were defined when creating the campaign. Three buttons are available that allow you to view logs, reporting, duplicate or delete the campaign. See this [section](create-campaigns.md#create-campaigns) 

Two tabs are available:

* The **Workflows** tab lists all workflows linked to the campaign. This tab also allows you to create a new workflow inside the campaign. See this [section](create-campaigns.md#create-campaigns).

* The **Deliveries** tab lists all deliveries linked to the current campaign. You can also create a new delivery inside the campaign. See this [section](create-campaigns.md#create-campaigns).

## Duplicate and delete a campaign

You can duplicate or delete a campaign:

* from the list of campaigns, click the ellipsis button then select **Duplicate** or **Delete**.
* from the campaign itself, click the **More** button then select **Duplicate** or **Delete**.

>[!NOTE]
>
>The **Deliveries** tab displays all deliveries linked to the campaign. However, deliveries created in a workflow cannot be deleted from there. To delete a delivery created in the context of a workflow, you must delete the delivery activity from the workflow. [Learn more](../msg/gs-messages.md#delivery-delete).

## Work with campaign templates{#manage-campaign-templates}

Campaign templates contain pre-configured settings which can be reused for creating new workflows. A set of built-in templates is available to help you get started. You can create and configure your campaign templates and then create campaigns from these templates.

A campaign template can store the following information:

* the campaign's **Properties** and **Schedule** settings 
* workflow templates
* delivery templates

To create a campaign template, follow the steps below:

1. Click the **[!UICONTROL Campaigns]** menu, browse to the **Templates** tab, then click the **[!UICONTROL Create template]** button.
1. Select the **Template** to use and provide a label for the campaign. This allows you to base your new template on a template already created.
1. If needed, you can change the following **Additional options**: internal name, folder, assignee, description and nature.
1. Define the **Schedule** of your campaign. Learn how to set your campaign schedule in [this section](create-campaigns.md#campaign-schedule)
1. Click **Create**.
1. Add workflows and delivery templates to your campaign.
