---
audience: end-user
title: Use the End workflow activity
description: Learn how to use the End workflow activity
---
# End {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="End activity"
>abstract="The **End** activity allows you to graphically mark the end of a workflow. When more than one inbound transition is available, use the **Sets to join** section to select which transitions to connect to the activity."

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_sets"
>title="Sets to join"
>abstract="Check the previous activities you wish to connect as inbound transitions of the **End** activity. The selected activities are then connected to the **End**. This section is only displayed when more than one inbound transition is available to be connected to the activity."

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="External signal"
>abstract="placeholder for the external signal section in the End activity parameters. Available for orchestrated campaigns only. DO NOT DELETE"

The **End** activity is a **Flow control** activity. It allows you to graphically mark the end of a workflow. This activity is optional.

The activity supports multiple inbound transitions. When more than one inbound transition is available. 

In the **Sets to join** section, check the previous activities you wish to connect as inbound transitions of the **End** activity. The selected activities are then linked to the **End** in the workflow canvas.

![Workflow deduplication configuration process](../assets/workflow-end.png) 
