---
audience: end-user
title: Use the Split workflow activity
description: Learn how to use the Split workflow activity
exl-id: 4457c70d-bc92-476f-90a3-d51e26ada8f1
---
# Split {#split}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split"
>title="Split activity"
>abstract="The **Split** activity allows you to segment incoming populations into multiple subsets based on different selection criteria, such as filtering rules or population size."

The **Split** activity is a **Targeting** activity that segments incoming populations into multiple subsets based on different selection criteria, such as filtering rules or population size.

## Configure the Split activity {#split-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="Segments for split activity"
>abstract="Add as many subsets as desired to segment the incoming population. When the **Split** activity is executed, the population is segmented across the different subsets in the order they are added to the activity. Before starting your workflow, ensure that you have ordered the subsets in the order that suits your needs using the arrow buttons."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_filter"
>title="Split activity filter"
>abstract="To apply a filtering condition to the subset, click **[!UICONTROL Create filter]** and configure the desired filtering rule using the query modeler. For example, include profiles from the incoming population whose email address exists in the database."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview" text="Work with the query modeler"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_limit"
>title="Split activity limit"
>abstract="To limit the number of profiles selected by the subset, toggle on the **[!UICONTROL Enable limit]** option, and specify the number or percentages of the population to include."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_sorting"
>title="Split activity sorting"
>abstract="When setting a population limit for a subset, you can rank the selected profiles based on a specific profile attribute, in ascending or descending order. To do this, toggle on the **Enable sorting** option. For instance, you can restrict a subset to include only the top 50 profiles with the highest purchase amount."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_complement"
>title="Split generate complement"
>abstract="Once you have configured all the subsets, you can select the remaining population that did not match any of the subsets and include them in an additional outbound transition. To do this, toggle on the **Generate complement** option."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Generate all subsets in the same table"
>abstract="Toggle on this option to group all the subsets into a single output transition."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_emptytransition"
>title="Skip empty transition"
>abstract="Toggle the **[!UICONTROL Skip empty transition]** option on to disable the output transition for this subset if the incoming population is empty."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_enable_overlapping"
>title="Enable overlapping of output populations"
>abstract="The **[!UICONTROL Enable overlapping of output populations]** option lets you manage populations belonging to several subsets. When the box isn't checked, the split activity ensures a recipient cannot be present in several output transitions, even if it meets the criteria of several subsets. They will be in the target of the first tab with matching criteria. When the box is checked, the recipients can be found in several subsets if they meet their filter criteria. Adobe Campaign recommends using exclusive criteria."

Follow these steps to configure the **Split** activity:

1. Add a **Split** activity to your workflow.

1. The activity configuration pane opens with a default subset. Click the **Add segment** button to add as many subsets as desired to segment the incoming population.

    ![Split activity configuration pane showing subsets](../assets/workflow-split.png)

    >[!IMPORTANT]
    >
    >When the **Split** activity is executed, the population is segmented across the different subsets in the order they are added to the activity. For example, if the first subset recovers 70% of the initial population, the next added subset will apply its selection criteria to the remaining 30% only, and so on.
    >
    >Before starting your workflow, ensure that you have ordered the subsets in the order that suits your needs. Use the arrow buttons to change the position of a subset.

1. Once subsets have been added, the activity shows as many output transitions as there are subsets. Change the label of each subset to identify them easily in the workflow canvas.

1. Configure how each subset filters the incoming population. Follow these steps:

    1. Open the subset to display its properties.

    1. To apply a filtering condition to the subset, click **[!UICONTROL Create filter]** and configure the desired filtering rule using the query modeler. For example, include profiles from the incoming population whose email address exists in the database. [Learn how to work with the query modeler](../../query/query-modeler-overview.md).

    1. To limit the number of profiles selected by the subset, toggle on the **[!UICONTROL Enable limit]** option, and specify the number or percentages of the population to include.

    1. To disable a transition if the incoming population is empty, toggle the **[!UICONTROL Skip empty transition]** option on. If no profile matches the subset, the workflow will not transition to the next activity.

        ![Subset configuration pane showing filtering and sorting options](../assets/workflow-split-subset.png)

        >[!NOTE]
        >
        >When setting a population limit for a subset, you can rank the selected profiles based on a specific [profile attribute](../../get-started/attributes.md), in ascending or descending order. To do this, toggle on the **[!UICONTROL Enable sorting]** option. For instance, you can restrict a subset to include only the top 50 profiles with the highest purchase amount.

1. Once you have configured all the subsets, you can select the remaining population that did not match any of the subsets and include them in an additional outbound transition. To do this, toggle on the **[!UICONTROL Generate complement]** option.

    ![Complement transition configuration pane](../assets/workflow-split-complement.png)

    >[!NOTE]
    >
    >The **[!UICONTROL Generate all subsets in the same table]** option allows you to group all the subsets into a single output transition.

1. The **[!UICONTROL Enable overlapping of output populations]** option lets you manage populations belonging to several subsets:

    * When the box isn't checked, the split activity ensures a recipient cannot be present in several output transitions, even if it meets the criteria of several subsets. They will be in the target of the first tab with matching criteria.
    * When the box is checked, the recipients can be found in several subsets if they meet their filter criteria. Adobe Campaign recommends using exclusive criteria.

The activity is now configured. At workflow execution, the population segments into the different subsets in the order they have been added to the activity.

## Example {#split-example}

In the following example, the **[!UICONTROL Split]** activity segments an audience into distinct subsets based on the communication channel to use:

* **Subset 1 "push"**: This subset comprises all profiles who have installed the mobile application.
* **Subset 2 "sms"**: Mobile phone users: For the remaining population that did not fall into Subset 1, Subset 2 applies a filtering rule to select profiles with mobile phones in the database.
* **Complement transition**: This transition captures all the remaining profiles that did not match Subset 1 or Subset 2. Specifically, it includes profiles who neither installed the mobile application nor have a mobile phone, such as users who haven't installed the mobile app or lack a registered mobile number.

![Example of a Split activity with subsets and complement transition](../assets/workflow-split-example.png)