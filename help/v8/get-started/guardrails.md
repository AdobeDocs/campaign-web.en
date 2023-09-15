---
title: Guardrails and limitations in Campaign Web UI
description: Guardrails and limitations in Campaign Web UI
badge: label="Beta" 
---

# Guardrails and limitations {#guardrails-limitations}

When working in Campaign web UI with components created or modified in Campaign client console, the guardrails and limitations listed below apply.

## Workflows {#wf-guardrails-limitations}

**Activity Edition**

*  Workflow activities that are not supported yet in the web UI are read-only. You can still execute the workflow, send messages, check the logs, etc.

| Console | Web UI |
| --- | --- |
| ![](assets/limitations-activities-console.png) | ![](assets/limitations-activities-web.png) |

**Canvas edition**

* If a console workflow has multiple start nodes/branches or floating activities, you need to add a start activity and a fork to connect start nodes to the main node. You also need to remove floating activities.

**Activity positioning**

* The positioning of the nodes will be recalculated (the initial positioning of the activities will therefore be modified) only when an activity has been added or removed (not all the time).

**Un-exposed options**

* Non-compatible options are not displayed in the web UI. 

**Loops**

* Loops are not available yet in the web UI. If you have created a wokflow including a loop using the console, it will not be accessible in the web UI. An error message is displayed.

| Console | Web UI |
| --- | --- |
| ![](assets/limitations-loops-console.png) | ![](assets/limitations-loops-web.png) |

**Reconciliation and enrichment**

In the Campaign client console, the **Enrichment** activity can perform both reconciliation and enrichment. In Campaign web UI, reconciliation capabilities are not available yet. If you have set reconciliation in the console activity, it will be displayed as a non-compatible activity in the web UI. 

   * If the **Enrichment** activity in the console only performs an enrichment, the **Enrichment** activity is displayed in the web. 
   * If the **Enrichment** activity in the console only performs a reconciliation, an incompatible activity is displayed. 

## Predefined filters {#filters-guardrails-limitations}

When selecting the audience of a delivery, or when building an audience in a workflow, some predefined filters are not available in the user interface, in that version of the product. 

A specific error message is displayed. Even if you cannot view the graphic representation of the query in the rule builder, and cannot edit the filter, you can still use it, and see the filtering conditions, and the results. You can also access the SQL query to check the exact settings. 

![](assets/filter-unavailable.png){width="70%" align="left"}
 

Note that if you build a filter in the Web interface and modify it in the console with unsupported attributes, the graphic representation can no longer be available in the Web interface. In any cases, you can still use the filter.

Unsupported attributes are listed below.

### Unsupported data types {#unsupported-data-type}

The following data types available in the client console are not supported when displaying a filter or a rule in the Web interface:

* datetime
* time
* timespan
* double
* float

### Unsupported filtering capabilities {#unsupported-filtering-capabilities}

When a filter is built with complex expressions and functions in the client console, it cannot be edited in the Web interface.

In addition, the following operators are not supported:

* Numeric type
    * is included in
    * no in

* String type
    * greater than
    * less than
    * greater than or equals to
    * less than or equals to
    * like
    * not like

* Date type
    * on or after
    * on or before
    * not equals to
    * is empty
    * is not empty
    * is included in
    * not in
    * in last

* 1-N links
    * COUNT, SUM, AVG, MIN, MAX