---
title: Manage target mappings
description: Learn how to manage target mappings.
---
# Manage target mappings {#target-mappings}

>[!CONTEXTUALHELP]
>id="acw_targetmapping_list"
>title="Target mappings "
>abstract="Target mappings"

## About target mappings {#about}

Each communication channel uses a default target mapping to target their recipients. For example, by default, email and SMS delivery templates target **[!UICONTROL Recipients]**. Their target mapping therefore uses the fields of the **nms:recipient** table. For Push notifications, the default target mapping is **Subscriber applications (nms:appSubscriptionRcp)**, which is linked to the recipients table. 

Target mappings are accessible from the **[!UICONTROL Administration]** > **[!UICONTROL Target mappings]** menu. From this screen, you can access details on each target mapping, or create new target mappings to suit your needs.

![](assets/target-mappings-list.png)

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

To create a new target mapping, access the **[!UICONTROL Administration]** > **[!UICONTROL Target mappings]** menu. Click the **[!UICONTROL Create mapping]** button then follow the steps detailed in the sections below.

1. In the **[!UICONTROL Properties]** section, enter a **[!UICONTROL Label]** for the target mapping.

1. Expand the **[!UICONTROL Additional options]** section to define advanced settings such as the target mapping's internal name, storage folder, and description.

1. Select the target population. You can either:

    * **[!UICONTROL Use the targeting dimension directly]**: Select the dimension to target directly from the list of available dimensions.
    * **[!UICONTROL Use linked data]**: This option allows you to start from a targeting dimension (for example subscriptions), and then switch to the targeting dimension that you want to target (for example recipients). 

    ![](assets/target-mappings-properties.png)

1. If the selected dimension is not already used by an existing target mapping, the schemas to store the logs need to be created. To do this, additional options are avaible in the **[!UICONTROL Storage]** section. Expand the section below for more details. 

    +++Storage options for new targeting dimensions

    1. **[!UICONTROL Namespace]**: Identify the namespace that will be used to create the logs. 
    1. **[!UICONTROL Suffix of the extension schema]**: Provide a suffix for the new schema. 

        In the example below, the broadlog name will be "cusbroadlogSupplier".

        ![](assets/target-mappings-new.png)

    1. **[!UICONTROL Delivery logs]**: Activate the options in this section to enrich the sending logs with a segment code field or with a field containing the delivery IP address. For example you can save a segment code calculated during the workflow into the sending logs in order to refine the target later on. This will allow you to target profiles having this specific segment code.

    1. **[!UICONTROL Exclusions]**: Specify how you want to store the exclusions logs.

    1. **[!UICONTROL Tracking logs]**: Activate the **[!UICONTROL Generate a schema for tracking]** option to generate a storage schema for tracking logs

    +++

1. Use the **[!UICONTROL Mapping]** section to identify which attributes from the target mapping's schema to use for each delivery address fields. For each field, select the desired attribute to map. You can also build an expression to identify the field. For example, you can apply a lower function to the address attribute.

    ![](assets/target-mappings-mapping.png)

1. When your target mapping is ready, click the **[!UICONTROL Create]** button. The systems automatically creates the target mapping and all the related schemas for the logs.

Once your target mapping has been created, two additional sections display in the screen:

* **[!UICONTROL Denylisting]**: This section allows you to identify the attributes from the target mapping's schema to use for denylists.

    ![](assets/target-mappings-denylisting.png)

* **[!UICONTROL Storage]**: This section allows you to identify the tables to use to store logs.

    ![](assets/target-mappings-storage.png)

    * **[!UICONTROL Message schema]**:  Identifies the schema to use to store the sending logs.
    * **[!UICONTROL Messages excluded]**: This section specifies how to manage delivery and exclusion logs storage.

        * **[!UICONTROL Store exclusions and messages in the same table]**
        * **[!UICONTROL Store messages only]**: Do not store exclusions.
        * **[!UICONTROL Store exclusions and messages in separate tables]**: Select the schema to use to store exclusion logs in the **[!UICONTROL Rejection schema]** field.

    * **[!UICONTROL Tracking logs]**: Choose where to store tracking logs and the default traffic source.
    * **[!UICONTROL Additional fields]**: This section allows you to specify a list of additional fields to store into  the delivery logs. These fields can permanently store information on individual members of the target (eg. `recipient/@firstName`) or store additional data calculated during the workflow (eg. `[targetData/@offeCode]`)

        To do this, select **[!UICONTROL Add field]**. Identify the information you want to save in the **[!UICONTROL Source]** field, and the attribute to use in the sending logs to save this information in the **[!UICONTROL Destination]** field.

        ![](assets/target-mappings-additional.png){width="50%" zoomable="yes"}
