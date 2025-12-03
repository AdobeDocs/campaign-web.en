---
title: Branding
description: Discover how to configure your brand
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
---
# Configure brands {#branding-configure}

>[!IMPORTANT]
>
>Brands cannot be created or modified by end-users: these operations have to be performed by Adobe Campaign technical administrator. For any request, contact Adobe Customer care.

In Adobe Campaign V8, Brands can be found in the **[!UICONTROL Administration > Platform > Branding]** menu.

A **[!UICONTROL Brand]** is defined by the following characteristics:

* An **[!UICONTROL Identity]**, which defines and personalizes your brand. This section contains the following fields:

    * **[!UICONTROL Label]** visible in the interface
    * **[!UICONTROL ID]**
    * **[!UICONTROL Brand name]**
    * **[!UICONTROL Website URL]** and **[!UICONTROL Website label]** of the brand
    * **[!UICONTROL Brand logo]**

  ![](assets/branding_1.png)

* **[!UICONTROL Header parameters of sent emails]** which personalizes what the recipients of your campaigns will see. This section contains the following fields:

    * **[!UICONTROL Sender (email address)]** with the brand's email address.
    * **[!UICONTROL Sender (name)]** with the brand's name.
    * **[!UICONTROL Reply to (email address)]** with the email address the customer can reply to.
    * **[!UICONTROL Reply to (name)]** with the brand's name.
    * **[!UICONTROL Error (email address)]** with the email address to use in case of an error.

  >[!IMPORTANT]
  >
  >After having updated the header parameters of the emails, if the name and email address of the sender have not changed in the email created from the template, check the template's advanced settings.

  ![](assets/branding_2.png)

* **[!UICONTROL Brand configs]** defines the servers used for tracking also for landing page access. This section contains the following fields:

    * **[!UICONTROL Brand subdomain]** refers to the designated subdomain URL specific to this brand, requested for delegation from Adobe.

  Note that configuration for tracking, mirror, and application servers is stored in separate external accounts associated with routing. These settings are applied during provisioning and should not be modified. To display URLs, access the **[!UICONTROL Branding prefixes]** tab from your external account.

  ![](assets/branding_3.png)

* **[!UICONTROL Tracking URL configs]** menu enables you to enhance URL tracking by defining additional parameters for integration with Web analytics tools such as Adobe Analytics and Google Analytics. 

  Use the **[!UICONTROL Additional URL Parameters]** menu to create additional parameters as key-value pairs along with their applicability conditions. Each parameter name must be unique and non-empty, and each parameter value must be non-empty. The applicability condition can be empty, but none of these values can include JST tags.

  These parameters will be applied to tracked URLs that match any domain name specified in the **[!UICONTROL List of Domain Names]**, which can include regular expressions.

  **Example:** A tracked URL like `https://www.example.com` will become `https://www.example.com/?age=21&deliveryName=DM101` when the additional parameters `age=21` and `deliveryName=DM101` are configured for that domain.

## Configure branding for transactional messaging {#branding-transactional-config}

>[!IMPORTANT]
>
>This section applies only to Transactional messaging (Message Center).
>
>While transactional capabilities are available in the Campaign Web UI, the steps below must be performed in the Campaign v8 Client Console (control instance).

If you are using Transactional messaging (Message Center) with branding, additional configuration is required.

### Tracking formulas for Real-Time instances

When branding is activated on a Real-Time (RT) control instance, specific tracking options are used to manage tracking formulas. These formulas are configured centrally on the RT Control instance rather than individually on each RT Execution instance.

The following options define the tracking formulas used by RT deliveries:

* **`NmsTracking_RT_ClickFormula`**: specifies the formula used for click tracking on RT instances

* **`NmsTracking_RT_OpenFormula`**: specifies the formula used for open tracking on RT instances

If your implementation requires custom tracking formulas for transactional messaging, use the option below:

* **`Branding_RT_ListXtkOptions_toPublish`**: list the XTK option names for your custom formulas here (separated by commas). This ensures that RT deliveries can apply the custom tracking formulas.