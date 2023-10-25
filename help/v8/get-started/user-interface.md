---
audience: end-user
title: Discover the interface
description: Campaign v8 Web user interface
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Beta" 
---
# Discover the interface {#user-interface}

The new Campaign v8 Web interface offers a modern and intuitive user experience to simplify marketing campaign design and delivery. This new interface is integrated with Adobe Experience Cloud apps and solutions. 


>[!NOTE]
>
>This documentation is frequently updated to reflect latest changes in the product user interface. However, some screenshots can slightly differ from your user interface.


## Left navigation menu {#user-interface-left-nav}

Browse the links on the left to access Campaign v8 Web capabilities. Several links display lists of objects which can be sorted and filtered. You can also configure columns to display all the information you need. See this [section](#list-screens). Some list screens are read-only. The items displayed in the left navigation menu and in the lists depend on your user permissions. Learn more about permissions in [this section](permissions.md).

![](assets/home.png)

### Home {#user-interface-home}

This screen includes key links and resources for a quick access to the main Campaign v8 Web features. 

The **Recents** list provides shortcuts to the recently created and modified deliveries. This list shows their channel, status, owner, creation and modification dates.

The **Key performance indicators** lets you check your platform effectiveness through common KPIs. Learn more about these KPIs in [this page](../reporting/kpis.md).

Access Campaign v8 Web key help pages from the **Learning** section of the home page.

### Explorer {#user-interface-explorer} 

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="The **Explorer** menu displays all Campaign components and objects with the same folder hierarchy as the one in the client console. Browse all your Campaign v8 components, folders and schemas, check associated permissions, and create folders and sub-folders from this menu."

The **Explorer** menu displays all Campaign resources and objects with the same folder hierarchy as the one in the client console. Browse all your Campaign v8 components, folders and schemas, and create deliveries, workflows and campaigns.

The items displayed in the **Explorer** depend on your user permissions. You can also add folders and sub-folders, if you have proper rights. Learn more about permissions in [this section](permissions.md).

You can configure columns to customize the display to view all the information you need. See this [section](#list-screens). You can also add folders and sub-folders, as detailed in [this section](permissions.md#folders).

For more information about the Campaign explorer, folder hierarchy and resources, refer to this [Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html#ac-explorer-ui){target="_blank"}.

### Campaign Management {#user-interface-campaign-management}

In the CAMPAIGN MANAGEMENT section, you can access marketing campaigns, deliveries, and workflows.

* **Campaigns** - This is the list of your campaigns, and campaign templates. By default, for each campaign you can view the start/end/creation/last modification dates, the current status, and the name of the Campaign operator who created it. You can filter the list by status, start/end dates, folder, or create an advanced filter to define your own filtering criteria. Learn more about campaigns [in this section](../campaigns/gs-campaigns.md).

* **Deliveries** - Browse through your list of deliveries. By default, you can view their state, last modification date as well as key KPIs. You can filter the list by status, contact date or channel. Click an email delivery to open its dashboard to get an overview of the delivery details. Deliveries on other channels are read-only. Learn more about deliveries [in this section](../msg/gs-messages.md).

    Use the **More actions** button to delete or duplicate a delivery.

    ![](assets/more-actions.png){width="70%" align="left"}

* **Workflows** - In this screen, you can access the full list of workflows and workflow templates. You can check their status, last/next execution dates, and create a new workflow or a new workflow template. You can filter the list with the same criteria as for other objects. In addition, you can filter workflows which belong to a campaign, or not. Learn more about workflows [in this section](../workflows/gs-workflows.md).


### Customer Management {#user-interface-customer-management}

In the CUSTOMER MANAGEMENT section, you can view your recipients, audiences, and subscriptions. These lists are read-only.

* **Recipients** - Access your recipient database. By default, you can view their email address, first name and last name. Learn more about recipients in [this section](../audience/about-recipients.md).
* **Audiences** - This is your list of audiences. By default, you can view their type, origin, creation/last modification dates and label. You can filter the list by origin. Learn more about audiences and lists in [this section](../audience/about-recipients.md).
* **Subscriptions** - Browse through your subscriptions lists. By default, you can view their type, mode and label. Learn how to manage subscriptions and unsubscriptions in [Adobe Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html){target="_blank"}. 

### Decision Management {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Offers"
>abstract="Browse through the lists of offers and offer templates that have been created in the console using the **Interaction** module. These lists are read-only."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html" text="Add offers to a delivery"

In the DECISION MANAGEMENT section, you can view the offers and offer templates. These lists are read-only.

* **Offers** - Browse through the list of offers and offer templates that have been created in the console using the **Interaction** module. By default, you can view their status, start/end dates and environment. You can filter the list by status and start/end dates. Offer templates are also available.

Learn how to create and send offers in emails and SMS in [this section](../content/offers.md).



## Contextual Help {#user-interface-help} 

A contextual help is available in the interface. When available, click on the `?` icon to display help information and related documentation links. 

![](assets/context-help.png){width="40%" align="left"}

With the new Beta version, the **AI-powered Knowledge Assistant** embedded within contextual help revolutionizes documentation searching and answering how-to questions with effortlessly sifting through vast documentation repositories, instantly pinpointing the precise information you need.

Thanks to Campaign Gen AI's capabilities, this assistant transforms your experience, making information retrieval and problem-solving a breeze. Whether you're seeking guidance in a complex task or navigating extensive documents, our AI-powered Knowledge Assistant is your ultimate companion, providing unmatched efficiency and accuracy in every interaction.

Learn more in [this section](using-ai.md).



## Learn more {#learn-more}

Learn how to browse, search, and filter lists available in your Campaign environment [in this page](list-filters.md).



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Permission required"
>abstract="Your administrator must grant you permission before you can create a segment."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Permission required"
>abstract="Your administrator must grant you permission before you can create a segment."

<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="Global reports sending"
>abstract="Tracking reporting metrics are visible in this screen"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="Global reports tracking"
>abstract="Tracking reporting metrics are visible in this screen"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Workflow list in a campaign"
>abstract="Workflow list in a campaign"

<!-- delivery settings-->






<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->




<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="Recipients creation"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Recipients details"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Recipients contact information"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Recipients adress"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Recipients account"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Recipients custom fields"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Recipients card overview"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Recipients touchpoints"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="Recipients subscriptions list"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="Recipients subscriptions selection"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="Recipients offers eligible list"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="Recipients offers preview"
>abstract="TBC"





>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Subscriptions delivery template"
>abstract="TBC"





>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Landing Pages"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Landing Pages properties"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Landing Pages pages"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Landing Pages schedule"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Landing Pages primary page"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Landing Pages subscription"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Landing Pages call to action"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Landing Pages simulate"
>abstract="TBC"




>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Activity non editable"
>abstract="TBC"




>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Fragments"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Fragments save"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Fragments creation"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Fragments properties"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Fragments type"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Fragments list"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragments details"
>abstract="TBC"




>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Content template"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Content template properties"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Content template design"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Content template selection"
>abstract="TBC"






>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Load file activity"
>abstract="TBC" 






>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Reconciliation activity"
>abstract="TBC" 

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Reconciliation targeting"
>abstract="TBC" 

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Reconciliation rules"
>abstract="TBC" 

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Reconciliation targeting dimension"
>abstract="TBC" 

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Reconciliation select field"
>abstract="TBC" 

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Reconciliation select attribute"
>abstract="TBC" 

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Reconciliation create condition"
>abstract="TBC" 

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Reconciliation generate complement"
>abstract="TBC" 





>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="Conditional content save filter"
>abstract="TBC" 

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="Conditional content select filter"
>abstract="TBC" 

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="Conditional content on subject line"
>abstract="TBC" 

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="Conditional content subjectline condition"
>abstract="TBC" 

