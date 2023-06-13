---
audience: end-user
title: Create workflows with Adobe Campaign Web
description: Learn how to build workflows with Adobe Campaign Web
badge: label="Alpha" 
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
---

# Create the workflow {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Workflow properties"
>abstract="In this screen, choose the template to use to create the workflow and specify a label. Expand the Additional options section to configure specific settings such as the workflow storing folder or timezone."

The first step to create your workflow in Campaign v8 Web is to create it either as a standalone workflow or directly within a campaign and to define its general properties. To do so, follow these steps:

1. Start by deciding whether you want to create a standalone workflow or integrate it directly within a campaign:

    * **Standalone workflow**: Navigate to the Worklows menu and click the Create workflow button in the upper-right corner.
    * **Campaign workflow:** Navigate to the Campaigns menu and open the campaign where you want to create a new workflow. Click the Create workflow button in the upper-right corner of the Workflows tab.

    The workflow Properties dialog box appears.

    ![](assets/workflow-create.png)

1. Select the template to use to create the workflow and provide a label for the workflow.

    Workflow templates contain pre-configured activities and overall property configurations that can be reused for creating new workflows. They are created from the client console. [Learn how to work with templates](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

1. Expand the **[!UICONTROL Additional options]** section if you want to configure specific settings for the workflow, such as the storing folder and timezone. [Learn how to configure worklow properties](workflow-settings.md)

1. Click the **[!UICONTROL Create workflow]** button to confirm the creation of your workflow.

With your workflow created, you can now start orchestrating the various tasks it will perform using a dedicated visual canvas. [Learn how to orchestrate workflow activities](orchestrate-activities.md)
