---
audience: end-user
title: Set up and manage the approval process
description: Learn how to manage approvals of marketing campaigns in Campaign Web
feature: Approvals, Campaigns
---
# Manage the approval process {#campaign-approvals}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn6"
>title="Campaign approval management"
>abstract="You can now coordinate stakeholder validation before sending deliveries. Require approvals from marketing managers, data analysts, or other teams for quality control."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"

>[!IMPORTANT]
>
>Approvals are only available for deliveries created inside a campaign. This does not apply to standalone deliveries or deliveries created in workflows outside of a campaign context.

The approval process helps coordinate multiple stakeholders and ensures quality control before deliveries are sent. Use approvals when your organization requires validation from different teams, such as marketing managers reviewing content or data analysts validating target audiences.

When approvals are enabled, you must submit content or target for approval. Designated reviewers receive email notifications requesting validation and can approve or reject directly from the Web UI interface. Deliveries cannot be sent until all required approvals are granted. You can enable:

* **Content approval**: validate message content, design, and personalization
* **Target approval**: validate the audience and targeting criteria
* **Delivery confirmation**: require a final confirmation before sending

## Configure approval settings {#configure-approvals}

Approval settings are inherited from the campaign template and can be modified for individual campaigns. Follow these steps to configure approval settings:

1. Open your campaign or campaign template, or create a new one, from the **[!UICONTROL Campaigns]** menu.

1. Click the **[!UICONTROL Settings]** button at the top right of the campaign dashboard.

1. In the **[!UICONTROL Approvals]** section, configure the following options:

   ![Screenshot showing the campaign approval settings](assets/approvals1.png){zoomable="yes"}

   * **[!UICONTROL Enable content approval]**: when enabled, the delivery content must be approved before sending. Click the folder icon in the **[!UICONTROL Reviewer]** field to select an operator or operator group.

   * **[!UICONTROL Enable target approval]**: when enabled, the delivery target audience must be approved. Click the folder icon in the **[!UICONTROL Reviewer]** field to select an operator or operator group.
   
   * **[!UICONTROL Confirm the delivery before sending]**: requires a final manual confirmation before sending, even after all other approvals are complete.

>[!NOTE]
>
>* If no reviewer is specified, the campaign owner is assigned as reviewer.
>* Reviewers need appropriate permissions to approve deliveries. Only users identified in the reviewer list can approve.

## Submit for approval {#submit-approval}

After creating your delivery, follow these steps to submit content and target for approval.

>[!NOTE]
>Approvals are available both in campaign workflow deliveries and campaign stand-alone deliveries.

1. From the delivery dashboard, click the **[!UICONTROL Submit content]** button. Designated reviewers can approve or reject. See this [section](#approve-reject).

   ![Screenshot showing the Submit content button](assets/approvals2.png){zoomable="yes"}

   The approval status changes to pending in the **[!UICONTROL Properties]** section of the delivery dashboard. See this [section](#rack-approvals). 

1. Once content is approved, click the **[!UICONTROL Prepare]** button to prepare the delivery target. The system prepares the audience and targeting criteria.

1. Click the **[!UICONTROL Submit target]** button. Designated reviewers can then approve or reject. See this [section](#approve-reject).

   ![Screenshot showing the Submit target buttonl](assets/approvals5.png){zoomable="yes"}

   The approval status changes to pending. See this [section](#rack-approvals). 

1. Once the target is approved, the preparation resumes and the delivery can be sent.

>[!NOTE]
>If an approval is rejected, the delivery owner must make all necessary changes to the content or target based on the reviewer's feedback and resubmit for approval.

## Approve or reject {#approve-reject}

Designated reviewers can approve or reject content and target submissions. See this [section](#submit-approval). 

>[!NOTE]
>For the email notification to be sent, the reviewer's address must be configured in the instance.

1. When you receive the notification email, open the delivery that requires approval directly from the Web UI interface.

1. Review the content or target information.

1. Click the **[!UICONTROL Approve content]** or **[!UICONTROL Approve target]** button.

   ![Screenshot showing the Approve content button in the delivery dashboard](assets/approvals3.png){zoomable="yes"}

1. Click **[!UICONTROL Approve]** or **[!UICONTROL Reject]**.

1. Optionally, add a **[!UICONTROL Comment]** to explain your decision. 

   ![Screenshot showing the approval dialog with Approve, Reject buttons and Comment field](assets/approvals4.png){zoomable="yes"}

1. Confirm your decision. The approval status updates immediately in the delivery dashboard. See this [section](#rack-approvals). 

## Track approval status {#track-approvals}

Approval status is visible in the **[!UICONTROL Properties]** section of the delivery dashboard. The status displays which approvals are waiting and their current state:

![Screenshot showing approval status](assets/approvals5.png){zoomable="yes"}

* **[!UICONTROL Being edited]**: the content or target has not been submitted for approval yet
* **[!UICONTROL Pending approval]**: the content or target is awaiting review
* **[!UICONTROL Approved]**: the content or target has been approved by the reviewer  
* **[!UICONTROL Rejected]**: the content or target has been rejected by the reviewer

The approval section shows all enabled approvals and updates in real-time as reviewers validate or reject each step.

## Related topics {#related}

* [Create campaigns](create-campaigns.md)
* [Manage campaigns](manage-campaigns.md)
