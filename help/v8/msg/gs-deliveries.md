---
product: campaign
title: Access deliveries
description: Learn how to access and manage your deliveries in Campaign Web
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
 
exl-id: 3afff35c-c15f-46f8-b791-9bad5e38ea44
---
# Access deliveries {#work-with-deliveries}

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Deliveries"
>abstract="A delivery is a communication sent to an audience on a specific channel: email, SMS, or Push. In this screen, you can edit, duplicate, and delete existing deliveries. You can also view reports for completed deliveries. Click the **Create delivery** button to add a new delivery."

## Access deliveries {#access}

>[!CONTEXTUALHELP]
>id="acw_deliveries_additional_target"
>title="Additional target"
>abstract="These rules can only be changed in the client console."

Deliveries are accessible from the **[!UICONTROL Deliveries]** menu on the left navigation. All deliveries created either from the client console or the Web User Interface appear in this list. From this screen, you can monitor all existing deliveries, duplicate or delete them, or create new ones.

![List of deliveries displayed in the interface](assets/deliveries-list.png)

To open a delivery, click its name from the list. The delivery opens, allowing you to perform various actions such as editing its parameters, checking its execution, or monitoring its performance using dedicated reports.

![Delivery details screen showing parameters and reports](assets/delivery-details.png)

If you open a delivery created in the client console, two new sections may display for the audience. These parameters can be modified in the console only.

* **[!UICONTROL Additional target]**: indicates that multiple targets have been configured for this delivery.

* **[!UICONTROL Additional proof target]**: indicates that a dynamic condition has been defined for proof targets in this delivery. 

![Warning message about additional target configuration](assets/target-warning-audience.png){zoomable="yes"}

## Duplicate a delivery {#delivery-duplicate}

You can create a copy of an existing delivery, either from the delivery list or from the delivery dashboard.

To duplicate a delivery from the list of deliveries, follow these steps:

1. Click the three dots button on the right, next to the name of the delivery to duplicate.
1. Select **[!UICONTROL Duplicate]**.
1. Confirm duplication. The new delivery dashboard opens in the central screen.

To duplicate a delivery from its dashboard, follow these steps:

1. Open the delivery and click the **[!UICONTROL ...More]** button on the top section of the screen.
1. Select **[!UICONTROL Duplicate]**.
1. Confirm duplication. The new delivery replaces the current delivery in the central screen.

## Delete a delivery {#delivery-delete}

Deliveries are deleted from the delivery list, either from the main delivery entry in the left rail or from the delivery list of a campaign.

To delete a delivery from the list of deliveries, follow these steps:

1. Click the three dots button on the right, next to the name of the delivery to delete.
1. Select **[!UICONTROL Delete]**.
1. Confirm deletion.

![Deleting a delivery from the delivery list interface](assets/delete-delivery-from-list.png)

All deliveries are available in these lists, but deliveries created in a workflow cannot be deleted from there. To delete a delivery created in the context of a workflow, delete the delivery activity from the workflow.

To delete a delivery from a workflow, follow these steps:

1. Select the delivery activity.
1. Click the **[!UICONTROL Delete]** icon on the right panel.
1. Confirm deletion. If the delivery has child nodes, choose to delete them as well or keep them.

![Deleting a delivery activity within a workflow](assets/delete-delivery-from-wf.png)