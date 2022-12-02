---
audience: end-user
title: Work with the Segment Buidler
description: Campaign v8 Web documentation
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
---
# Work with the Segment Builder {#segment-builder}

>[!NOTE]
>
>This documentation is under construction and frequently updated. The final version of this content will be ready in January 2023.

In this example, we will build a segment to target all customers living in Atlanta, San Francisco, or Seattle and born after 1980.

Access the Segments menu, then click the Create segment button.

The segment definition screen allows you to configure all the required fields to define your segment. Learn how to configure segments in the Segmentation Service documentation.

In the Segment properties pane, provide a name and a description (optional) for the segment.

Drag and drop the desired fields from the left pane into the center workspace, then configure them according to your needs.

NOTE
Note that the fields available in the left pane vary depending on how the XDM Individual Profile and XDM ExperienceEvent schemas have been configured for your organization. Learn more in the Experience Data Model (XDM) documentation.

In this example, we need to rely on Attributes and Events fields to build the segment:

Attributes: profiles living in Atlanta, San Francisco or Seattle born after 1980

Events: profiles who opened the Luma application within the last 7 days, then made a purchase within 2 hours after opening the application.

As you are adding and configuring new fields in the workspace, the Segment Properties pane is automatically updated with information on the estimated profiles belonging to the segment.

Once the segment is ready, click Save. It displays in the list of Adobe Experience Platform segments. Note that a search bar is available to help you search a specific segment in the list.

The segment can now be used in your journeys. For more on this, refer to this section.
