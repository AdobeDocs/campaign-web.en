---
audience: end-user
title: Set up and manage the approval process
description: Learn how to manage approvals of marketing campaigns in Campaign Web
feature: Approvals, Campaigns
exl-id: 8140f904-ec0a-44e1-981f-0e050d3c9cdb
TQID: https://experienceleague.adobe.com/Gpk7fY-VSFdgvgJo2STGjJ8-mHBkVZnp8cD-bFZrWpU
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
---
# Manage the approval process {#campaign-approvals}

>[!IMPORTANT]
>
>Approvals are only available for campaigns and deliveries created inside a campaign.

The approval process helps coordinate multiple stakeholders and ensures quality control before deliveries are sent. Use approvals when your organization requires validation from different teams, such as marketing managers reviewing content or data analysts validating target audiences.

When approvals are enabled, you must submit content or target for approval. Designated reviewers receive email notifications requesting validation and can approve or reject directly from the Web UI interface. Deliveries cannot be sent until all required approvals are granted. You can enable:

* **Content approval**: validate message content, design, and personalization. You can add an editing step before content approval, handled by a designated operator, and an approval step for an external reviewer once the content is internally approved.
* **Target approval**: validate the audience and targeting criteria
* **Budget approval**: validate the delivery budget
* **Delivery start**: restrict who can start sending the delivery to a specific reviewer
* **Delivery confirmation**: require a final confirmation before sending

## Configure approval settings {#configure-approvals}

Approval settings are inherited from the campaign template and can be modified for individual campaigns. The same **[!UICONTROL Approvals]** section is also available in the settings of a delivery created inside a campaign, letting you override the campaign-level configuration for that delivery only.

Follow these steps to configure approval settings at the campaign level:

1. Open your campaign or campaign template, or create a new one, from the **[!UICONTROL Campaigns]** menu.

1. Click the **[!UICONTROL Settings]** button at the top right of the campaign dashboard. 

1. In the **[!UICONTROL Approvals]** section, configure the following options:

   ![Screenshot showing the campaign approval settings](assets/approvals1.png){zoomable="yes"}

   >[!NOTE]
   >
   > If you decide to enable an approval option, click the folder icon in the **[!UICONTROL Reviewer]** field to select an operator or operator group.

1. Configure **[!UICONTROL Content approval]**: when enabled, the delivery content must be approved before sending. When this option is enabled, two fields are displayed:

   * **[!UICONTROL Assign content editing]**: adds an editing step before content approval. A designated operator, such as a webmaster, is notified to edit the content, then makes it available for approval.
   * **[!UICONTROL External content approval]**: adds an approval step for an external reviewer, such as a partner or supplier, who validates the rendering of the delivery (for example brand consistency) once the content is internally approved.

1. Define the **[!UICONTROL Target approval]**: when enabled, the delivery target audience must be approved.

1. Set the **[!UICONTROL Budget approval]**: when enabled, the delivery budget must be approved. This option requires a budget to already be assigned to the campaign, which is currently done from the Client Console.

1. Set the **[!UICONTROL Delivery start]**: restrict the delivery start to a specific operator or operator group. If a non-authorized operator tries to send the delivery, they see an error indicating they are not authorized to perform this action.

1. Set the **[!UICONTROL Confirm the delivery before sending]**: requires a final manual confirmation before sending, even after all other approvals are complete.

>[!NOTE]
>
>* If no reviewer is specified, the campaign owner is assigned as reviewer.
>* Reviewers need appropriate permissions to approve deliveries. Only users identified in the reviewer list can approve.

## Submit for approval {#submit-approval}

After creating your delivery, follow these steps to submit content and target for approval.

>[!NOTE]
>
>Approvals apply whether the delivery was created directly in the campaign or through a campaign workflow.

1. From the delivery dashboard, click the **[!UICONTROL Submit content]** button. Designated reviewers can approve or reject. See this [section](#approve-reject).

   ![Screenshot showing the Submit content button](assets/approvals2.png){zoomable="yes"}

   The approval status changes to pending in the **[!UICONTROL Properties]** section of the delivery dashboard. See this [section](#track-approvals). 

1. Once content is approved, click the **[!UICONTROL Prepare]** button to prepare the delivery target. The system prepares the audience and targeting criteria.

1. Click the **[!UICONTROL Submit target]** button. Designated reviewers can then approve or reject. See this [section](#approve-reject).

   ![Screenshot showing the Submit target button](assets/approvals5.png){zoomable="yes"}

   The approval status changes to pending. See this [section](#track-approvals). 

1. If budget approval is enabled, submit the budget for approval following the same principle. Designated reviewers can approve or reject. See this [section](#approve-reject).

1. Once the target and, if applicable, the budget are approved, the preparation resumes and the delivery can be sent.

>[!NOTE]
>If an approval is rejected, the delivery owner must make all necessary changes to the content or target based on the reviewer's feedback and resubmit for approval.

## Approve or reject {#approve-reject}

Designated reviewers can approve or reject content, target, and budget submissions. See this [section](#submit-approval). 

>[!NOTE]
>For the email notification to be sent, the reviewer's address must be configured in the instance.

1. When you receive the notification email, open the delivery that requires approval directly from the Web UI interface.

1. Review the content or target information.

1. Click the **[!UICONTROL Approve content]**, **[!UICONTROL Approve target]**, or **[!UICONTROL Approve budget]** button.

   ![Screenshot showing the Approve content button in the delivery dashboard](assets/approvals3.png){zoomable="yes"}

1. Click **[!UICONTROL Approve]** or **[!UICONTROL Reject]**.

1. Optionally, add a **[!UICONTROL Comment]** to explain your decision. 

   ![Screenshot showing the approval dialog with Approve, Reject buttons and Comment field](assets/approvals4.png){zoomable="yes"}

1. Confirm your decision. The approval status updates immediately in the delivery dashboard. See this [section](#track-approvals). 

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
