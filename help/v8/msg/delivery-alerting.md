---
audience: end-user
title: Delivery alerting
description: Learn how to work with delivery alerting.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
---
# Get started with delivery alerting {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Delivery alerting"
>abstract="Delivery Alerting is now available in Campaign. This capabiltiy is an alert management system that enables groups of users to automatically receive email notifications with information on their delivery executions."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"

Delivery Alerting is an alert management system that enables groups of users to automatically receive email notifications with information on their delivery executions. Recipients can monitor ongoing deliveries processed by Adobe Campaign and take appropriate actions if issues arise.

Notifications can be customized based on specific alerting criteria defined through the Adobe Campaign Web User Interface.

For more in formation on how to manage delivery failures, refer to the [Adobe Campaign v8 (console) documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## Email notification contents {#content}

Email notifications include the following sections:

* **Summary**: Displays the number of deliveries meeting your defined criteria, with labels and colors for each criterion.
* **Details**: Lists all defined delivery criteria for the dashboard and the corresponding deliveries for each criterion.

![](assets/alerting-email.png)

## Set up delivery alerts {#set-up}

To help you set up these alerts, Campaign Web User Interface allows you to create and manage:

* **Delivery alerting dashboards**: Specify recipients, set alerting criteria to include in the dashboard, and access a history of sent alerts. [Learn how to work with dashboards](../msg/delivery-alerting-dashboards.md)
* **Delivery alerting criteria**: Campaign Web User Interface provides pre-defined alerting criteria (deliveries with low throughput, deliveries whose preparation failed...) that you can add to your dashboard. You can also create your own criteria to suit your needs. [Learn how to work with criteria](../msg/delivery-alerting-criteria.md)

Let's say you want to notify users with administration rights only about failed deliveries, and marketing users about deliveries with a high soft bounce error ratio. To achieve this, create two separate dashboards with the appropriate criteria for each group of recipients.

>[!NOTE]
>
>To access and configure dashboards and alerting criteria, you must have **administration rights** or be part of the **Delivery Supervisors** security group. Standard users cannot access dashboards in the Adobe Campaign interface but can receive alerting notifications. [Learn more on access and permissions](../get-started/permissions.md)
