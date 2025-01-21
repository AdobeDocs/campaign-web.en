---
title: How to make your content dynamic?
description: Learn how to make your content dynamic using personalization and conditional content.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
---
# How to make your content dynamic? {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personalization"
>abstract="The personalization editor allows you to select, arrange, customize and validate all the data to create a customized experience for your content. You can personalize your messages to each recipient by leveraging profile data, and create conditional content to adapt your message to each recipient and only show the content that is relevant."

As a marketer, it is crucial to target customers who are genuinely interested in your offerings and to engage themby providing effective and relevant content. Given the diverse range of recipients you encounter, creating multiple pieces of marketing content to appeal to different people can be time-consuming and wasteful. This is where dynamic content comes into play.

Adobe Campaign Web dynamic content capabilities allows you to customize your content based on the information you have gathered about your recipients. By utilizing dynamic content, you ensure that your marketing efforts are more relevant, avoiding marketing unwanted or unnecessary products or services. This approach makes your content more appealing and increases the likelihood of it being read. Moreover, it enables you to personalize your content, making recipients feel like they are receiving information from a person rather than a machine.

## How to make your content dynamic? {#make-content-dyn}

You can make your message content dynamic by inserting JavaScript constructs in Campaign Web expression editor. At message sending, those expressions are interpreted by Adobe Campaign in order to deliver the correct content to each of your recipients:

* **Personalize your messages** to each specific recipient by leveraging profile data such as their first name, interests, where they live, what they bought, and much more. You can select any field available in the database from the personalization editor related to the recipient, the message or the delivery. These personalization attributes can be inserted in the subject line or the body of your messages. The following syntax inserts the city of the recipient in your content: <%= recipient.location.city %>.

    ![](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **Create conditional content** to adapt your deliveries to each recipient and only show the content that is relevant for a given customer based on the information you have about them. This allows you to display specific text blocks and/or images based on conditions. For example, adapt an email banner based on the recipients' subscription to a specific service. 

    ![](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

## Access the expression editor {#access}

Adobe Campaign Web provides an expression editor where you can select, arrange, customize and validate all the data to create a customized experience for your content. The expression editor is available for all channels, in every fields with the **[!UICONTROL Open personalization dialog]** icon, such as the subject line field, or email links and text/button content components.

Here are some examples on how to access the expression editor depending on the content that you want make dynamic:

* *Accessing the expression editor from the Sender name field*

    ![](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *Accessing the expression editor from an email text component*

    ![](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *Accessing the expression editor from a link in an email*

    ![](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>In addition to the expression editor, you can also leverage a dedicated conditional content builder when designing an email. [Learn how to build conditional content in emails](conditions.md)
