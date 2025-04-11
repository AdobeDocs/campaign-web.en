---
audience: end-user
title: About read-only workflows
description: Learn why workflows are on read-only mode
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
---
# About read-only workflows {#readonly-workflows}

>[!CONTEXTUALHELP]  
>id="acw_wf_read_only_canvas"  
>title="This workflow is read only"  
>abstract="You cannot edit this workflow due to your rights or the type of the workflow."

Some workflows are read-only. Built-in technical workflows are always read-only, but this restriction can also apply to other types of workflows.

Campaign users may have restricted access to Adobe Campaign data. A Campaign administrator can grant them the right to view certain features, but not to edit or modify them. User permissions on data are essential to ensure data and process security. Learn more about permissions management in Campaign in [this section](../get-started/permissions.md).

When a workflow is in read-only mode:

* The mention **[!UICONTROL Read-only]** appears near the **[!UICONTROL Settings]** button.  
* The action buttons are not accessible.  

![Read-only workflow interface showing the settings button and disabled action buttons.](assets/readonly-workflow.png){zoomable="yes"}

Users cannot edit anything in a read-only workflow. They are not allowed to change the settings of the activities.

![Scheduler interface in read-only mode, showing disabled settings options.](assets/scheduler-readonly.png){zoomable="yes"}

Users cannot delete the workflow.

![Interface showing restricted rights for deleting workflows.](assets/readonly-rights.png){zoomable="yes"}

## Types of read-only workflows {#readonly-workflow-types}

Depending on the type of workflow, the read-only mode may vary.

### Campaign workflows {#readonly-campaign-wf}

In a read-only campaign workflow, the user cannot access the monitoring button.

![Campaign workflow interface in read-only mode, showing disabled monitoring options.](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Technical workflows {#readonly-tech-wf}

Built-in technical workflows are read-only for all Campaign users, including administrators. However, users can **pause** or **stop** them if needed. These are the only actions allowed.

![Technical workflow interface in read-only mode, showing options to pause or stop workflows.](assets/readonly-technical-workflow.png){zoomable="yes"}

Learn more about technical workflows in [this section](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows).