---
title: Manage external account
description: Learn how to configure external accounts
---
# Campaign-specific external accounts {#external-account}

Follow the steps below to configure the account settings based on the type of external account you selected.

## Bounce mails (POP3) {#bounce}

The Bounce mails external account specifies the external POP3 account used to connect to the email service. All servers configured for POP3 access can receive return mail.

![Screenshot showing the Bounce mails (POP3) external account configuration fields.](assets/external_account_bounce.png)

To configure the **[!UICONTROL Bounce mails (POP3)]** external account, fill in the following fields:

* **[!UICONTROL Server]** - URL of the POP3 server.

* **[!UICONTROL Port]** - POP3 connection port number (default port is 110).

* **[!UICONTROL Account]** - Name of the user.

* **[!UICONTROL Password]** - User account password.

* **[!UICONTROL Encryption]** - Type of chosen encryption, including:
    * By default (POP3 if port 110, POP3S if port 995).
    * POP3 that switches to SSL after sending a STARTTLS.
    * POP3 non-secure (port 110 by default).
    * POP3 secure above SSL (port 995 by default).

* **[!UICONTROL Function]** - Select **[!UICONTROL Inbound email]** to configure the account for receiving incoming emails or **[!UICONTROL SOAP router]** to handle SOAP requests.

>[!IMPORTANT]
>
>Before configuring your POP3 external account using Microsoft OAuth 2.0, you first need to register your application in the Azure portal. For more on this, refer to [this page](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app){target=_blank}.

To configure a POP3 external using Microsoft OAuth 2.0, check the Microsoft OAuth 2.0 option and fill in the following fields:

* **[!UICONTROL Azure Tenant]**

    Azure ID (or Directory (tenant) ID) can be found in the Essentials drop-down of your application overview in the Azure portal.

* **[!UICONTROL Azure Client ID]**

    Client ID (or Application (client) ID) can be found in the Essentials drop-down of your application overview in the Azure portal.

* **[!UICONTROL Azure Client Secret]**

    Client secret ID can be found in the Client secrets column from the Certificates & secrets menu of your application in the Azure portal.

* **[!UICONTROL Azure Redirect URL]**

    Redirect URL can be found in the Authentication menu of your application in the Azure portal. It should end with the following syntax nl/jsp/oauth.jsp, e.g. `https://redirect.adobe.net/nl/jsp/oauth.jsp`.

Internet access is needed for setup and to use the Test Connection button in the client console. After setup, the inMail process can communicate with Microsoft servers without internet.

After entering your different credentials, you can click Setup the connection to finish your external account configuration.

## Routing {#routing}

To configure a specific external account for external deliveries, follow the steps below.

1. Create an external account. [Learn more](create-external-account.md)

1. Select the **[!UICONTROL Routing]** type.

    ![Screenshot showing the Routing external account type selection.](assets/external-account-routing.png){zoomable="yes"}

1. Select the desired channel and click **[!UICONTROL Create]**.

1. In the external account **[!UICONTROL Details]** section, **[!UICONTROL External]** is selected by default as the **[!UICONTROL Delivery mode]**.

    ![Screenshot showing the Delivery mode configuration for Routing external accounts.](assets/external-account-delivery-mode.png){zoomable="yes"}

    >[!NOTE]
    >
    >Currently, **[!UICONTROL External]** is the only available mode.

1. To handle the process after delivery execution, externalize this to a post-processing workflow. Create a workflow with an [External signal](../workflows/activities/external-signal.md) activity and select it from the **[!UICONTROL Post-processing]** field.

    ![Screenshot showing the Post-processing field configuration for Routing external accounts.](assets/external-account-post-processing.png){zoomable="yes"}

1. In the **[!UICONTROL Activity]** field, edit the name of the post-processing workflow activity displayed in the logs. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## Execution instance {#instance-exec}

If you have a segmented architecture, identify the execution instances associated with the control instance and establish connections between them. Transactional message templates are deployed on the execution instance.

![Screenshot showing the Execution instance external account configuration fields.](assets/external_account_exec.png)

To configure the **[!UICONTROL Execution instance]** external account:

* **[!UICONTROL URL]** - URL of the server where the execution instance is installed.

* **[!UICONTROL Account]** - Name of the account, matching the Message Center Agent as defined in the operator folder.

* **[!UICONTROL Password]** - Password of the account as defined in the operator folder.

* **[!UICONTROL Method]** - Choose between Web service or Federated Data Access (FDA). 
    
    For FDA, select your FDA account. Note that Campaign connection to external systems is restricted to advanced users and only available from the client console. [Learn more](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Create archiving workflow]** - For each execution instance registered in the Message Center, regardless of whether you have one or multiple instances, create a separate archiving workflow for each external account associated with the execution instance.
