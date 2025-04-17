---
product: campaign
title: Audit trail
description: Learn how to monitor your instance with Campaign Audit trail
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
---
# Audit trail {#audit-trail}

In Adobe Campaign Web User Interface, the **[!UICONTROL Audit trail]** feature provides users with full visibility into all modifications made to important entities within your instance, typically those that significantly impact smooth operation of the instance.

>[!IMPORTANT]
>
>* Adobe Campaign Web User Interface does not audit changes made within user rights, templates, personalization, or campaigns.  
>* Only administrators of the instance can manage the audit trail.

The **[!UICONTROL Audit trail]** feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.

+++ Learn more about Audit Trail available entities

* **Source Schema audit trail** allows you to monitor activities and recent modifications made to your schemas within the Campaign v8 client console. 

  For detailed information on schemas, refer to [Campaign v8 Documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **Workflow audit trail** allows you to keep track of activities and recent changes made to workflows, including their current states such as:

    * Start
    * Pause
    * Stop
    * Restart
    * Cleanup, which equals the action Purge history
    * Simulate, which equals the action Start in simulation mode
    * Wakeup, which equals the action Execute pending tasks now
    * Unconditional Stop

  For more information on workflows, refer to this [page](../workflows/gs-workflows.md).

* **Option audit trail** enables you to monitor activities and recent modifications made to your options in Campaign v8. 

  For more information on options, refer to this [page](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Delivery audit trail** allows you to check the activities and last modifications done to your deliveries. 

  For more information on deliveries, refer to this [page](../msg/gs-deliveries.md).

* **External Account** allows you to check modifications made to external accounts in Campaign v8, used by technical processes such as technical workflows or campaign workflows.

  For more information on external accounts, refer to this [page](../administration/external-account.md).

* **Delivery Mapping** enables you to monitor activities and recent modifications made to your Delivery Mapping in Campaign v8. 

  For more information on delivery mapping, refer to this [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Web Application** allows you to check modifications made to Web forms in Campaign v8, used to create pages with input and selection fields, and which may include data from the database. 

  For more information on web applications, refer to this [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* **Offer** allows you to check the activities and last modifications done to your offers.

  For more information on offers, refer to this [page](../msg/offers.md).

* **Operator** enables you to monitor activities and recent modifications made to your Operators in Campaign v8.

  For more information on operators, refer to this [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Accessing Audit trail {#accessing-audit-trail}

To access your instance's **[!UICONTROL Audit trail]**:

1. Under the **[!UICONTROL Administration]** menu, select **[!UICONTROL Audit trail]**.

    ![Screenshot showing the Administration menu with the Audit trail option selected](assets/audit-trail-1.png)

1. The **[!UICONTROL Audit trail]** window opens with the list of your entities. Adobe Campaign Web User Interface audits the create, edit, and delete actions for workflows, options, deliveries, and schemas.

    Select one of the entities to learn more about the last modifications.

1. The **[!UICONTROL Audit entity]** window provides detailed information on the chosen entity, such as:

    * **[!UICONTROL Type]**: Workflow, Options, Deliveries, or Schemas.
    * **[!UICONTROL Entity]**: Internal name of your activities.
    * **[!UICONTROL Modified by]**: Username of the last person who modified this entity.
    * **[!UICONTROL Action]**: Last action performed on this entity, either Created, Modified, or Deleted.
    * **[!UICONTROL Modification date]**: Date of the last action performed on this entity.

    The code block provides more information on what was changed exactly in your entity.

    ![Screenshot showing the Audit entity window with detailed information on modifications](assets/audit-trail-2.png)