---
title: Work with dynamic JavaScript pages
description: Learn how to work with dynamic JavaScript pages.
exl-id: b7de9f55-2aef-4ba9-a2a1-e9ca15deacfb
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Work with dynamic JavaScript pages {#dynamic-javascript-pages}

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_list"
>title="Dynamic JavaScript pages"
>abstract="Dynamic JavaScript pages (JSSP) let you build server-side pages that generate dynamic content when accessed through a URL, such as custom APIs, exports, or web application logic. From this list, you can create, modify, duplicate, or delete a dynamic JavaScript page."

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_create"
>title="Create Dynamic JavaScript page"
>abstract="Define a namespace, name, and label for your dynamic JavaScript page, then write its content using JavaScript code. Once created, the namespace and name cannot be modified."

## About dynamic JavaScript pages {#about}

Dynamic JavaScript pages (JSSP) let you build server-side pages that generate dynamic content when accessed through a URL, such as custom APIs, exports, or web application logic. These pages are stored in the **[!UICONTROL Administration]** > **[!UICONTROL Dynamic JavaScript pages]** menu in the left navigation pane.

![Dynamic JavaScript pages list interface showing available options](assets/dynamic-javascript-pages.png)

From the dynamic JavaScript pages list, you can:

* **Duplicate or delete a page**: Click the ellipsis button, and select the desired action.
* **Modify a page**: Click a page's name to open its properties, make your changes, and save.
* **Create a new dynamic JavaScript page**: Click the **[!UICONTROL Create Dynamic JavaScript page]** button.

<!--
>[!NOTE]
>
>In the Campaign console, dynamic JavaScript pages are available under **[!UICONTROL Administration]** > **[!UICONTROL Configuration]** > **[!UICONTROL Dynamic JavaScript pages]**. Although the menu location differs from the Web user interface, the list is identical and operates like a mirror.
-->

## Create a dynamic JavaScript page {#create}

To create a dynamic JavaScript page, follow these steps:

1. Navigate to the **[!UICONTROL Dynamic JavaScript pages]** menu, and click the **[!UICONTROL Create Dynamic JavaScript page]** button.

1. Define the page's properties:

    * **[!UICONTROL Namespace]**: Specify the namespace relevant to your custom resources. By default, the namespace is "cus", but it may vary depending on your implementation.
    * **[!UICONTROL Name]**: The unique identifier used to reference the page.
    * **[!UICONTROL Label]**: The descriptive label displayed in the dynamic JavaScript pages list.

    ![Dynamic JavaScript page creation interface showing namespace, name, and label fields](assets/dynamic-javascript-pages2.png)

    >[!NOTE]
    >
    >Once created, the **[!UICONTROL Namespace]** and **[!UICONTROL Name]** fields cannot be modified. To make changes, duplicate the page and update as needed.

1. Click the **[!UICONTROL Create code]** button to define the page's content, then write your JSSP code using `<%@ page %>` directives and `NL.require()` calls to load core libraries.

    ![Dynamic JavaScript page code editor](assets/dynamic-javascript-pages4.png)

1. Click **[!UICONTROL Confirm]** to save your code.

1. When your dynamic JavaScript page is ready, click **[!UICONTROL Create]**. The page is now accessible at a URL built from its namespace and name, in the format `https://<your-instance>/<namespace>/<name>`. For example, a page named `recipientAPI.jssp` in the `cus` namespace is accessible at `https://<your-instance>/cus/recipientAPI.jssp`.

For more information on reusable JavaScript functions, refer to [Work with JavaScript codes](javascript-codes.md).
