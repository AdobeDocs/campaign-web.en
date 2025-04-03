---
audience: end-user
title: Permission management in Campaign Web user interface
description: Learn more about permissions in Campaign Web user interface
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
---
# Permissions {#permissions}

Each user in Adobe Campaign has specific permissions and restrictions in the application. The user can belong to an operators group and inherit the group's permissions.

Based on their permissions, an operator can:

* Access certain capabilities
* Access certain data
* Access certain actions (create, modify, delete)

A detailed procedure for setting up permissions in Adobe Campaign is available in [Adobe Campaign v8 (console) documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.

## Permissions on folders {#folder-permissions}

Based on your rights, you can view and manage permissions on folders in the **[!UICONTROL Folder settings]**.

Below is an example of a delivery folder:

  ![Example of folder settings in Adobe Campaign](assets/folder_settings.png){zoomable="yes"}

In the **[!UICONTROL Security]** section of the **[!UICONTROL Folder settings]**, you can view and manage (add or delete) operators or groups who can access the folder.

  ![Example of folder security settings in Adobe Campaign](assets/folder_security.png){zoomable="yes"}

You can directly click on the permissions and change them to either **[!UICONTROL Allowed]** or **[!UICONTROL Denied]**.

  ![Example of denied permissions in folder security settings](assets/folder_security_denied.png){zoomable="yes"}

If the **[!UICONTROL Propagate]** option is enabled, all permissions defined for a folder apply to all its sub-folders. These permissions can be overridden for each sub-folder.

If the **[!UICONTROL System folder]** option is selected, access is allowed to all operators, regardless of their permissions.

You can also [manage the permissions on folders in Adobe Campaign console](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

All permissions in the Campaign Web user interface synchronize with Campaign Client Console permissions.