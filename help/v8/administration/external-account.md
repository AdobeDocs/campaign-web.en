---
title: External account
description: Learn how to configure external accounts
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
---
# Configure external accounts {#external-accounts}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="External accounts"
>abstract="You can now connect to additional platforms or customize the connections to fit your workflow, and easily create new external accounts to meet your specific needs and ensure seamless data transfers."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"


>[!AVAILABILITY]
>
> Note that external accounts are currently available only for Bounce mails (POP3) and the Execution instance, with additional account types to be added in the future.
> Non-supported external accounts created in Adobe Campaign console are visible in the Web User Interface but cannot be edited or accessed.

Adobe Campaign comes with a set of pre-configured external accounts for easy integration with various systems. If you need to connect to additional platforms or customize the connections to fit your workflow, you can now easily create new external accounts using Web User Interface to meet your specific needs and ensure seamless data transfers.

## Create an external account {#create-ext-account}

To create a new external account, follow the steps below. Detailed settings depend on the type of external account.

1. From the left-pane menu, select **[!UICONTROL External accounts]** under **[!UICONTROL Administration]**.

1. Click **[!UICONTROL Create external account]**.

    ![](assets/external_account_create_1.png)

1. Enter your **[!UICONTROL Label]** and select your External account **[!UICONTROL Type]**.

    ![](assets/external_account_create_2.png)

1. Click **[!UICONTROL Create]**. 

1. From the **[!UICONTROL Advanced options]** drop-down, you can change the **[!UICONTROL Internal name]** or **[!UICONTROL Folder]** path if needed. 

    ![](assets/external_account_create_3.png)

1. Enable the **[!UICONTROL Exported automatically]** if you want your data managed by this external account to automatically be exported.

1. Configure the access to the account by specifying credentials depending on the chosen external account type.

1. Click **[!UICONTROL Test the connection]** to check that your configuration is correct 

1. From the **[!UICONTROL More...]** menu, duplicate or delete your external account.

    ![](assets/external_account_create_4.png)

1. Once configuration is done, click **[!UICONTROL Save]**.

## Campaign-specific external accounts {#campaign-specific}

### Bounce mails (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 is currently not supported.

The Bounce mail external account specifies the external POP3 account used to connect to the email service. All servers configured for POP3 access can receive return mail.

![](assets/external_account_bounce.png)

To configure the **[!UICONTROL Bounce mails (POP3)]** external account:

* **[!UICONTROL Server]**

    URL of the POP3 server

* **[!UICONTROL Port]**

    POP3 connection port number (default port is 110)

* **[!UICONTROL Account]**

    Name of the user

* **[!UICONTROL Password]**

    User account password

* **[!UICONTROL Encryption]**

    Type of chosen encryption between:

    * By default (POP3 if port 110, POP3S if port 995)
    * POP3 that switches to SSL after the sending of a STARTTLS
    * POP3 non-secure (port 110 by default)
    * POP3 secure above SSL (port 995 by default)

* **[!UICONTROL Function]**

    Inbound email, when the external account is configured to receive incoming emails, or SOAP router, to handle SOAP requests.

### Execution instance{#instance-exec}

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
