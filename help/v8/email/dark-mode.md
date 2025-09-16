---
title: Switch to dark mode
description: Learn how to use dark mode in the Adobe Campaign Email Designer
feature: Email Design
topic: Content Management
role: User
level: Beginner, Intermediate
keywords: dark mode, email, color, editor
hide: yes
hidefromtoc: yes

---
# Manage dark mode content {#dark-mode}

>[!CONTEXTUALHELP]
>id="ac_edition_darkmode"
>title="Switch to dark mode"
>abstract="Switch to dark mode where you can preview how it may render, and define specific custom settings. <br>The final rendering depends on the recipient's email client. Note that all email clients do not support custom dark mode."

>[!CONTEXTUALHELP]
>id="ac_edition_darkmode_preview"
>title="Switch to dark mode"
>abstract="Switch to dark mode to preview how it may render on supporting email clients. <br>The final rendering depends on the recipient's email client. Note that all email clients do not support dark mode."

When designing your emails, the [!DNL Adobe Campaign] [Email Designer](get-started-email-designer.md) allows you to switch to the **[!UICONTROL Dark mode]** view.

In this <!--Email Designer -->dark mode view, you can also define specific custom settings which will be displayed by the supporting email clients when their dark mode is on.

## What is dark mode? {#what-is-dark-mode}

The way dark mode is rendered in the various email clients is complex. Let's first define dark mode.

Dark mode allows the supporting email clients and apps to display emails with darker backgrounds and lighter colors for text, buttons and other UI elements. It enables to reduce eye strain, save battery life, and improve readability in low-light environments for a more comfortable viewing experience.

As a growing trend across major operating systems and apps<!-- (Apple Mail, Gmail, Outlook, Twitter, Slack)-->, it has become an important consideration in modern email design to ensure content remains legible and visually appealing for all users.

## Guardrails {#guardrails}

The expectations in terms of dark mode rendering must be considered with caution as the way it is applied by the different email clients can vary a lot.

<!--The dark mode final rendering depends on the recipient's email client. It is not possible to guarantee that your email will look the same in dark mode across all devices.-->

Before using dark mode in the [!DNL Adobe Campaign] Email Designer, it is crucial to understand how the main email clients handle it. There are three cases to distinguish:

<!--
* Check out the list of [email clients supporting dark mode](https://www.caniemail.com/search/?s=dark){target="_blank"}

* Learn more on Dark mode in this [Litmus blog post](https://www.litmus.com/blog/the-ultimate-guide-to-dark-mode-for-email-marketers){target="_blank"}
-->

### Clients not supporting dark mode {#not-supporting}

Some email clients do not support this feature at all, such as:

* Yahoo!Mail
* AOL

Whether you define dark mode custom settings or not in the Email Designer, these email clients never display any dark mode rendering. <!--Regardless of whether the interface is in light or dark mode, your email will render the same.-->

### Clients applying their own dark mode {#default-support}

Some email clients systematically apply their own default dark mode for all emails that are received. Colors, backgrounds, images, etc. are automatically adjusted with the dark mode settings specific to the email client, meaning that no external modification is possible.

<!--It is important to note that less than 25% of email clients offer customization options for dark mode. Clients such as Gmail implement their own dark mode rendering, which is not subject to external modification.-->

These clients are for example:

* Gmail (Desktop Webmail, iOS, Android, Mobile Webmail)
* Outloook Windows
* Outlook Windows Mail

In this case, if you define custom dark mode settings in the Email Designer, those settings are overriden with the email client settings.

It is important to understand that these email clients do handle dark mode, but your specific dark mode design will not be rendered.

### Clients supporting custom dark mode {#custom-support}

Other email clients offer the option to render custom dark mode with the `@media (prefers-color-scheme: dark)` query, which is the method used by the [!DNL Journey Optimizer] Email Designer.

Here is a list of the main clients handling this option:

* Apple Mail macOS
* Apple Mail iOS
* Outloook macOS
* Outlook.com
* Outloook iOS
* Outloook Android

In this case, the specific settings you define in the Email Designer should be displayed.

>[!NOTE]
>
>Learn how to define custom dark mode settings with the Email Designer in [this section](#define-custom-dark-mode).

However, some restrictions may apply according to each email client. For example, some clients such as Apple Mail 16 (macOs 13) will not generate dark mode if images are present in the email content.

For optimal results, test your content with the email clients you are targeting. To see a simulation that comes as close as possible to the final result for each client, use the [Email rendering](../preview-test/email-rendering.md) option in the Email Designer.

## Dark mode in the Email Designer {#dark-mode-email-designer}

When it comes to dark mode in the Email Designer, there are two aspects to consider:

* You can get a preview of how the default dark mode will render in most supporting email clients. [Learn more](#preview-dark-mode)

* If you want to override the default settings of email clients [supporting custom dark mode](#custom-support), you can define custom settings for the email you are editing. [Learn more](#define-custom-dark-mode)

### Preview default dark mode {#preview-dark-mode}

To access dark mode in the Email Designer and get a preview of the default dark mode settings, follow the steps below.

1. From the Email Designer home page, select the **[!UICONTROL Design from scratch]** option. [Learn more](create-email-content.md)

1. Add [structures](create-email-content.md) and [content components](content-components.md) to your content.

1. On top right of the central canvas, switch the toggle to **[!UICONTROL Dark mode]**.

    ![](assets/light-mode-toggle.png)

1. The default dark mode preview displays.

    ![](assets/dark-mode-default.png)

By default, the Email Designer dark mode preview applies the 'full color invert' color scheme to all elements except images and icons.

It means that it detects areas with light and dark elements and inverts them, so that light backgrounds become dark and dark text becomes light, whereas dark backgrounds become light and light text becomes dark.

>[!CAUTION]
>
>The final rendering may vary according to the recipient's email client. To see a simulation that comes as close as possible to the final result for each email client, use the [Email rendering](../preview-test/email-rendering.md) option.

### Define custom dark mode {#define-custom-dark-mode}

>[!CONTEXTUALHELP]
>id="ac_edition_darkmode_image"
>title="Use a specific image for dark mode"
>abstract="You can select another image that will display when dark mode is on. <br>Adding a specific image for dark mode does not guarantee it renders correctly in all email clients. Note that all email clients do not support custom dark mode."

After switching to **[!UICONTROL Dark mode]**, you can choose to edit specific styling elements of your content that will be displayed only when dark mode is enabled in the recipient's email client - provided it supports that feature.

>[!WARNING]
>
>The dark mode final rendering depends on each email client, so results can vary from one to another. [Learn more](#guardrails)

<!--
>[!WARNING]
>
>Not all email clients support dark mode. Moreover, some email clients only apply their own default dark mode for all emails that are received. In both cases, the custom settings that you defined in the Email Designer cannot be rendered.-->

To leverage the Email Designer custom dark mode styling, Journey Optimizer uses the<!-- `@media (prefers-color-scheme: dark)` method--> `@media (prefers-color-scheme: dark)` CSS query, which detects if the user's email client is set to dark mode and applies the dark-themed design that was defined in your email.

To define custom dark mode settings, follow the steps below.

1. Make sure you switch to the **[!UICONTROL Dark mode]** preview in the Email Designer. [Learn how](#preview-dark-mode)

1. Edit any styling color attributes such as text, backgrounds, button, etc.

1. You cannot change the colors of images and icons, but you can define specific assets for dark mode only.

    To do so, select any image. Switch to **[!UICONTROL Dark mode]** using the dedicated toggle in the **[!UICONTROL Settings]** pane and select a different asset.

    ![](assets/dark-mode-image.png)

    <!--![](assets/dark-mode-custom.png)-->

1. At any time you can **[!UICONTROL Switch to live view]** in order to check how your content might render on various device sizes. From this view, select the Dark mode toggle on top of the screen to preview the dark mode version of your content across the different devices.

    ![](assets/dark-mode-live-view.png){width="80%" align="center"}

    >[!CAUTION]
    >
    >The live view is a generic preview designed to compare how the rendering might look across various device sizes. The final rendering may vary according to the recipient's email client.

1. Once you are satisfied with the changes for dark mode, click **[!UICONTROL Simulate Content]**.

    ![](assets/dark-mode-simulate.png)

1. Select **[!UICONTROL Render email]** and connect to your Litmus account. You can see the final dark mode rendering for various email clients. Learn more on [Email rendering](../preview-test/email-rendering.md).

    >[!WARNING]
    >
    >While simulation closely approximates how emails will appear in dark mode, actual rendering may differ due to variations in email service providers or device-level settings.

## Best practices {#best-practices}

As dark mode adoption increases across major email clients, it is essential to consider how your emails render in both light and dark environments - whether you are using [custom dark mode](#define-custom-dark-mode) or not.

Dark mode can alter colors, backgrounds, and images — sometimes overriding design choices. To ensure visual consistency, accessibility, and brand integrity, follow the best practices listed below.

**Optimize your images and logos**

* Save logos and icons as PNGs with transparent backgrounds to avoid visible white boxes in dark mode.

* Avoid images with hardcoded white or light backgrounds.

* If transparency is not an option, place images on a solid background in your design to prevent awkward color inversions.

**Watch your backgrounds**

* Ensure sufficient contrast between text and background colors for readability in both light and dark modes.

* Avoid relying on background colors alone for critical content. Some clients override background colors in dark mode, so ensure key information is still visible.

<!--**Inline critical styles**

Inline CSS helps maintain more control over styling, as some clients strip external styles in dark mode.-->

**Design accessible content in dark mode**

<!--KEEP dark mode accessibility best practices IN ONE SINGLE LOCATION - for now listed on this page.
If needed, it can be moved to the Design accessible content page:
The best practices for designing accesible content in dark mode are listed in [this section](accessible-content.md#dark-mode).-->

* Use color combinations easy to distinguish for people with color blindness.

* Use a midtone palette to ensure contrast against both light and dark backgrounds.

* Use accessible color combinations with high contrast to improve readability and meet Web Content Accessibility Guidelines (WCAG) standards. Use tools like WebAIM's Contrast Checker to verify color contrast.

* Avoid thin fonts as it can impact readability. If your brand requires a thin font, bold it in dark mode.

* Skip pure white on pure black as it can cause eye strain and might be automatically inverted by some email clients.

* Provide accessible fallback styling if dark mode is not supported.

**Test your emails in dark mode environment**

* Use the Email Designer's [dark mode preview](#preview-dark-mode) which uses inverted color schemes to spot issues early.

* Use the [Email rendering](../preview-test/email-rendering.md) option that leverages Litmus to simulate your designs across major email clients (Apple Mail, Gmail, Outlook) and see how colors and images behave in dark mode.
