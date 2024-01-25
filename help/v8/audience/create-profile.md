---
title: Create a profile
description: Learn how to create a profile in Campaign Web.
badge: label="Limited Availability"
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
---
# Create a profile {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Basic details"
>abstract="This section offers insights into the basic details of the profile. To modify any information, make your changes directly within the respective field and click the **Save** button located in the upper-right corner of the screen."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Contact information"
>abstract="This section offers insights into the profile's contact information. To modify any information, make your changes directly within the respective field and click the **Save** button located in the upper-right corner of the screen."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Address"
>abstract="This section offers insights into the profile's postal address and the address quality. To modify any information, make your changes directly within the respective field and click the **Save** button located in the upper-right corner of the screen."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Account details"
>abstract="This section offers insights into the account details of the profile. To modify any information, make your changes directly within the respective field and click the **Save** button located in the upper-right corner of the screen."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Recipients No longer contact"
>abstract="This section offers insights into the contact preferences of the profile. To modify any information, make your changes directly within the respective field and click the **Save** button located in the upper-right corner of the screen."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Custom fields"
>abstract="Custom fields are specific attributes tailored to your needs that have been configured for your instance. To modify any information, make your changes directly within the respective field and click the **Save** button located in the upper-right corner of the screen."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Others"
>abstract="This section provides additional built-in attributes. To modify any information, make your changes directly within the respective field and click the **Save** button located in the upper-right corner of the screen."

To create a profile, follow these steps:

1. Navigate to **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]** and click the **[!UICONTROL Create profile]** button in the upper-right corner of the screen.

1. The list of attributes available for the profile display, organized into different sections detailed in the table below.

    ![](assets/create-profile.png)

    |Attributes section|Description|
    |  ---  |  ---  |
    |**Basic details**|Basic information on the profile, such as the name or date of birth.<br/>By default, profiles are stored in the **[!UICONTROL Recipients]** folder. You can change it by browsing to the desired location. [Learn how to work with folders](../get-started/permissions.md#folders)|
    |**Contact information**|The profile's contact information such as the email address or phone number.|
    |**Address**|The profile's postal address. This section also provides an evaluation of the address quality. A profile's address is considered valid if the 'Last name', 'City' and 'Postcode' fields are specified.|
    |**Account details**|Information on the profile's account  such as its status or account number.|
    |**No longer contact**|The contact preferences of the profile. When any of these options is selected, the profile is on denylist.<br/>For example, if the recipient clicked an unsubscription link in a newsletter, this information is added to the contact data. Such recipient is no longer targeted on the selected channel(s). Learn more on quarantine management in [Adobe Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"}|
    |**Custom fields**|If custom fields have been configured, they display in this section. Custom fields are additional attributes added to the **[!UICONTROL Profiles]** schema through the Adobe Campaign console. Learn more in the [Adobe Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}|
    |**Others**|Additional built-in attributes.|

1. Once you have configure the profile, click **[!UICONTROL Create]** to save it into the database.

    Once done, you can edit the profile at any time by opening it from the profiles' list. [Learn how to explore profiles' details](profile-view.md) 
