---
title: Guardrails and limitations in Campaign Web user interface workflows
description: Guardrails and limitations when working with workflows in Campaign Web user interface
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
---
# Guardrails and limitations for workflows {#guardrails-limitations}

When working in Campaign Web user interface with workflows created or modified in Campaign client console, the guardrails and limitations listed below apply.

Please note that, while this page identifies key considerations when working with workflows in the console and the web user interface, it does not encompass every potential incompatibility between the two interfaces. 

## Workflow activities {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Activity non editable"
>abstract="When a **Query** or an **Enrichment** activity is configured with additional data in the console, the enrichment data is taken into account in Campaign Web and passed into the outbound transition, but it cannot be edited."

Workflow activities that are not supported yet in Campaign Web user interface are read-only and displayed as incompatible activities. You can still execute the workflow, send messages, check the logs, etc. Workflow activities that are available both in the Campaign Web user interface and the Campaign client console are editable. 

| Console | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

When a **Query** or an **Enrichment** activity is configured with additional data in the console, the enrichment data is taken into account in Campaign Web and passed into the outbound transition, but it cannot be edited.

| Console | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

In the console, the **Enrichment** activity can perform both reconciliation and enrichment. If you have defined, in the client console, reconciliation settings in the **Enrichment** activity, it will be displayed as a **Reconciliation** activity in Campaign Web user interface.

| Console | Web |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## Workflow canvas {#wkf-canvas}

When creating a new workflow in Campaign Web user interface, the canvas only supports one entry point. However, if you created a worflow in the console with multiple entry points, you can open and edit it in Campaign Web user interface. 

| Console | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

The positioning of the nodes is refreshed everytime an activity is added or removed. If you create a workflow in the console, modify it using Campaign Web user interface and re-open it in the console, you may notice some minor positioning imperfections. This has no impact on the workflow's processes and tasks.

| Initial workflow | Positionning change |
| --- | --- |
| ![](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |
