---
title: Guardrails and limitations in Campaign Web UI
description: Guardrails and limitations in Campaign Web UI
badge: label="Beta" 
---

# Guardrails and limitations {#guardrails-limitations}

When working in Campaign web UI with components created or modified in Campaign client console, the guardrails and limitations listed below apply.

## Workflows {#wf-guardrails-limitations}

The same workflow can be accessed both in the console and the web UI. However, please be aware that certain limitations apply.

**Activity Edition**

*  When accessing a console workflow in the web UI, you can only modify activities that are compatible.

**Canvas edition**

* If a console workflow has multiple start nodes/branches or floating activities, you need to add a start activity and a fork to connect start nodes to the main node. You also need to remove floating activities.

**Activity positioning**

* The positioning of the nodes will be recalculated (the initial positioning of the activities will therefore be modified) only when an activity has been added or removed (not all the time).

**Un-exposed options**

* Non-compatible options are not displayed in the web UI. 

**Loops**

* Wokflows including loops are not displayed in the web UI. An error message is displayed.

**Reconciliation and enrichment**

In the Campaign client console, the **Enrichment** activity can perform both reconciliation and enrichment. In Campaign web UI, reconciliation capabilities are not available yet. If you have set reconciliation in the console activity, it will be displayed as a non-compatible activity in the web UI. 

   * If the **Enrichment** activity in the console only performs an enrichment, the **Enrichment** activity is displayed in the web. 
   * If the **Enrichment** activity in the console only performs a reconciliation, an incompatible activity is displayed. 

## Predefined filters {#filters-guardrails-limitations}


When selecting the audience of a delivery, or when building an audience in a workflow, some predefined filters are not available. A specific error message is displayed. You can still use the query, and see: the filtering condition and the results, but you cannot view the exact query in the rule builder, and cannot edit the filter. 

![](assets/filter-unavailable.png)
