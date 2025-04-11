---
audience: end-user
title: Build a one-time audience for a delivery
description: Learn how to build a one-time audience for a delivery.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
---
# Build a one-time audience {#one-time}

This section explains how to build an audience when creating a new delivery. In this scenario, the profiles included in the delivery audience are targeted by querying the database using the query modeler. The resulting audience is used only once for this delivery and is not saved in the audiences list.

When defining the main target of a delivery, you can also:
* [Select an existing audience](add-audience.md) from the **[!UICONTROL Audiences]** list.
* [Load an audience from an external file](file-audience.md) (for emails only).

To build a one-time new audience for a delivery, follow these steps:

1. From the **Audience** section of the delivery creation assistant, click the **[!UICONTROL Select audience]** button.

    [Screenshot showing the Audience section of the delivery creation assistant with the Select audience button highlighted](assets/segment-builder0.png){zoomable="yes"}

1. Select **Create your own** to open the query modeler. The query modeler allows you to define the targeted population by filtering data contained in the database. [Learn how to use the query modeler](../query/query-modeler-overview.md).

    [Screenshot showing the query modeler interface](assets/query-modeler.png){zoomable="yes"}

1. Once your query is ready, click **Confirm** to use the resulting audience as the main target of your delivery.

   You can also set a control group to measure the impact of your campaigns. The control group does not receive the message. This allows you to compare the behavior of the population that received the message with the behavior of contacts that did not. [Learn more](control-group.md).