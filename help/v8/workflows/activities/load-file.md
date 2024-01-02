---
audience: end-user
title: Use the Load file workflow activity
description: Learn how to use the Load file workflow activity
badge: label="Limited Availability"
---
# Load file {#load-file}


The **Load file** activity is a **Data management** activity. Use this activity to target profiles stored in an external file. Profiles are not added to the database, but all fields in the input file are available for [personalization](../personalization/gs-personalization.md). Supported file formats are: text (TXT) and comma-separated value (CSV).

This activity can be used with a Reconciliation activity to link unidentified data to existing resources. For example, the **Load file** activity can be placed before a **Reconciliation** activity if you import non-standard data into the database. 

## Best practices{#load-best-practices}



## Configure the Load file activity {#load-configuration}

Follow these steps to configure the **Load file** activity:


1. Drag and drop a **Load file** activity into your workflow. This activity should be added following a transition containing a population whose targeting dimension does not directly come from Adobe Campaign. 
1. Select the new targeting dimension. By default, the targeting dimension is the recipient table (Recipients (nms)), but you can select any other dimension. A dimension lets you define the targeted population: recipients, contract beneficiaries, operators, subscribers, etc. Learn more about targeting dimensions in [this page](../../audience/about-recipients.md#targeting-dimensions).


## Example{#load-example}

In the following example, the activity is configured so that the workflow 


