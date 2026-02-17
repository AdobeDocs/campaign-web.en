---
audience: end-user
title: Get started with campaigns
description: Learn how to start with cross-channel campaigns
exl-id: 690229e7-73e1-4cc1-b69a-f3e5d8de58af
---
# Access and manage your campaigns {#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Campaign schedule"
>abstract="Set or modify your campaign schedule."

To access and manage your campaigns, click the **[!UICONTROL Campaigns]** menu on the left navigation. Two tabs are available:

* The **Browse** tab lists all existing campaigns. You can click a campaign to open its dashboard or create a new campaign by clicking the **Create campaign** button. See this [section](create-campaigns.md#create-campaigns).

* The **Templates** tab lists all available campaign templates. You can view an existing template or create a new one. [Read more](#manage-campaign-templates).

![Description: The campaign list screen showing the Browse and Templates tabs, along with options to create or view campaigns](assets/campaign-list.png)

## Campaigns inventory {#inventory}

The **[!UICONTROL Browse]** tab provides information about the campaigns' current status, start and end dates, creation date, the last time they were modified, etc. You can customize the displayed columns by clicking the **Configure column for a custom layout** icon located in the upper-right corner of the list. This allows you to add or remove columns and reorder information in the campaign list.

### Search & filter the inventory {#search}

A search bar and filters are available to facilitate easy searching within the list. [Learn more](../get-started/user-interface.md#list-screens). For example, you can filter on your campaign schedule. Open the filter panel and use the **Start - End Date** section:

![Description: The filter panel showing options to filter campaigns by start and end dates](assets/campaign-filter-on-dates.png)

### Timeline view {#timeline}

By default, the campaign screen shows the **List view** (inventory). You can switch to **Timeline view** at any time using the view toggle. Both views show the same campaigns and share the same filters and search—when you change filters or search in one view, the other view reflects the same selection.

The Timeline view helps you visualize and manage your campaigns over time. You can see all your campaigns in a time-based format, making it easier to plan, schedule, and coordinate your marketing activities.

![](assets/timeline-view.png)

**How the timeline works:**

* The timeline displays your campaigns according to their start and end dates. Campaigns that span multiple days appear across the relevant dates.
* You can navigate by week, month, or day. Use the date selector or arrow buttons to move between periods. Use the **Today** button to return quickly to the current date.
* Selecting a campaign opens a right-hand panel with campaign details: status, start and end dates, list of workflows, and list of deliveries. You can navigate to those workflows and deliveries from the panel.
* Campaigns in progress are prioritized in the display when many campaigns fall on the same date.
* When many campaigns fall on a single day (for example in month view), a **More** control lets you expand to see the full set for that day, or switch to week or day view for more detail.

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

![Description: The campaign dashboard screen showing the status, schedule, and tabs for workflows and deliveries](assets/campaign-dashboard.png)

The status and schedule of the campaign are displayed at the top of the screen. Use the **Settings** button to update the properties of your campaign, such as its label, folder, and description. You can also change the schedule of your campaign from the settings screen. Learn more about campaign schedule in [this section](create-campaigns.md#campaign-schedule).

From the campaign dashboard, use the **Logs** and **Reports** buttons to monitor your campaign. Learn more in this [section](create-campaigns.md#create-campaigns).

For each campaign, the dashboard shows two main tabs: Workflows and Deliveries.

* The **Workflows** tab lists all workflows associated with the campaign. This tab also allows you to create a new workflow inside the campaign. See this [section](create-campaigns.md#create-campaigns).

* The **Deliveries** tab lists all deliveries created in the current campaign. You can also create a new delivery inside the campaign. See this [section](create-campaigns.md#create-campaigns).

>[!NOTE]
>
>The **Deliveries** tab displays all deliveries linked to the campaign. However, deliveries created in a workflow cannot be deleted from there. To delete a delivery created in the context of a workflow, delete the delivery activity from the workflow. [Learn more](../msg/gs-messages.md#delivery-delete).

## Delete a campaign {#campaign-delete}

You have two ways to delete a campaign:

* From the list of campaigns, click the ellipsis button, then select **Delete**.

    ![Description: The campaign list screen showing the ellipsis button and the Delete option](assets/delete-a-campaign-from-list.png)

* From the campaign itself, click the **More** button, then select **Delete**.

    ![Description: The campaign dashboard screen showing the More button and the Delete option](assets/delete-a-campaign-from-dashboard.png)

## Duplicate a campaign {#campaign-duplicate}

You have two ways to duplicate a campaign:

* From the list of campaigns, click the ellipsis button, then select **Duplicate**.

* From the campaign itself, click the **More** button, then select **Duplicate**.

In both cases, confirm the duplication to create the new campaign. The label of the campaign is **Copy of `<label of the initial campaign>`**. Browse to the campaign settings to update this label.

## Work with campaign templates {#manage-campaign-templates}

Campaign templates contain pre-configured settings that can be reused for creating new campaigns. A set of built-in templates is available to help you get started. You can create and configure your campaign templates and then create campaigns from these templates.

A campaign template can store the following information:

* The campaign **Settings**
* The campaign **Schedule**
* Workflow templates
* Delivery templates

To create a campaign template, follow the steps below:

1. Click the **[!UICONTROL Campaigns]** menu, browse to the **Templates** tab, then click the **[!UICONTROL Create template]** button.
1. Select the **Template** to use. This allows you to base your new template on a template previously created.
1. Provide a label for your template.
1. If needed, change the following **Additional options**: internal name, folder, assignee, description, and nature.
1. Define the **Schedule** of your campaign. Learn how to set your campaign schedule in [this section](create-campaigns.md#campaign-schedule).
1. Click **Create**.
1. Add workflows and delivery templates to your campaign.
