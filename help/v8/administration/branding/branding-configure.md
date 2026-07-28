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

Technical administrators can create and manage multiple brands directly from the Web UI. This allows you to define all the elements that make up your brand identity, including logos and even email tracking settings.

>[!NOTE]
>
>This capability requires the branding package on your instance. Contact your Adobe representative if you do not see the **Branding** menu.

## Create or edit a brand {#create-edit-brand}

>[!CONTEXTUALHELP]
>id="acw_branding_create"
>title="Create a brand"
>abstract="Click **Create brand** to define a new brand identity. Fill in the brand details across the configuration tabs, then click **Create brand** to save. The brand becomes available to be linked to delivery templates and standalone deliveries."

To create a new brand, follow these steps:

1. Browse to **[!UICONTROL Administration > Branding]** from the left menu, or to **[!UICONTROL Administration > Platform > Branding]** from the **[!UICONTROL Explorer]**.

1. Click the **[!UICONTROL Create brand]** button above the list.

   ![Screenshot showing the brand creation](assets/branding-create.png)

1. Fill in the brand details across the different sections. Each field is described in the [Brand attributes](#brand-attributes) section below.

   ![Screenshot showing the brand creation fields](assets/branding-create2.png)

1. Click **[!UICONTROL Create brand]** to save. The brand is now available to be linked to delivery templates and standalone deliveries. [Learn how to assign a brand](branding-assign.md).

To edit an existing brand, select it from the list, update the fields, and save your changes.

## Brand attributes {#brand-attributes}

A **[!UICONTROL Brand]** is configured across four sections: **[!UICONTROL Identity]**, **[!UICONTROL Brand configs]**, **[!UICONTROL Email header parameters]**, and **[!UICONTROL URL tracking parameters]**.

### Identity {#identity}

The **[!UICONTROL Identity]** section allows you to define and personalize your brand.

![Screenshot showing the Identity tab when creating a brand](assets/branding-create3.png)

This section contains the following fields:

* **[!UICONTROL Brand name]**: The name of your brand. This field is required.
* **[!UICONTROL Label]**: The label visible in the interface.
* **[!UICONTROL ID]**: The internal identifier automatically generated. You can change it. Only letters, digits, and underscores are allowed. Special characters are replaced with underscores.
* **[!UICONTROL Logo URL]**: The URL of the brand logo image.
* **[!UICONTROL Website URL]** and **[!UICONTROL Website label]**: The website URL and label associated with the brand.


### Brand configs {#brand-configs}

In the **[!UICONTROL Brand configs]** section, you define the subdomain and URL protocols used for tracking and landing page access. 

![Screenshot showing the Brand configs tab](assets/branding-create4.png)

This section contains the following fields:

* **[!UICONTROL Brand subdomain]**: The subdomain URL specific to this brand, requested for delegation from Adobe.
* **[!UICONTROL Tracking URL protocol]**, **[!UICONTROL Mirror page URL protocol]**, and **[!UICONTROL Application URL protocol]**: The protocol used for each URL type (for example, **Secure (https)**).

>[!NOTE]
>
>Configuration for tracking, mirror, and application servers is stored in separate external accounts associated with routing. These settings are applied during provisioning and should not be modified. To display URLs, access the **[!UICONTROL Branding prefixes]** tab from your external account.

### Email header parameters {#header-param}

The **[!UICONTROL Email header parameters]** allow you to personalize what the recipients will see in the header section of your campaigns.

![Screenshot showing the Header params tab with email header fields](assets/branding-create5.png)

This section contains the following fields:

* **[!UICONTROL Sender (email address)]**: The brand's email address.
* **[!UICONTROL Sender (name)]**: The brand's name.
* **[!UICONTROL Reply-to (email address)]**: The email address the customer can reply to.
* **[!UICONTROL Reply-to (name)]**: The display name for replies.
* **[!UICONTROL Error (email address)]**: The email address to use in case of an error.

<!--
>[!IMPORTANT]
>
>After having updated the header parameters of the emails, if the name and email address of the sender have not changed in the email created from the template, check the template's advanced settings.
-->

### URL tracking parameters {#tracking-param}

In the **[!UICONTROL URL tracking parameters]** section, you can enhance URL tracking by defining additional parameters for integration with Web analytics tools such as Adobe Analytics and Google Analytics.

![Screenshot showing URL tracking parameters in the Header params tab](assets/branding-create6.png)

This section contains the following fields:

* **[!UICONTROL Additional URL parameters]**: Add parameters as key-value pairs along with their applicability conditions. Each parameter name must be unique and non-empty, and each parameter value must be non-empty. The applicability condition can be empty, but none of these values can include JST tags.

* **[!UICONTROL Domain name allow-list]**: Add domain names or regular expressions to match URLs where tracking parameters will be appended.

**Example:** A tracked URL like `https://www.luma.com` will become `https://www.luma.com/?age=21&deliveryName=DM101` when the additional parameters `age=21` and `deliveryName=DM101` are configured for that domain.

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
