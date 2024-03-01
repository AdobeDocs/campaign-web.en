---
audience: end-user
title: Discover the interface
description: Adobe Campaign Web user interface
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
---
# Discover the interface {#user-interface}

The new Adobe Campaign Web interface offers a modern and intuitive user experience to simplify marketing campaign design and delivery. This new interface is integrated with Adobe Experience Cloud apps and solutions. 

Learn how to connect to Adobe Campaign and discover Experience Cloud navigation basics [in this article](connect-to-campaign.md).


>[!NOTE]
>
>This documentation is frequently updated to reflect latest changes in the product user interface. However, some screenshots can slightly differ from your user interface.

## Campaign home page {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Recents"
>abstract="The **Recents** list provides shortcuts to the recently created and modified deliveries. This list shows their channel, status, owner, creation and modification dates."

Campaign home page lets you quickly and easily browse key resources, indicators, and components. 

The upper section of the home page provides details about latest updates and new capabilities available in the product, with link to Release Notes and detailed documentation. Use the left arrow to scroll feature cards. 

![](assets/home.png){zoomable="yes"}

The **Key performance indicators** lets you check your platform effectiveness through common KPIs. Learn more about these KPIs in [this page](../reporting/kpis.md).

The **Recents** list provides shortcuts to the recently created and modified deliveries. This list shows their channel, status, owner, creation and modification dates. Click the **Show more** link to load more deliveries.

In addition, you can access Adobe Campaign Web key help pages from the **Learning** section of the page.

## Left navigation menu {#user-interface-left-nav}

Browse the links on the left to access Adobe Campaign Web capabilities. Several links display lists of objects which can be sorted and filtered. You can also configure columns to display all the information you need. See this [section](#list-screens). Some list screens are read-only. The items displayed in the left navigation menu and in the lists depend on your user permissions. Learn more about permissions in [this section](permissions.md).


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

    ![](assets/more-actions.png){zoomable="yes"}{width="70%" align="left"}

* **Workflows** - In this screen, you can access the full list of workflows and workflow templates. You can check their status, last/next execution dates, and create a new workflow or a new workflow template. You can filter the list with the same criteria as for other objects. In addition, you can filter workflows which belong to a campaign, or not. Learn more about workflows [in this section](../workflows/gs-workflows.md).


### Content Management {#user-interface-content-management}

In the CONTENT MANAGEMENT section, you can view your content templates and fragments.

* **Content templates** - For an accelerated and improved design process, you can create standalone templates to easily reuse custom content across [!DNL Adobe Campaign]. Only available for emails, this functionality enables content-oriented users to work on standalone templates so that marketing users can reuse and adapt them inside their own email campaigns. Learn more in [this section](../email/create-email-templates.md).

<!--
* **Fragments** -
-->

### Customer Management {#user-interface-customer-management}

In the CUSTOMER MANAGEMENT section, you can view your profiles, audiences, and subscriptions. These lists are read-only.

* **Profiles** - Create and manage profiles, and access your recipient database. By default, you can view their email address, first name and last name. Learn more about profiles in [this section](../audience/about-recipients.md).
* **Audiences** - This is your list of audiences. By default, you can view their type, origin, creation/last modification dates and label. You can filter the list by origin. Learn more about audiences and lists in [this section](../audience/about-recipients.md).
* **Subscription services** - Browse through your subscriptions lists. By default, you can view their type, mode and label. Learn how to manage subscriptions and unsubscriptions in [Adobe Campaign v8 (console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html){target="_blank"}. 
* **Predefined filters** - Predefined filters are custom filters which are created and saved to be available for future use. They can be used as shortcuts during any filtering operations with the query modeler, for example when filtering a list of data, or creating the audience of a delivery. Learn more in [this section](predefined-filters.md).


### Decision Management {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Offers"
>abstract="Browse through the lists of offers and offer templates that have been created in the console using the **Interaction** module. These lists are read-only."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html" text="Add offers to a delivery"

In the DECISION MANAGEMENT section, you can view the offers and offer templates. These lists are read-only.

* **Offers** - Browse through the list of offers and offer templates that have been created in the console using the **Interaction** module. By default, you can view their status, start/end dates and environment. You can filter the list by status and start/end dates. Offer templates are also available.

Learn how to create and send offers in emails and SMS in [this section](../msg/offers.md).

### Reporting {#left-nav-reporting}

* **Reports** - The **Report** entry offers a consolidated overall summary of traffic and engagement metrics for each channel within your Campaign environment. These reports consist of various widgets, each offering a distinct perspective on your campaign or delivery performance. Learn more in [this section](../reporting/global-reports.md).


## Contextual Help {#user-interface-help} 

A contextual help is available in the interface. When available, click on the `?` icon to display help information and related documentation links. 

![](assets/do-not-localize/context-help.png){zoomable="yes"}{width="40%" align="left"}

Currently released as a Beta version within the new Campaign Web user interface, the **AI-powered Knowledge Assistant** embedded within contextual help revolutionizes documentation searching and answering how-to questions with effortlessly sifting through vast documentation repositories, instantly pinpointing the precise information you need.

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

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="Global reports sending"
>abstract="Tracking reporting metrics are visible in this screen"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="Global reports tracking"
>abstract="Tracking reporting metrics are visible in this screen"


<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->


<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="Recipients creation"
>abstract="Recipients creation"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Recipients card overview"
>abstract="Recipients card overview"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Recipients touchpoints"
>abstract="Recipients touchpoints"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="Recipients subscriptions selection"
>abstract="Recipients subscriptions selection"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="Recipients offers eligible list"
>abstract="Recipients offers eligible list"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="Recipients offers preview"
>abstract="Recipients offers preview"

>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Fragments"
>abstract="Fragments"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Fragments save"
>abstract="Fragments save"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Fragments creation"
>abstract="Fragments creation"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Fragments properties"
>abstract="Fragments properties"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Fragments type"
>abstract="Fragments type"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Fragments list"
>abstract="Fragments list"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragments details"
>abstract="Fragments details"




>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="Conditional content save filter"
>abstract="Conditional content save filter" 

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="Conditional content select filter"
>abstract="Conditional content select filter" 

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="Conditional content on subject line"
>abstract="Conditional content on subject line" 

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="Conditional content subjectline condition"
>abstract="Conditional content subjectline condition" 


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="Simulate test profiles"
>abstract="Simulate test profiles"
<!--ML: not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="Simulate test profiles selection"
>abstract="Simulate test profiles selection"
<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="Simulate test profiles sending"
>abstract="Simulate test profiles sending"
<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="Simulate email log"
>abstract="Simulate email log"
<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Content for Direct Mail"
>abstract="Content for Direct Mail"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="File properties for Direct Mail"
>abstract="File properties for Direct Mail"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Content properties for Direct Mail"
>abstract="Content properties for Direct Mail"

<!-- FOR POST-GA -->



<!--
Deprecated IDs - to remove in GA: -->

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Display advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Rule builder advanced fields"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Rule builder advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."



>[!CONTEXTUALHELP]
>id="acw_contenttemplate_readonlymode"
>title="This template is ready only"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Generate all subsets in the same table"
>abstract="TBC"
<!-- ML: not found in wiki pages-->


<!-- Subscription activity-->

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="Default Landing Pages"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Subscription services"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Subscription services parameters"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Subscription services outbound transition"
>abstract="TBC"


<!--Update file-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata"
>title="Update Data"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_operationtype"
>title="Update Data"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_recordid"
>title="Update Data"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_fieldsupdate"
>title="Update Data"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_advancedoptions"
>title="Update Data"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition"
>title="Update Data"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition_rejects"
>title="Update Data"
>abstract="TBC"

