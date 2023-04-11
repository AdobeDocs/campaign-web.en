---
audience: end-user
title: Work with workflows data management activities
description: Learn how to use data management activities into Adobe Campaign Web workflows
badge: label="Alpha" type="Positive"
---
# Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section

## Enrichment {#enrichment}

description: add one or multiple enrichment data, can leverage to personalize deliveries
use case: retrieve the latest purchase or last digital subscription and total amount of a purchase and personalize an email with it

process
use example: retrieve 4 latest purchases that are less than 100$ and personlize an email with it
1. add activity
1. select attribute to use as enrichment data

    + display advanced fields option
    + i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    + select an existing filter
    + save the filter for reuse
    + view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?
