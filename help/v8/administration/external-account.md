---
title: Manage external account
description: Learn how to configure external accounts
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
---
# Manage external accounts {#external-accounts}

>[!AVAILABILITY]
>
>* External accounts are currently available only for Bounce mails (POP3), Routing and the Execution instance. Additional account types will be added in the future.
>
>* Non-supported external accounts created in Adobe Campaign console are visible in the Web User Interface but cannot be edited nor accessed.

Adobe Campaign comes with a set of pre-configured external accounts for easy integration with various systems. If you need to connect to additional platforms or customize the connections to fit your workflow, you can now easily create new external accounts using Web User Interface to meet your specific needs and ensure seamless data transfers.

## Create an external account {#create-ext-account}

To create a new external account, follow the steps below. Detailed settings depend on the type of external account. [Learn more](#campaign-specific)

1. From the left-pane menu, select **[!UICONTROL External accounts]** under **[!UICONTROL Administration]**.

1. Click **[!UICONTROL Create external account]**.

    ![](assets/external_account_create_1.png)

1. Enter your **[!UICONTROL Label]** and select the external account **[!UICONTROL Type]**.

    >[!NOTE]
    >
    >The settings for Campaign-specific types are detailed in [this section](#campaign-specific).

    ![](assets/external_account_create_2.png)

1. Click **[!UICONTROL Create]**. 

1. From the **[!UICONTROL Additional options]** drop-down, you can change the **[!UICONTROL Internal name]** or **[!UICONTROL Folder]** path if needed. 

    ![](assets/external_account_create_3.png)

1. Enable the **[!UICONTROL Exported automatically in packages]** option if you want your data managed by this external account to automatically be exported. <!--Exported where??-->

    ![](assets/external_account_create_exported.png)

1. In the **[!UICONTROL Details]** section, configure the access to the account by specifying credentials depending on the chosen external account type. [Learn more](#bounce)

1. Click **[!UICONTROL Test connection]** to check that your configuration is correct. 

1. From the **[!UICONTROL More...]** menu, you can duplicate or delete your external account.

    ![](assets/external_account_create_4.png)

1. Once configuration is done, click **[!UICONTROL Save]**.

## Campaign-specific external accounts {#campaign-specific}

Depending on the external account type you selected, follow the steps below to configure the account settings.

### Bounce mails (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 is currently not supported.

The Bounce mails external account specifies the external POP3 account used to connect to the email service. All servers configured for POP3 access can receive return mail.

![](assets/external_account_bounce.png)

To configure the **[!UICONTROL Bounce mails (POP3)]** external account, fill in the following fields:

* **[!UICONTROL Server]** - URL of the POP3 server

* **[!UICONTROL Port]** - POP3 connection port number (default port is 110)

* **[!UICONTROL Account]** - Name of the user

* **[!UICONTROL Password]** - User account password

* **[!UICONTROL Encryption]** - Type of chosen encryption between:

    * By default (POP3 if port 110, POP3S if port 995)
    * POP3 that switches to SSL after the sending of a STARTTLS
    * POP3 non-secure (port 110 by default)
    * POP3 secure above SSL (port 995 by default)

* **[!UICONTROL Function]** - Inbound email, when the external account is configured to receive incoming emails, or SOAP router, to handle SOAP requests.

### Routing {#routing}

To configure a specific external account that will be used in your external deliveries, follow the steps below.

1. Create an external account. [Learn more](../administration/external-account.md#create-ext-account)

1. Select the **[!UICONTROL Routing]** type.

    ![](assets/external-account-routing.png){zoomable="yes"}

1. Select the desired channel and click **[!UICONTROL Create]**.

1. In the external account **[!UICONTROL Details]** section, **[!UICONTROL External]** is selected by default as the **[!UICONTROL Delivery mode]**.

    ![](assets/external-account-delivery-mode.png){zoomable="yes"}

    >[!NOTE]
    >
    >Currently **[!UICONTROL External]** is the only available mode.

1. To handle the process after your delivery execution, you can externalize this to a post-processing workflow. To do so, you must create a workflow with an [External signal](../workflows/activities/external-signal.md) activity and select it from the **[!UICONTROL Post-processing]** field.

    ![](assets/external-account-post-processing.png){zoomable="yes"}

1. In the **[!UICONTROL Activity]** field, you can edit the name of the post-processing workflow activity that will be displayed in the logs. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->


### Execution instance {#instance-exec}

If you have a segmented architecture, you must identify the execution instances associated with the control instance and establish connections between them. Transactional message templates are deployed on the execution instance.

![](assets/external_account_exec.png)

To configure the **[!UICONTROL Execution instance]** external account:

* **[!UICONTROL URL]**

    URL of the server on which the execution instance is installed.

* **[!UICONTROL Account]**

    Name of the account, it must match the Message Center Agent as defined in the operator folder.

* **[!UICONTROL Password]**

    Password of the account as defined in the operator folder.

* **[!UICONTROL Method]**

    Choose between Web service or Federated Data Access (FDA). 
    In case of FDA method, select your FDA account. Note that Campaign connection to external systems is restricted to advanced users and only available from the client console. [Learn more](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Create archiving workflow]**

    For each execution instance registered in the Message Center, regardless of whether you have one or multiple instances, you need to create a separate archiving workflow for each external account associated with the execution instance.
