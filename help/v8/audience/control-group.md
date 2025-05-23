---
audience: end-user
title: Set a control group
description: Learn how to set a control group for your messages in Campaign Web user interface
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
---
# Set a control group {#control-group}

A control group is a sub-population excluded from the delivery. You can define a control group to avoid sending messages to a portion of your audience and compare post-delivery behavior with the main target. This option helps measure the impact of your campaign.

➡️ [Discover this feature in video](create-audience.md#video)

## Enable control group {#add-a-control-group}

To add a control group, enable the option when defining the audience of your delivery. The control group can be extracted randomly from the main target or selected from a specific population. Consequently, there are two main ways to define a control group:

* Extract a number of profiles from the main target.
* Exclude some profiles from a list or based on criteria defined in a query.

You can combine both methods when defining a control group.

All profiles included in the control group at the delivery preparation step are removed from the main target. They do not receive the message.

>[!CAUTION]
>
>You cannot use control groups when loading the target population [from an external file](file-audience.md).

To add a control group to a delivery, activate the **[!UICONTROL Enable control group]** toggle from the **Audience** section of the delivery creation screen.

![Enable control group option toggle on the delivery creation screen](assets/control-group1.png)

## Extract from target {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extraction mode"
>abstract="A control group is a set of profiles excluded from the delivery. To define a control group, you can choose to extract, randomly or based on a sorting, a percentage or a fixed number of profiles from the target population."

### Build a control group {#build-extract-target}

To define a control group, choose to extract, randomly or based on a sorting, a percentage or a fixed number of profiles from the target population. If adding an extra population, choose the **No extraction** option and select the extra population [as detailed here](#extra-population).

First, define how the profiles are extracted from the target: randomly or based on a sorting.

Under the **Control group** section, choose an **Extraction mode**:

* **Random**: When preparing the delivery, Adobe Campaign randomly extracts a number of profiles corresponding to the percentage or the maximum number set as the size limit.
* **Ranked by attribute(s)**: This option excludes a set of profiles based on specific attributes in a specific sorting order.

Then, use the **Size limit** section to set the number of profiles to extract from the main target. It can be a raw number (for example, 50 profiles to exclude) or a percentage of your initial audience (for example, 5% of the main target).

### Sample of control group {#control-group-sample}

For example, to create a control group with the 100 youngest profiles, follow these steps:

1. Select the **Age** field as a sorting criterion. Leave the **Ascending** sort option. 
1. Add the **Creation Date** field. Change to the **Descending** sort option.
1. Define 100 as the threshold in the **Size limit** section.

    ![Control group configuration for youngest profiles](assets/control-group2.png){zoomable="yes"}

These 100 youngest profiles are then excluded from the main target. 

### Check your control group {#check-control-group}

View the logs to check and identify the excluded profiles. For example, consider a random exclusion of five profiles.

![Example of excluded profiles in logs](assets/control-group4.png){zoomable="yes"}

After the delivery preparation, review how the exclusions were applied:

* In the delivery dashboard, before sending, check the **To exclude** KPI.

    ![Delivery dashboard showing the "To exclude" KPI](assets/control-group5.png){zoomable="yes"}

* In the delivery logs, the Logs tab shows the exclusion step.

    ![Delivery logs showing exclusion step](assets/control-group-sample-logs.png){zoomable="yes"}

<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}

-->

* The **Exclusion causes** tab displays the number of excluded profiles for each typology rule.

    ![Exclusion causes tab showing typology rule exclusions](assets/control-group7.png){zoomable="yes"}

For more information on delivery logs, refer to this [section](../monitor/delivery-logs.md).

## Add an extra population {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Extra population"
>abstract="A control group is a set of profiles excluded from the delivery. You can exclude a specific population from the delivery audience by selecting an existing audience, or by defining a query."

Another way to define a control group is to select a specific population in an existing audience or define a query.

From the **Extra population** section of the **Control Group** definition screen, click the **[!UICONTROL Select Audience]** button.

![Extra population selection screen](assets/control-group3.png){zoomable="yes"}

* To use an existing audience, click **Select audience**. Learn more in [this section](add-audience.md). 
* To define a new query, select **Create your own** and define the exclusion criteria using the query modeler. Learn more in [this section](../query/query-modeler-overview.md). 

The profiles included in the audience or matching the result of the query are **excluded** from the delivery target. They do not receive any message.

## Compare the results {#control-group-results}

Once the delivery is sent, extract the sending logs to compare behavior between the profiles that did not receive the communication and the effective target. Use the delivery logs to build a new targeting.

To see which profiles were removed from the target, check the **Delivery logs**. Learn more [in this section](#check-control-group).