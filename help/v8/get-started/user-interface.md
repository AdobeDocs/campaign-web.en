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

### About link {#user-interface-about}


>[!CONTEXTUALHELP]
>id="acw_about"
>title="About page"
>abstract="The About page provides details about your Adobe Campaign instance"

>[!CONTEXTUALHELP]
>id="acw_about_instance"
>title="About Instance"
>abstract="The Instance section provides key information about your console client, including both the version and the associated build number"

>[!CONTEXTUALHELP]
>id="acw_about_web"
>title="About Web"
>abstract="The Web section displays the version of your Campaign Web user interface, with the last update date of it, if available."

>[!CONTEXTUALHELP]
>id="acw_about_packages"
>title="About Installed Packages"
>abstract="The Installed packages section lists all the modules, features and integrations present on your instance."

At the bottom of the page, the **[!UICONTROL About]** link provides details about your Adobe Campaign instance. those information are in read-only mode.

![](assets/about-link.png){zoomable="yes"}

The **Instance** section provides key information about your console client, including both the **version** and the associated **build** number. 

* The **version** refers to the official release version you are using,
* The **build** refers to a specific iteration of that version.

Both version and build numbers are crucial for troubleshooting, as they help determine exactly what features and fixes are present in your environment.

The **Web** section displays the version of your Campaign Web user interface, with the last update date of it, if available. This helps track changes or improvements made to the Campaign Web user interface.

The **Installed packages** section lists all the modules, features and integrations present on your instance. These packages extend Adobe Campaign's functionality, allowing it to perform specialized tasks such as integrating with other Adobe solutions or enabling specific workflows. Given the large number of packages, you can do a research within this section to quickly check if a particular module is installed on your instance.

![](assets/about.png){zoomable="yes"}

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

* **Fragments** - A fragment is a reusable component that can be referenced in one or more deliveries across campaigns. When modifying a fragment, every content using it is updated. [Learn how to work with fragments](../content/fragments.md)

This functionality allows to prebuild multiple custom content blocks that can be used by marketing users to quickly assemble email contents in an improved design process.

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

### Administration {#left-nav-admin}


* **Audit trail** - The **Audit trail** entry provides users with full visibility into all modifications made to important entities within your instance, typically those that significantly impact a smooth operation of the instance. [Learn more](../reporting/audit-trail.md)

* **External accounts** - Create new external accounts using Web User Interface to meet your specific needs and ensure seamless data transfers. [Learn more](../administration/external-account.md)

* **Schemas** - Custom fields are additional attributes added to the out-of-the-box schemas through the Adobe Campaign console. [Learn more](../administration/custom-fields.md)

* **Delivery Alerting** - Delivery Alerting is an alert management system that enables groups of users to automatically receive email notifications with information on their delivery executions. [Learn more](../msg/delivery-alerting.md)

<!--
## Contextual Help {#user-interface-help} 

A contextual help is available in the interface. When available, click on the `?` icon to display help information and related documentation links. 

![](assets/do-not-localize/context-help.png){zoomable="yes"}{width="40%" align="left"}

Currently released as a Beta version within the new Campaign Web user interface, the **AI-powered Knowledge Assistant** embedded within contextual help revolutionizes documentation searching and answering how-to questions with effortlessly sifting through vast documentation repositories, instantly pinpointing the precise information you need.

Thanks to Campaign Gen AI's capabilities, this assistant transforms your experience, making information retrieval and problem-solving a breeze. Whether you're seeking guidance in a complex task or navigating extensive documents, our AI-powered Knowledge Assistant is your ultimate companion, providing unmatched efficiency and accuracy in every interaction.

Learn more in [this section](using-ai.md).

-->

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

<!-- FOR POST-GA -->

<!--Update file-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata"
>title="Update Data"
>abstract="The **Update data** activity performs a mass update of the fields in the database."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_operationtype"
>title="Select how to update data"
>abstract="The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update (it if it has already been added). You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_recordid"
>title="Record identification"
>abstract="Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or direct use of reconciliation keys."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_fieldsupdate"
>title="Select fields to update"
>abstract="Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_advancedoptions"
>title="Advanced options to update data"
>abstract="The **Advanced options** section let you specify additional settings to manage data and duplicates."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition"
>title="Generate an outbound transition"
>abstract="Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow and therefore the option is not activated by default."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition_rejects"
>title="Generate an outbound transition for rejects."
>abstract="Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example if there is a duplicate). The update generally marks the end of a targeting workflow and therefore the option is not activated by default."

<!-- Workflow settings -->

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_initscript"
>title="Initialization script"
>abstract="Initialization script"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_properties"
>title="Execution properties"
>abstract="Execution properties"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_error"
>title="Execution error"
>abstract="Execution error"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_initscript"
>title="Execution inititialization script"
>abstract="Execution inititialization script"

<!-- Schema edit custom fields -->


>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields"
>title="Edit custom detail"
>abstract="Edit custom detail"

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_separatorproperties"
>title="Separator properties"
>abstract="Separator properties"

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings"
>title="Attribute settings"
>abstract="Attribute settings"

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_general"
>title="General"
>abstract="General"

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_link"
>title="Link properties"
>abstract="LaLink propertiesyout"

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_layout"
>title="Layout"
>abstract="Layout"


<!--Schema-->

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Schema"
>abstract="Schema"

>[!CONTEXTUALHELP]
>id="acw_schema_type"
>title="Schema Types"
>abstract="Schema Types"

>[!CONTEXTUALHELP]
>id="acw_schema_properties"
>title="Schema properties"
>abstract="Schema"

>[!CONTEXTUALHELP]
>id="acw_schema_existing"
>title="Select existing schema"
>abstract="Schema"

>[!CONTEXTUALHELP]
>id="acw_schema_external"
>title="Select external database"
>abstract="Schema"

>[!CONTEXTUALHELP]
>id="acw_schema_add_tables"
>title="Add tables"
>abstract="Schema"

>[!CONTEXTUALHELP]
>id="acw_schema_logs_tasks"
>title="Workflow logs and tasks"
>abstract="Schema"

>[!CONTEXTUALHELP]
>id="acw_schema_update"
>title="Update database"
>abstract="Schema"

>[!CONTEXTUALHELP]
>id="acw_schema_update_script"
>title="Update script"
>abstract="Schema"

>[!CONTEXTUALHELP]
>id="acw_schema_start_update"
>title="Start database update"
>abstract="Schema"



<!-- Target Mapping -->


>[!CONTEXTUALHELP]
>id="acw_targetmapping_properties"
>title="Target Mapping properties"
>abstract="Target Mapping properties"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_mapping"
>title="Target Mapping mapping"
>abstract="Target Mapping mapping"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_denylist"
>title="Target Mapping deny list"
>abstract="Target Mapping deny list"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_storage"
>title="Target Mapping storage"
>abstract="Target Mapping deny storage"

<!-- Favorites & recents -->

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="Favorites & Recents"
>abstract="Favorites & Recents"

<!-- Options -->

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="Options"
>abstract="Options"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="Create option"
>abstract="Create option"

<!-- JavaScript codes -->
 
>[!CONTEXTUALHELP]
>id="acw_javascript_codes_list"
>title="JavaScript codes"
>abstract="JavaScript codes"

>[!CONTEXTUALHELP]
>id="acw_javascript_codes_create"
>title="Create JavaScript code"
>abstract="Create JavaScript code"

<!-- Enumerations -->

>[!CONTEXTUALHELP]
>id="acw_enumerations_list"
>title="Enumerations"
>abstract="Enumerations"

>[!CONTEXTUALHELP]
>id="acw_enumerations_properties"
>title="Properties"
>abstract="Properties"

>[!CONTEXTUALHELP]
>id="acw_enumerations_values"
>title="List of enumeration values"
>abstract="List of enumeration values"
