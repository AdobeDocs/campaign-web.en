---
audience: end-user
title: About read-only workflows
description: Learn why workflows are on read-only mode

---
# About read-only workflows {#readonly-workflows}

Some workflows may be in read-only mode. You can see it with :

- The mention **Read-only** near the Settings button
- The monitoring buttons not accessible

![](assets/readonly-workflow.png){zoomable="yes"}

Nothing in the read-only workflow is editable. The settings of activities are not permitted to change. 


![](assets/scheduler-readonly.png){zoomable="yes"}

In some activities (like javascript code for example), you have the possibility to access and change the code content but the modifications won't be saved.

You don't have the rights to delete the workflow also.

![](assets/readonly-rights.png){zoomable="yes"}

## Why do we have read-only workflows 

Read-only mode is for users who don't have permission and access rights to edit those workflows. [Learn more here](../get-started/permissions.md)

A campaign user may have restrictions in the data he can access in Adobe Campaign. The administrator can give him the possibility to view some features but not to work on them.

## Different types of read-only workflows

According to the type of the workflow, the read-only mode may be different.

### Campaign workflows

In the case of a campaign workflow, there is no monitoring button accessible. 

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Technical workflows

Technical workflows are all in read-only mode for campaign users. But the user can **pause** or **stop** it if needed. Those are the only actions allowed. 

![](assets/readonly-technical-workflow.png){zoomable="yes"}