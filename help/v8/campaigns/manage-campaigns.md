---
audience: end-user
title: Get started with campaigns
description: Learn how to start with cross-channel campaigns
exl-id: 690229e7-73e1-4cc1-b69a-f3e5d8de58af
---
# Access and manage your campaigns{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Campaign schedule"
>abstract="Set or modify your campaign schedule."

To access and manage your campaigns, click the **[!UICONTROL Campaigns]** menu on the left navigation. 

## List of campaigns {#access-campaigns}

In the campaign list, two tabs are available:

* The **Browse** tab lists all existing campaigns. You can click a campaign to open its dashboard or create a new campaign by clicking the **Create campaign** button. See this [section](create-campaigns.md#create-campaigns).

* The **Templates** tab lists all available campaign templates. You can view an existing template or create a new one. [Read more](#manage-campaign-templates).

![Campaign list](assets/campaign-list.png)

By default, each campaign in the list displays information about its current status, start and end dates, creation date, the last time it was modified, etc.

You can customize the displayed columns by clicking the **Configure column for a custom layout** icon located in the upper-right corner of the list. This allows you to add or remove columns, and reorder information in the campaign list. 

In addition, a search bar and filters are available to facilitate easy searching within the list. [Learn more](../get-started/user-interface.md#list-screens).

For example, you can filter on your campaign schedule. Open the filter panel and use the **Start - End Date** section:

![Campaign filter](assets/campaign-filter-on-dates.png)

## Campaign dashboard {#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="List of deliveries in the campaign"
>abstract="The **Deliveries** tab lists all deliveries linked to the current campaign. Click the name of a delivery to edit it. Use the Create delivery button to add a new delivery for this campaign."

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Workflow list in a campaign"
>abstract="The **Workflow** tab lists all the workflow linked to the current campaign."

In the **Browse** tab of the campaign list, click a campaign name to display its details. 

![Campaign dashboard](assets/campaign-dashboard.png)

The status and schedule of the campaign is displayed at the top of the screen. You can use the **Settings** button to update the properties of your campaign, such as the its label, folder, and description. You can also change the schedule of your campaign from the settings screen. Learn more about campaign schedule in [this section](create-campaigns.md#campaign-schedule).

From the campaign dashboard, use the **Logs** and **Reports** buttons to monitor your campaign. Learn more in this [section](create-campaigns.md#create-campaigns) 

For each campaign, the dashboard shows two main tabs: Workflows and Deliveries. 

* The **Workflows** tab lists all workflows associated to the campaign. This tab also allows you to create a new workflow inside the campaign. See this [section](create-campaigns.md#create-campaigns).

* The **Deliveries** tab lists all deliveries created in the current campaign. You can also create a new delivery inside the campaign. See this [section](create-campaigns.md#create-campaigns).

>[!NOTE]
>
>The **Deliveries** tab displays all deliveries linked to the campaign. However, deliveries created in a workflow cannot be deleted from there. To delete a delivery created in the context of a workflow, you must delete the delivery activity from the workflow. [Learn more](../msg/gs-messages.md#delivery-delete).


## Delete a campaign {#campaign-delete}

You have two ways to delete a campaign:

* from the list of campaigns, click the ellipsis button then select **Delete**

    ![Delete a campaign from the list of campaigns](assets/delete-a-campaign-from-list.png)
    
* from the campaign itself, click the **More** button then select **Delete**

    ![Delete a campaign from the campaign dashboard](assets/delete-a-campaign-from-dashboard.png)


## Duplicate a campaign {#campaign-duplicate}

You have two ways to duplicate a campaign:

* from the list of campaigns, click the ellipsis button then select **Duplicate**
    
* from the campaign itself, click the **More** button then select **Duplicate**

In both cases, confirm the duplication to create the new campaign. The label of the campaign **Copy of `<label of the initial campaign`**. Browse to the campaign settings to update this label.
    

## Work with campaign templates{#manage-campaign-templates}

Campaign templates contain pre-configured settings which can be reused for creating new campaigns. A set of built-in templates is available to help you get started. You can create and configure your campaign templates and then create campaigns from these templates.

A campaign template can store the following information:

* the campaign **Settings**
* the campaign  **Schedule** 
* workflow templates
* delivery templates

To create a campaign template, follow the steps below:

1. Click the **[!UICONTROL Campaigns]** menu, browse to the **Templates** tab, then click the **[!UICONTROL Create template]** button.
1. Select the **Template** to use. This allows you to base your new template on a template previously created. 
1. Provide a label for your template.
1. If needed, you can change the following **Additional options**: internal name, folder, assignee, description and nature.
1. Define the **Schedule** of your campaign. Learn how to set your campaign schedule in [this section](create-campaigns.md#campaign-schedule)
1. Click **Create**.
1. Add workflows and delivery templates to your campaign.
