---
title: Manage target mappings
description: Learn how to manage target mappings.
exl-id: 144d5650-9632-4af3-b64e-f6e81503a621
---
# Manage target mappings {#target-mappings}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Target Mappings"
>abstract="You can now create target mappings in Campaign Web User Interface. Target mappings define how different delivery channels (email, SMS, push notifications) link to the data fields of a schema."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_list"
>title="Target mappings "
>abstract="Target mappings"

## About target mappings {#about}

Each communication channel uses a default target mapping to target their recipients. For example, by default, email and SMS delivery templates target **[!UICONTROL Recipients]**. Their target mapping therefore uses the fields of the **nms:recipient** table. For Push notifications, the default target mapping is **Subscriber applications (nms:appSubscriptionRcp)**, which is linked to the recipients table.

Target mappings are accessible from the **[!UICONTROL Administration]** > **[!UICONTROL Target mappings]** menu. From this screen, you can access details on each target mapping or create new target mappings to suit your needs.

![Target mappings list screen showing available mappings](assets/target-mappings-list.png)

For more information on the built-in target mappings provided with Adobe Campaign, refer to the [Campaign v8 Client console documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## Create a target mapping {#create-mapping}

>[!CONTEXTUALHELP]
>id="acw_targetmapping_properties"
>title="Target Mapping properties"
>abstract="The **[!UICONTROL Properties]** section allows you to define generic settings for the target mapping and the targeted population."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_mapping"
>title="Target Mapping mapping"
>abstract="The **[!UICONTROL Mapping]** section allows you to identify which attributes from the target mapping's schema to use for the various delivery address fields."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_denylist"
>title="Target Mapping deny list"
>abstract="Target Mapping deny list"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_storage"
>title="Target Mapping storage"
>abstract="The **[!UICONTROL Storage]** section allows you to identify where logs must be stored."

To create a new target mapping, access the **[!UICONTROL Administration]** > **[!UICONTROL Target mappings]** menu. Click the **[!UICONTROL Create mapping]** button, then follow the steps detailed in the sections below.

1. In the **[!UICONTROL Properties]** section, enter a **[!UICONTROL Label]** for the target mapping.

1. Expand the **[!UICONTROL Additional options]** section to define advanced settings such as the target mapping's internal name, storage folder, and description.

1. Select the target population. You can either:

    * **[!UICONTROL Use the targeting dimension directly]**: Select the dimension to target directly from the list of available dimensions.
    * **[!UICONTROL Use linked data]**: Start from a targeting dimension (for example subscriptions), and then switch to the targeting dimension that you want to target (for example recipients).

    ![Target mappings properties screen showing population options](assets/target-mappings-properties.png)

1. If the selected dimension is not already used by an existing target mapping, schemas to store the logs need to be created. Additional options are available in the **[!UICONTROL Storage]** section. Expand the section below for more details.

    +++Storage options for new targeting dimensions

    1. **[!UICONTROL Namespace]**: Identify the namespace that will be used to create the logs.
    1. **[!UICONTROL Suffix of the extension schema]**: Provide a suffix for the new schema.

        In the example below, the broadlog name will be "cusbroadlogSupplier."

        ![Example of storage options for new targeting dimensions](assets/target-mappings-new.png)

    1. **[!UICONTROL Delivery logs]**: Activate the options in this section to enrich the sending logs with a segment code field or a field containing the delivery IP address. For example, save a segment code calculated during the workflow into the sending logs to refine the target later on. This allows targeting profiles with this specific segment code.

    1. **[!UICONTROL Exclusions]**: Specify how to store the exclusions logs.

    1. **[!UICONTROL Tracking logs]**: Activate the **[!UICONTROL Generate a schema for tracking]** option to generate a storage schema for tracking logs.

    +++

1. Use the **[!UICONTROL Mapping]** section to identify which attributes from the target mapping's schema to use for each delivery address field. For each field, select the desired attribute to map. You can also build an expression to identify the field. For example, apply a lower function to the address attribute.

    ![Mapping section showing attribute selection for delivery address fields](assets/target-mappings-mapping.png)

1. When your target mapping is ready, click the **[!UICONTROL Create]** button. The system automatically creates the target mapping and all related schemas for the logs.

Once your target mapping has been created, two additional sections display on the screen:

* **[!UICONTROL Denylisting]**: This section allows you to identify the attributes from the target mapping's schema to use for denylists.

    ![Denylisting section showing attribute selection](assets/target-mappings-denylisting.png)

* **[!UICONTROL Storage]**: This section allows you to identify the tables to use to store logs.

    ![Storage section showing table options for logs](assets/target-mappings-storage.png)

    * **[!UICONTROL Message schema]**: Identifies the schema to use to store the sending logs.
    * **[!UICONTROL Messages excluded]**: Specifies how to manage delivery and exclusion logs storage.

        * **[!UICONTROL Store exclusions and messages in the same table]**
        * **[!UICONTROL Store messages only]**: Do not store exclusions.
        * **[!UICONTROL Store exclusions and messages in separate tables]**: Select the schema to use to store exclusion logs in the **[!UICONTROL Rejection schema]** field.

    * **[!UICONTROL Tracking logs]**: Choose where to store tracking logs and the default traffic source.
    * **[!UICONTROL Additional fields]**: Specify a list of additional fields to store in the delivery logs. These fields can permanently store information on individual members of the target (e.g., `recipient/@firstName`) or store additional data calculated during the workflow (e.g., `[targetData/@offeCode]`).

        To do this, select **[!UICONTROL Add field]**. Identify the information to save in the **[!UICONTROL Source]** field, and the attribute to use in the sending logs to save this information in the **[!UICONTROL Destination]** field.

        ![Additional fields section showing options for storing extra data](assets/target-mappings-additional.png){width="50%" zoomable="yes"}