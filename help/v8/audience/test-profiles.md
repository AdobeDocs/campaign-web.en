---
title: Create test profiles in Campaign
description: Learn how to create and manage test profiles in Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner

---
# Create and manage test profiles {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Create test profiles"
>abstract="Test profiles are created as seed addresses. They are additional recipients in the database used to target fictitious profiles who do not match the defined target criteria."

Test profiles are created as seed addresses. They are additional recipients in the database used to target fictitious profiles who do not match the defined target criteria.

This way, test profiles let you preview and test the personalization and rendering before sending your delivery, by sending them proofs.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

The steps to send test messages to seed addresses are detailed in [this section](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>Test profiles are automatically excluded from reports on the following delivery statistics: **[!UICONTROL Clicks]**, **[!UICONTROL Opens]**, **[!UICONTROL Unsubscriptions]**.

## Create a test profile {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Test profiles Additional Data"
>abstract="Enter the personalization data used for the deliveries created in the Data management workflows and which you want to assign a specific value to."

To create a test profile, follow the steps below.

1. Browse to **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]**.

1. Select the **[!UICONTROL Test profiles]** tab.

    ![](assets/test-profile-list.png)

1. Click the **[!UICONTROL Create test profile]** button.

1. Fill in the test profile details. Most of the fields are the same as when creating profiles. [Learn more]

    ![](assets/test-profile-details.png)

   >[!NOTE]
   >
   >The label of the address is automatically filled in with the last name and first name you defined.<!--Is this note valid?-->
   >
   >You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis.<!--Is this note valid?-->

1. In the **[!UICONTROL Additional data]** tab, enter the personalization data used for the deliveries created in the Data management workflows and which you want to assign a specific value to. 
    
   Make sure that additional target data has been defined with an alias starting with '@' in the **[!UICONTROL Enrichment]** workflow activity. Otherwise, you will not be able to use them properly with your seed addresses in your delivery activity.<!--Is this will be visible in UI for GA?-->

1. Click the **[!UICONTROL Save]** button.

The test profile you just created is now ready to be used to send a test. [Learn more](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

<!--Where can you see touchpoints? seen in mocks-->

<!--Add test audience? Seen in dev ticket-->