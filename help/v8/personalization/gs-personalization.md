---
title: Get started with dynamic content
description: Learn how to make your content dynamic using personalization, conditional content and built-in content blocks.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
---

# Get started with dynamic content

Delivering relevant content to your customers is key to ensure that you appeal to a variety of customers and you play their interest so that your marketing content is read.

To get the most out of every marketing campaign, Adobe Campaign gives you a way to create a custom experience for different groups and individuals by delivering custom dynamic content that speaks to customers on their level by leveraging the information you have gathered about them.

* **Personalize your messages** to each specific recipient by leveraging profile data such as their first name, interests, where they live, what they bought, and much more.

     You can select any field available in the database from the personalization editor related to the recipient, the message or the delivery. These personalization attributes can be inserted in the subject line or the body of your messages. The following syntax inserts the city of the recipient in your content: <%= recipient.location.city %>.

    ![](assets/perso-subject-line.png){width="800" align="center"}

* **Create conditional content** to adapt your deliveries to each recipient and only show the content that is relevant for a given customer based on the information you have about them. This allows you to display specific text blocks and/or images based on conditions. For example, adapt an email banner based on the recipients' subscription to a specific service. 

    ![](assets/condition-sample.png){width="800" align="center"}
    
* **Use personalization blocks** to save time and leverage easily reusable personalizated content into your messages. Campaign comes with a set of personalization blocks which contain a specific rendering that you can insert into your deliveries. For example, you can add a logo, a greeting message, or a link to the mirror page of an email message. Content blocks are available from a dedicated entry in the personalization editor.

    ![](assets/content-blocks.png){width="800" align="center"}

## Access the expression editor {#access}

Adobe Campaign V8 Web provides an expression editor where you can select, arrange, customize and validate all the data to create a customized experience for your content. The expression editor is available for all channels, in every fields with the **[!UICONTROL Open personalization dialog]** icon, such as the subject line field, or email links and text/button content components.

Here are some examples on how to access the expression editor depending on the content that you want make dynamic:

* *Accessing the expression editor from the Sender name field*

    ![](assets/expression-editor-access.png){width="800" align="center"}

* *Accessing the expression editor from an email text component*

    ![](assets/expression-editor-access-email.png){width="800" align="center"}

* *Accessing the expression editor from a link in an email*

    ![](assets/perso-link-insert-icon.png){width="800" align="center"}

>[!NOTE]
>
>In addition to the expression editor, you can also leverage a dedicated conditional content builder when designing an email. [Learn how to build conditional content in emails](conditions.md)

## Let's dive deeper

Now that you have an understanding of how to make your content dynamic, it's time to dive deeper into these documentation sections to start working with the feature.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="personalize.md">
<img alt="Personalize content" src="assets/do-not-localize/dynamic-personalization.jpg">
</a>
<div>
<a href="personalize.md"><strong>Add personalization</strong></a>
</div>
<p>
</td>
<td>
<a href="conditions.md">
<img alt="Lead" src="assets/do-not-localize/dynamic-conditional.jpg">
</a>
<div><a href="conditions.md"><strong>Add conditional content</strong>
</div>
<p>
</td>
<td>
<a href="content-blocks.md">
<img alt="Infrequent" src="assets/do-not-localize/dynamic-content-blocks.jpg">
</a>
<div>
<a href="content-blocks.md"><strong>Add built-in content blocks</strong></a>
</div>
<p></td>
</tr></table>
