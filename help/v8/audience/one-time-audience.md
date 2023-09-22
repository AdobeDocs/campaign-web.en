---
audience: end-user
title: Build a one-time audience for a delivery
description: Learn how to build a one-time audience for a delivery.
badge: label="Beta" 
---
# Build a one-time audience for a delivery {#sone-time}

This section describes how to build an audience when creating a new delivery. In this case, the recipients to include in the delivery audience are targeted by querying the database with the rule builder.

The resulting audience is only used once for this delivery. It is not saved in the audiences list.

When defining the main target of a delivery, you can also:

* [Select an existing audience](add-audience.md) from the **[!UICONTROL Audiences]** list.
* [Load an audience from an external file](file-audience.md) (for emails only).

To build a new audience directly from a delivery, follow these steps: 

1. From the **Audience** section of the delivery creation assistant, click the **[!UICONTROL Select audience]** button.

    ![](assets/segment-builder0.png)

1. Select **Create your own**. The rule builder is displayed. It allows you to define the population targeted by your delivery by filtering data contained in the database. [Learn how to use the rule builder](segment-builder.md)

    ![](assets/segment-builder.png)

1. Once your query is ready, click **Confirm** to use the audience as the main target of your delivery.

   You can also set a control group to measure the impact of your campaigns. The control group do not receive the message. This allows you to compare the behavior of the population which received the message with the behavior of contacts which did not. [Learn more](control-group.md)
