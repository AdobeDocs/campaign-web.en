---
title: Configure [!DNL Campaign] options
description: Learn how to configure Campaign options and create your own custom options.
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
---
# Configure [!DNL Campaign] options {#options}

>[!CONTEXTUALHELP]  
>id="acw_options_list"  
>title="Options"  
>abstract="Options"  

>[!CONTEXTUALHELP]  
>id="acw_options_create"  
>title="Create option"  
>abstract="Create option"  

Adobe Campaign Web includes technical options that allow you to configure the application more specifically. Some of these options are built-in, while others can be added manually as needed.

>[!IMPORTANT]  
>Built-in options are pre-configured and should only be modified by advanced users. If you have any questions or requests, contact your Adobe representative.

## Access Campaign options {#access}

Options are available from the **[!UICONTROL Administration]** / **[!UICONTROL Options]** menu. Use the filter pane to narrow down the list and quickly locate the option you need.

![](assets/options-list.png)  
[Options list displayed in the Administration / Options menu]

>[!NOTE]  
>Although the options menu location differs between the Adobe Campaign console and Web user interface, the list is identical and operates like a mirror. For more details on the available options, refer to the list of options in [Campaign v7 documentation](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}.

From the options list, you can:

* **Duplicate or delete an option**: Click the ellipsis button and select the desired action.  
* **Modify an option**: Click the option's name to open its properties. Make your changes and save.  
* **Create a custom option**: Click the **[!UICONTROL Create option]** button.  

## Create an option {#create}

The Adobe Campaign Web user interface enables you to create custom options to meet your requirements. This is particularly useful when working with **[!UICONTROL JavaScript code]** workflow activities to store intermediate data.

To create an option:

1. Access the options list and click **[!UICONTROL Create option]**.  
1. Enter a name for the option, select its type, and set the desired value.  
1. Click **[!UICONTROL Create]** to create the option.  

![Create option interface showing fields for name, type, and value](assets/options-create.png)  

Options can act as temporary storage for data, offering the following benefits:

* Typed Values: Options support specific data types, such as dates, integers, strings, etc.
* Flexibility: Options allow users to store and retrieve data efficiently without the overhead of managing database tables.  

In the example below, a custom option named `sampleOption` is created with the initial value "a". A **[!UICONTROL JavaScript code]** activity in a workflow modifies this option's value and stores it in a variable. The updated value is displayed in the workflow logs and reflected in the **[!UICONTROL Options]** menu.

1. Create the option.  

    ![Custom option creation interface showing the name `sampleOption` and initial value "a"](assets/options-sample-create.png)  

1. Configure a **[!UICONTROL JavaScript code]** activity and start the workflow.  

    ![JavaScript code activity configuration interface](assets/options-sample-javascript.png)

1. Run the workflow to see the updated value in the workflow logs.  

    ![Workflow logs showing the updated value of the custom option](assets/options-sample-logs.png)

1. The updated value is now visible in the **[!UICONTROL Options]** menu.  

    ![Options menu displaying the updated value of the custom option](assets/options-sample-updated.png)