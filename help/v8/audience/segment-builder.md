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

This section explains how to select an existing audience, when defining the target population of an email delivery. If you want to create a new audience, refer to this [section](segment-builder.md).

This section describes how to create an audience when designing a new email. The segment builder allows you to define the population targeted by your message by filtering data contained in the Adobe Campaign database. If you want to select an existing audience, refer to this [section](add-audience.md). 

For more information on the Segment Builder, refer to the [Segmentation Service documentation](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html?lang=en).

![](assets/segment-builder.png)

## The palette

The palette, located on the left side contains all the elements that you can filter on to create your audience. The tiles contained in the palette must be moved into the center canvas in order to be configured and taken into account. The palette is divided into two tabs:

* **Attributes**: this tab allows you to access all available fields from the schema. The list of fields depends on the targeting schema defined in the email template.

* **Audiences**: this tab allows you to filter using one of the existing audiences defined in the Campaign Classic console.

You can use the search bar to find elements quickly.

## The canvas

The canvas is the central zone in which you can configure and combine rules based on the elements added from the palette. To add a new rule, drag a tile from the palette and drop it onto the canvas. You will then be presented with context-specific options according to the type of data being added. 

## The rule properties pane

On the right side, the **Rule properties** pane allows you to perform the following actions

* View results: displays the list of recipients targeted by the audience
* Code view: displays a code-based version of the audience in PQL.
* Display advanced attributes: check this option if you want to view the complete list of attributes: nodes, groupings, 1-1 links, 1-N links.
* Attributes: displays a description of the created audience.

## Example

In this example, we will build an audience to target all customers living in Atlanta, San Francisco, or Seattle and born after 1980. 

Drag and drop the desired fields from the left pane into the center workspace, then configure them according to your needs.

In this example, we need to rely on Attributes to build the segment:

Attributes: profiles living in Atlanta, San Francisco or Seattle born after 1980

As you are adding and configuring new fields in the workspace, the Segment Properties pane is automatically updated with information on the estimated profiles belonging to the segment.
