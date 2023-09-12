---
audience: end-user
title: Create audiences
description: Learn how to create audiences in Adobe Campaign Web
badge: label="Beta" 
---

# Create audiences {#create-audiences}

audiences menu

can create and target them in standalone deliveries or campaigns

## Create your first audience {#create}

1. Audience > menu
1. Create audience
1. Properties : label and additional options
1. Workflow canvas with a build audience activity
1. Edit activity, edit workflow flow depending on his needs
1. start the workflow (can add targeting activities only? No channel activities?) = Creates the audience and the workflow

## Monitor and manage your audiences {#monitor}

In audience created, dashboard with two tabs:
* overview: properties + workflow status and number of recipient part of this audience by cling calculate + can access and edit workflow from here
* data: view data profiles part of the audience. Can add new columns if needed. See enriched data

audience list: duplicate, delete

**questions:**

Workflow in "audience mode" => sending channel activities not available

* on stage instance: we can remove the last qsave activity and add a channel activity instead
* how do we recognize a workflow in 'audience' mode?
