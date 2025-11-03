---
title: Manage external account
description: Learn how to configure CRM external accounts
---
# CRM external account {#external-crm}

Use an external CRM-type account to connect Adobe Campaign with a third-party database.

The configuration settings for this external account depend on the specific database engine you are connecting to. Detailed setup instructions for each supported database are provided in the sections below.

## Microsoft Dynamics CRM

The Microsoft Dynamics CRM external account allows you to connect your Campaign instance to your Microsoft Dynamics CRM external database.

In Adobe Campaign Web User Interface, configure your Microsoft Dynamics CRM external account.

1. [Create your external account](external-account.md) and select **[!UICONTROL External database]** as your external account's **[!UICONTROL Type]** and Microsoft Dynamics CRM as **[!UICONTROL Provider type]**.

1. Click **[!UICONTROL Create]**. 

1. To configure the **[!UICONTROL Microsoft Dynamics CRM]** external account, fill in the following fields:

    ![Screenshot showing the Microsoft Dynamics CRM external account configuration fields.](assets/crm-microsoft-1.png)

    +++ For CRM OAuth type: Password credentials

      * **[!UICONTROL Server]**: Enter the URL of your Microsoft CRM server.
        
        To locate your Microsoft CRM Server URL, sign in to your Microsoft Dynamics CRM account, select Dynamics 365, then open your app. The server URL is displayed in your browser's address bar, for example:`https://myserver.crm.dynamics.com/`.

      * **[!UICONTROL Account]**: Specify the account used to sign in to Microsoft CRM.

      * **[!UICONTROL Password]**: Enter the password associated with the specified account.

      * **[!UICONTROL Client identifier]**: Enter the Client ID found in the Microsoft Azure Management Portal.

      * **[!UICONTROL CRM version]**: Choose Dynamics CRM 365 CRM version.

    +++

    </br>

    +++ For CRM O-Auth type: Certificate

      * **[!UICONTROL Server]**: Enter the URL of your Microsoft CRM server.
        
        To locate your Microsoft CRM Server URL, sign in to your Microsoft Dynamics CRM account, select Dynamics 365, then open your app. The server URL is displayed in your browser's address bar, for example:`https://myserver.crm.dynamics.com/`.

      * **[!UICONTROL Private Key(Base64 encoded)]**: Provide the private key encoded in Base64 format.

        To do so, you can use the help of a Base64 encoder or use the command line `base64 -w0 private.key` for Linux.

      * **[!UICONTROL Custom Key identifier]**: Enter the custom key identifier used for your certificate.

      * **[!UICONTROL Key ID]**: Enter the key ID associated with your certificate.

      * **[!UICONTROL Client identifier]**: Enter the Client ID found in the Microsoft Azure Management

      * **[!UICONTROL CRM version]**: Choose Dynamics CRM 365 CRM version.

    +++

1. After setting up the connection, access **[!UICONTROL Microsoft CRM configuration wizard]** to generate your Microsoft CRM tables list.

    Click **[!UICONTROL Next]** to select the tables required.

    ![Screenshot showing the Microsoft Dynamics CRM external account configuration fields.](assets/crm-microsoft-2.png)
  
1. Select the Microsoft CRM tables to retrieve, or add a remote table by specifying the **[!UICONTROL Table label]** and **[!UICONTROL Table internal name]**, then enable the **[!UICONTROL Selected]** toggle.

    Click **[!UICONTROL Next]**.

1. Click **[!UICONTROL Start]** to begin creating the Microsoft CRM schema based on the selected tables.

1. Follow the on-screen instructions to insert pages from Adobe Campaign Marketing History and Subscription Management directly into Microsoft Dynamics CRM.

1. Click **[!UICONTROL Display marketing history URLs]** to view the URLs for integrating Marketing History pages or **[!UICONTROL Display URLs for lead subscriptions]** to view the URLs for integrating Subscription Management pages.

    ![Screenshot showing the Microsoft Dynamics CRM external account configuration fields.](assets/crm-microsoft-3.png)

1. Click **[!UICONTROL Save]** once your Microsoft CRM external account is configured.

1. Once your External account is created, you can now click **[!UICONTROL Synchronizing enumerations...]** to synchronize enumerations automatically from Microsoft CRM to Adobe Campaign Web User Interface.
  
    ![Screenshot showing the Microsoft CRM CRM external account configuration fields.](assets/crm-microsoft-4.png)

1. Select the Adobe Campaign enumeration that matches the Microsoft CRM enumeration.
  
    To replace Adobe Campaign values with Microsoft CRM values, enable the **[!UICONTROL Replace]** option.

## Salesforce {#salesforce}

To configure the Salesforce external account to work with Adobe Campaign, you need to provide the following details:

1. [Create your external account](external-account.md) and select **[!UICONTROL External database]** as your external account's **[!UICONTROL Type]** and Salesforce.com as **[!UICONTROL Provider type]**.

    ![Screenshot showing the Salesforce external account configuration fields.](assets/crm-salesforce-1.png)

1. Click **[!UICONTROL Create]**. 

1. To configure the **[!UICONTROL Salesforce]** external account, fill in the following fields:

      * **[!UICONTROL CRM O-Auth type]**: **[!UICONTROL Password credentials]** or **[!UICONTROL Credentials]**

      * **[!UICONTROL Account]**: Account used to sign in to Salesforce CRM.

      * **[!UICONTROL Password]**: Enter the password associated with the specified account.

      * **[!UICONTROL Security token]**: Enter the Salesforce security token associated with the account.

      * **[!UICONTROL API version]**: Choose Version 49.

    ![Screenshot showing the Salesforce external account configuration fields.](assets/crm-salesforce-2.png)

1. Open the **[!UICONTROL Salesforce CRM configuration wizard]** to generate your Salesforce CRM tables list, then click **[!UICONTROL Next]**.

    ![Screenshot showing the Salesforce CRM external account configuration fields.](assets/crm-salesforce-3.png)
  
1. Select the Salesforce tables to retrieve, or add a remote table by entering the **[!UICONTROL Table label]** and **[!UICONTROL Table internal name]**, then enable the **[!UICONTROL Selected]** toggle.

    Click **[!UICONTROL Next]**.

1. Click **[!UICONTROL Start]** to begin creating the Salesforce CRM schema based on the selected tables.

1. Click **[!UICONTROL Salesforce link creation wizard...]** to generate the web links in Salesforce.

    Then, click **[!UICONTROL Next]** to retrieve the web links for **Leads** and **Contacts** from Salesforce.

1. Select the links to export to the Salesforce web links list.

1. Follow the on-screen instructions to insert **Marketing History** and **Subscription Management** pages from Adobe Campaign Web User Interface into Salesforce CRM.

1. Click **[!UICONTROL Save]** once your Salesforce CRM external account is configured.

1. Once your External account is created, you can now click **[!UICONTROL Synchronizing enumerations...]** to synchronize enumerations automatically from Salesforce to Adobe Campaign Web User Interface.
  
    ![Screenshot showing the Salesforce CRM external account configuration fields.](assets/crm-salesforce-4.png)

1. Select the Adobe Campaign enumeration that matches the Salesforce enumeration.
  
    To replace Adobe Campaign values with Salesforce values, enable the **[!UICONTROL Replace]** option.

    ![Screenshot showing the Salesforce CRM external account configuration fields.](assets/crm-salesforce-5.png)

