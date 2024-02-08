---
title: Define landing page-specific content
description: Learn how to design landing page specific content in Campaign Web
feature: Landing Pages
badge: label="Limited Availability" 

---
# Define landing page-specific content {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Use content components"
>abstract="Content components are empty content placeholders that you can use to create the layout of a landing page. To define specific content that will enable users to select and submit their choices, use the form component."

When editing the content of any page of your landing page, it is already pre-filled.

The first page, which is immediately displayed to the users after they click the link to your landing page, is already pre-filled with the [landing page-specific form component](#use-form-component) for the selected template to enable users to select and submit their choices. You can also define [landing page-specific styles](#lp-form-styles).

To further design your landing page content, you can use the same components as for an email. [Learn more](../email/content-components.md#add-content-components)

The content of the **[!UICONTROL Confirmation]**, **[!UICONTROL Error]** and **[!UICONTROL Expiration]** pages is also pre-filled. Edit them as needed.

## Use the form component {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Set the form component fields"
>abstract="Define how your recipients will see and submit their choices from your landing page."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="What happens when clicking the button"
>abstract="Define what will happen upon users submitting the landing page form."

To define specific content that will enable users to select and submit their choices from your landing page, use the **[!UICONTROL Form]** component. To do so, follow the steps below.

1. The landing page-specific **[!UICONTROL Form]** component is already displayed in the canvas for the selected template.

    >[!NOTE]
    >
    >The **[!UICONTROL Form]** component can only be used once on the same page.

1. Select it. The **[!UICONTROL Form content]** tab displays in the right palette to let you edit the different fields of the form.

    ![](assets/lp-form-component.png)

    >[!NOTE]
    >
    >Switch to the **[!UICONTROL Styles]** tab at any time to edit the styles of your form component content. [Learn more](#lp-form-styles)

1. Expand the first text field. From the **[!UICONTROL Text field 1]** section, you can edit the field type, the field from the database, the label, and the text that will be displayed inside the field before the user fills in the field.

    ![](assets/lp-form-text-field.png)

1. Check the **[!UICONTROL Make form field mandatory]** option if needed. In that case, the landing page can only be submitted if the user has filled in this field.

    >[!NOTE]
    >
    >If a mandatory field is not filled in, an error message will display when the user submits the page.

1. Add a checkbox. Select if that checkbox should update a service or a field from the database.

    ![](assets/lp-form-checkbox.png)

    Define if this checkbox is to opt users in or out. Select amongst the two options below:

    * **[!UICONTROL Subscribe in if checked]**: Users need to check the box to consent (opt-in).
    * **[!UICONTROL Unsubscribe if checked]**: Users need to check the box to remove their consent (opt-out).

1. You can delete and add as many text fields and/or checkboxes as needed.

1. Once you added all the desired checkboxes and/or text fields, click **[!UICONTROL Call to action]** to expand the corresponding section. It enables you to define the behavior of the button in the **[!UICONTROL Form]** component.

    ![](assets/lp-call-to-action.png)

1. Define what will happen upon clicking the button:

    * **[!UICONTROL Confirmation page]**: The user will be redirected to the **[!UICONTROL Confirmation]** page set for the current landing page.

    * **[!UICONTROL Redirect URL]**: Enter the URL of the page the users will be redirected to.

1. If you want to make additional updates upon submitting the form, select **[!UICONTROL Additional updates]**, choose **[!UICONTROL Opt in]** or **[!UICONTROL Opt out]**, and define if you want to update a subscription list, the channel or just the email address used.

    ![](assets/lp-form-additionnal-updates.png)

1. Save your content to go back to the [landing page properties](create-lp.md).

## Define landing page form styles {#lp-form-styles}

1. To modify the styles of your form component content, switch at any time to the **[!UICONTROL Style]** tab.

    ![](assets/lp_designer-form-style.png)

1. The **[!UICONTROL Fields]** section is expanded by default and enables you to edit the appearance of the text field, such as the label and placeholder font, the position of the label, the field background color, or the field border.

    ![](assets/lp_designer-form-style-fields.png)

1. Expand the **[!UICONTROL Checkboxes]** section to define the appearance of the checkboxes and corresponding text. For example, you can adjust the font family or size, or the checkbox border color.

    ![](assets/lp_designer-form-style-checkboxes.png)

1. Expand the **[!UICONTROL Buttons]** section to modify the appearance of the button in the component form. For example, you can change the font, add a border, edit the label color on hover, or adjust the alignment of the button.

    ![](assets/lp_designer-form-style-buttons.png)

    You can preview some of your settings such as button label color on hover by using the **[!UICONTROL Simulate content]** button. Learn more on testing landing pages [here](create-lp.md#test-landing-page).

1. Expand the **[!UICONTROL Form layout]** section to edit the layout settings such as the background color, padding, or margin.

    ![](assets/lp_designer-form-style-layout.png)

<!--
1. Expand the **[!UICONTROL Form error]** section to adjust the display of the error message that displays in case a problem occurs. Check the corresponding option to preview the error text on the form.

    ![](assets/lp_designer-form-error-preview.png)-->

