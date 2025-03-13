---
audience: end-user
title: Edit the email content
description: Learn how to start building your content using the Email Designer in Campaign Web user interface
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
---
# Get started with the Email Designer {#get-started-email-designer}


Once you have created an email in Adobe Campaign, you need to define its content.

The Email Designer enables you to create captivating, individually tailored emails through an intuitive drag-and-drop interface. Whether you're starting from a blank slate, importing an existing content or leveraging existing templates, design and refine all content for every email, whether promotional or transactional.

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* Use [!DNL Campaign] email designing capabilities to easily build responsive emails. [Learn more](create-email-content.md)

* Enhance customers' experience by creating personalized based on their profile attributes. [Learn more](../personalization/personalize.md)

* Configure conditional content fields to create dynamic personalization based on the recipient's profile. [Learn more](../personalization/conditions.md)

## Email design best practices {#best-practices}

When sending emails, it's important to consider that recipients may forward them, which can sometimes cause issues with the email's rendering. This is particularly true when using CSS classes that may not be supported by the email provider used for forwarding, for example, if you're using the "is-desktop-hidden" CSS class to hide an image on mobile devices.

To minimize these rendering issues, we recommend keeping your email design structure as simple as possible. Try to use a single design that works well for both desktop and mobile devices, and avoid using complex CSS classes or other design elements that may not be fully supported by all email clients. When using images in your emails, avoid images that are larger than 2 MB or use encoded image links.

By following these best practices, you can help ensure that your emails are consistently rendered correctly, regardless of how they are viewed or forwarded by recipients.

## Start authoring your content {#start-authoring}

From the email delivery dashboard, go through the [Edit content](edit-content.md) screen to open the Email Designer home page. From there, choose how you want to design your email from the following options:

* **Design your email from scratch** through the email designer's interface. Learn how to design your email content in [this section](create-email-content.md).

* **Code or paste raw HTML** directly in the email designer. Learn how to code your own content in [this section](code-content.md).

* **Import existing HTML content** from a file or a .zip folder. Learn how to import an email content in [this section](existing-content.md).

* **Select an existing content** from a list of built-in or custom templates. Learn how to work with email templates [this section](create-email-templates.md).

    ![](assets/email_designer_create_options.png){zoomable="yes"}
