---
title: Create conditional content
description: Learn how to define conditions to personalize your content in Adobe Campaign web UI
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
---
# Build conditional content{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Create conditional content"
>abstract="Create conditional content to define dynamic personalization based on the recipient's profile, automatically replacing text blocks and images when certain conditions are met. This feature can take your campaigns to new heights and deliver highly targeted, personalized experiences to your audience."


Conditional content is a powerful feature that allows you to create dynamic personalization based on the recipient's profile, automatically replacing text blocks and images when certain conditions are met. This feature can take your campaigns to new heights and deliver highly targeted, personalized experiences to your audience.

By configuring conditional content fields, you can create advanced dynamic personalization based on the recipient’s profile for example. Text blocks, links, subject line, and/or images are replaced in the message content when a particular condition is satisfied. For example, you can display 'Mr' or 'Mrs' according to the value of the Gender field in Adobe Campaign database, or include a different link based on the recipient preferred language.

## Personalization syntax{#perso-syntax}



## Work with conditions in the personalization editor{#condition-perso-editor}

To define a conditional content for a delivery:

1. Open a delivery and edit the content.
1. Click the **[!UICONTROL Open personalization dialog]** icon, for example, for SMS, on the right of the Message field.

    ![](assets/open-perso-editor-sms.png)

1. In the personalization editor, browse to **[!UICONTROL Helper functions]**.
1. Click the '+' icon next to the **If** function. The following line is added to the central screen:
    `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>``
1. Replace `<FIELD>` by a personalization field. For example, the recipient's company: `recipient.company`.
1. Replace `<VALUE>` by a the value to satisfy. For example, `ADOBE`.




## Sample: conditional SMS subject line{#condition-subject-line}

To create a conditional subject line for a SMS message, follow the steps below:

1. Open a delivery and edit the content.
1. Click the Open personalization dialog icon, on the right of the subject line.
1. In the personalization editor, browse to
1. 

```sql
<% if 
(recipient.email == 'recipient@domain.com' ) 
{ % >
<table>
    <tr>
        <td>variant A</td>
    </tr>
</table>
< % } 
else 
{ % >
<table>
    <tr>
        <td>variant B< td>
    </tr>
</table>
< % } 
%>
```