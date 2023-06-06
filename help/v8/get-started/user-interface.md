---
audience: end-user
title: Discover the interface
description: Campaign v8 Web user interface
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alpha" type="Positive"
---
# Discover the interface {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Discover the interface"
>abstract="The new Campaign v8 Web interface offers an integrated, intuitive and consistent user experience."

The new Campaign v8 Web interface offers a modern and intuitive user experience to simplify marketing campaign design and delivery. This new interface is integrated with Adobe Experience Platform. 

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>This documentation is frequently updated to reflect latest changes in the product user interface. However, some screenshots can slightly differ from your user interface.


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## Left navigation menu

Browse the links on the left to access Campaign v8 Web capabilities. Several links display lists of objects which can be sorted and filtered. You can also configure columns to display all the information you need. See this [section](#list-screens). All list screens are read-only, except the email delivery list. Clicking on any list item for edition/viewing is not available in Alpha. All lists will be editable in future versions. The items displayed in the left navigation menu depend on your user permissions.

![](assets/home.png)

### Home

This screen includes key links and resources for a quick access to the main Campaign v8 Web features. The **Recents** list provides shortcuts to the recently created and modified deliveries. This list shows their creation and modification dates and status.

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

Access Campaign v8 Web key help pages from the lower section of the home page.

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### Explorer

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="The **Explorer** menu displays the same folder hierarchy as the one in the client console. Browse all your Campaign v8 components, folders and schemas. All list screens are read-only, except the email delivery list."

The **Explorer** menu displays the same folder hierarchy as the one in the client console. Browse all your Campaign v8 components, folders and schemas. 

The items displayed in the Explorer depend on your user permissions. 

Like in any list screen, you can configure columns to personalize the display to view all the information you need. See this [section](#list-screens).

For more information on the Campaign explorer, refer to this [documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/ac-ui/campaign-ui.html#ac-explorer-ui){target="_blank"}.
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Campaign Management

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Campaigns"
>abstract="This is the list of your campaigns. You can view useful information such as their start/end/last modification dates, as well as their status. You can filter the list by status or start/end dates. Click the 'Create campaign' button to add a new campaign. Select a campaign to view its content, deliveries, and details. Browse to the 'Templates' tab to view and create templates."

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Deliveries"
>abstract="Browse through your list of deliveries. You can view their status, contact and modification dates, key KPIs. You can filter the list by state, contact date or channel. Click the 'Create delivery' button to add a new delivery. Select a delivery to view its content, audience, and details."

In the CAMPAIGN MANAGEMENT section, you can access marketing campaigns, deliveries and workflows.

* **Campaigns** - This is the list of your campaigns, and campaign templates. By default, for each campaign you can view the start/end/creation/last modification dates, the current status, and the name of the Campaign operator who created it. You can filter the list by status, start/end dates, folder, or create an advanced filter to define your own filtering criteria. Learn more about campaigns [in this section](../campaigns/gs-campaigns.md).

* **Deliveries** - Browse through your list of deliveries. By default, you can view their state, last modification date as well as key KPIs. You can filter the list by state, contact date or channel. Click an email delivery to open its dashboard to get an overview of the delivery details. Deliveries on other channels are read-only. Learn more about deliveries [in this section](../msg/gs-messages.md).

    Use the **More actions** button to delete or duplicate a delivery.

    ![](assets/more-actions.png){width="70%" align="left"}

* **Workflows** - In this screen, you can access the full list of workflows and workflow templates. You can check their status, last/next execution dates, and create a new workflow or a new workflow template. You can filter the list with the same criteria as for other objects. In addition, you can filter workflows which belong to a campaign, or not. Learn more about workflows [in this section](../workflows/gs-workflows.md).


### Customer Management

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Recipients"
>abstract="Access your recipient database. You can view useful information such as their email address, first name and last name. This list is read-only."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="This is your list of audiences. You can view their type, origin, creation/last modification dates and label. You can filter the list by origin. This list is read-only."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Subscriptions lists"
>abstract="Browse through your subscriptions lists. You can view their type, mode and label. This list is read-only."

* **Recipients** - Access your recipient database. By default, you can view their email address, first name and last name. This list is read-only. 
* **Audiences** - This is your list of audiences. By default, you can view their type, origin, creation/last modification dates and label. You can filter the list by origin. This list is read-only. 
* **Subscriptions lists** - Browse through your subscriptions lists. By default, you can view their type, mode and label. This list is read-only. 

### Decision Management

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Offers"
>abstract="Browse through your list of Interaction offers. By default, you can view their status, start/end dates and environment. You can filter the list by state and start/end dates. Offer templates are also available. These lists are read-only."

* **Offers** - Browse through your list of Interaction offers. By default, you can view their status, start/end dates and environment. You can filter the list by state and start/end dates. Offer templates are also available. These lists are read-only. 

## Top bar

The top bar of the interface allows you to:

* share your feedback as an Alpha tester
* switch between organizations and instances
* switch between your Adobe Experience Cloud applications
* access help pages, contact support and share feedback. You can search help articles and videos from the search field.

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Configure list screens {#list-screens}

Several links from the left navigation menu, for example **Deliveries** or **Campaigns**, display lists of objects. These list screens are read-only, except the email delivery list. 

To find items quicker, you can use the search bar or filter the list based on contextual criteria. 

![](assets/filter.png){width="70%" align="left"}

The lists are displayed in columns. You can display additional information by changing the column configuration. To do this, click the icon in the top right corner of the list. You can add or remove columns and change the order in which they are displayed.

![](assets/columns.png){width="70%" align="left"}

You can sort items in the list by clicking any column header. An arrow is displayed (Up or Down) indicating that the list is sorted on that column. For numeric or date columns, the Up arrow indicates that the list is sorted in ascending order while the Down arrow indicates a descending order. For string or alphanumeric columns, values are listed in alphabetical order.

## Contextual help and on-boarding guide

A contextual help is available in the interface. When available, click on the **?** icon to display help information and related documentation links. 

![](assets/context-help.png){width="70%" align="left"}

An on-boarding guide is also available to help you get started with Campaign v8 Web. Click the icon in the bottom right corner, choose one of the available step-by-step scenarios, and simply follow the instructions.

![](assets/onboarding.png){width="70%" align="left"}

## Supported browsers {#browsers}

Campaign v8 Web is designed to work optimally in the latest version of Google Chrome, Safari and Microsoft Edge. You might have trouble using certain features on older versions or other browsers.

## Language preferences {#language-pref}

Campaign v8 Web is currently available in the following languages:

<table>
<tr>
<td>
<p>English (US) - EN-US</p>
<p>French - FR</p>
<p>German - DE</p>
<p>Italian - IT</p>
</td>
<td>
<p>Spanish - ES</p>
<p>Portuguese (Brazilian) - PTBR</p>
<p>Japanese - JP</p>
</td>
<td>
<p>Korean - KR</p>
<p>Simplified Chinese - CHS</p>
<p>Traditional Chinese - CHT</p>
</td>
</tr>
</table>

Your default interface language is determined by the preferred language specified in your user profile.

To change your language:

1. Click on your profile icon, on the top right, then select **Preferences**.

    ![](assets/preferences.png){width="70%" align="left"}

1. Then click the language displayed under your email address.

    ![](assets/preferences2.png)

1. Select your preferred language and click **Save**. You can select a second language in case the component you are using is not localized in your first language.

    ![](assets/select-language.png)

<!--
## Supported browsers {#browsers}

Adobe Campaign interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Rule Builder Advanced attributes"
>abstract="Use an advanced attributes to define your rule."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Sent Metrics"
>abstract="Number of email delivered."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Errors Metrics"
>abstract="Number of emails with the error status."

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Test population"
>abstract="Select a test population mode."

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Preview mode"
>abstract="Preview and test the message by including the test population to the main target."

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Enrichment data"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personalization"
>abstract="TBD"


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="Reporting Sending"
>abstract="Consult the sending indicators for the campaign reporting."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="Reporting tracking"
>abstract="Consult the tracking indicators for the campaign reporting."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Reporting overview"
>abstract="Key metrics for your delivery."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Reporting target statistics"
>abstract="This section displays specific metrics according to audiences."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="Aggregated reporting for deliveries"
>abstract="Select at least two deliveries for displaying an aggregated data report."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Deduplication fields"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Deduplication settings"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Deduplication complement"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Dimension complement"
>abstract="TBD"

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Permission required"
>abstract="Your administrator must grant you permission before you can create a segment."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Permission required"
>abstract="Your administrator must grant you permission before you can create a segment."

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Attribute picker advanced fields"
>abstract="Configure columns with advanced fields."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Rule builder advanced fields"
>abstract="Configure columns with advanced fields."



>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="New quarantines metric"
>abstract="New quarantine metric."


>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Delivered"
>abstract="Delivered KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Opens"
>abstract="Opens KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Clicks"
>abstract="Clicks KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Unsubscriptions"
>abstract="Unsubscriptions KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="Spam KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Errors"
>abstract="Errors KPI"
