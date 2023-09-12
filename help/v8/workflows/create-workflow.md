---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to create a workflow with Adobe Campaign Web
badge: label="Beta" 
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
---

# Create the workflow {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Workflow properties"
>abstract="In this screen, choose the template to use to create the workflow and specify a label. Expand the ADDITIONAL OPTIONS section to configure more settings such as the workflow internal name, its folder, timezone, and supervisor group. It is highly recommended to select a supervisor group so that operators are alerted if an error occurs."

You can create standalone workflows, or workflows within a campaign. The first step is to select a template and define its general properties. You can then configure additional settings as needed.

To do so, follow these steps:

1. To create a **Standalone workflow**, browse to the **Worklows** menu.
    
    To create a **Campaign workflow**, browse to the **Campaigns** menu, and open the campaign for which you want to create a new workflow. 

1. Click the **[!UICONTROL Create workflow]** button in the upper-right corner of the screen.

    ![](assets/workflow-create.png)

1. In workflow **Properties** dialog, select the template to use to create the workflow (you can also use the default built-in template). Learn more about templates in [the section below](#work-with-workflow-templates-workflow-templates).

1. Enter a label for the workflow. In addition, we strongly recommend you to add a description to your workflow, in the dedicated field of the **[!UICONTROL Additional options]** section of the screen.

1. Expand the **[!UICONTROL Additional options]** section to configure more settings for the workflow. Learn how to configure the worklow properties in [this page](workflow-settings.md#properties)

    ![](assets/workflow-additional-options.png)

1. Click the **[!UICONTROL Create workflow]** button to confirm the creation of your workflow.

Your workflow is now created and available in the list of worklows. You can now access its visual canvas and start adding, configuring, and orchestrating the tasks it will perform. Learn how to orchestrate workflow activities in [this page](orchestrate-activities.md).

## Work with workflow templates {#workflow-templates}

Workflow templates contain pre-configured activities and overall settings that can be reused for creating new workflows. Templates are created from Campaign client console. 

In Campaign v8 Web, you can select the template of your workflow from the workflow properties. An emplty template is provided by default.

Learn how to work with templates in [Campaign (client console) v8 documentation](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates){target="_blank"}.
