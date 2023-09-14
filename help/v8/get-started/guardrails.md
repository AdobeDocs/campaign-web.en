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

![](assets/filter-unavailable.png){width="70%" align="left"}
 

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