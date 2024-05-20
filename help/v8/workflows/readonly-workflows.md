---
audience: end-user
title: About read-only workflows
description: Learn why workflows are on read-only mode

---
# About read-only workflows {#readonly-workflows}

Some workflows may be in read-only mode. You can see it with :

- The mention **[!UICONTROL **Read-only**]**  near the **[!UICONTROL Settings]** button
- The monitoring buttons not accessible

![](assets/readonly-workflow.png){zoomable="yes"}

You cannot edit anything in a read-only workflow. You are not allowed to change the settings of the activities.


![](assets/scheduler-readonly.png){zoomable="yes"}

In some activities (like **[!UICONTROL Javascript Code]** for example), you have the possibility to access and change the code content but the modifications will not be saved.

You do not have the rights to delete the workflow also.

![](assets/readonly-rights.png){zoomable="yes"}

## Why read-only workflows 

Read-only mode is for users who do not have permission and access rights to edit those workflows. [Learn more here](../get-started/permissions.md)

A campaign user may have restrictions in the data he can access in Adobe Campaign. The administrator can give him the possibility to view some features but not to work on them.

## Types of read-only workflows

According to the type of the workflow, the read-only mode may be different.

### Campaign workflows

In the case of a read-only campaign workflow, the user cannot access the monitoring button. 

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Technical workflows

Technical workflows are in read-only mode for campaign users.
Built-in technical workflows are in read-only mode for all, even for the administator users. But the user can **pause** or **stop** them if needed. Those are the only actions allowed. [Learn more here](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}