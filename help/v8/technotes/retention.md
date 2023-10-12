---
title: Technote - Campaign data retention period
description: Understand data retention mechanism and timeline in Campaign 
---

# Retention period

Data retention period is the duration of time for which data should be kept in Campaign database. Built-in log tables in Campaign have pre-set retention periods on them, generally limiting their data storage to six months or less.

The following are the default retention values for built-in tables. Be aware that the retention configuration is set by Adobe technical administrators during implementation and values may vary for each implementation, based on customer requirements.

* **Consolidated tracking**: 1 year
* **Delivery logs**: 6 months
* **Tracking logs**: 1 year
* **Deleted deliveries**: 1 week
* **Import rejects**: 6 months
* **Visitor profiles**: 1 month
* **Offer propositions**: 1 year
* **Events**: 1 month
* **Statistics of event processing**: 1 year
* **Archived events**: 1 year
* **Pipeline events ignored**: 1 month

Learn more about data retention, database performances, and purge mechanisms in [Adobe Campaign (console) v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/implement/datamodel-best-practices.html#data-retention)