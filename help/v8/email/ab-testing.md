---
audience: end-user
title: Create content experiments
description: Learn how to create content experiments in Adobe Campaign Web
exl-id: 476aaaef-c4b2-4007-a050-9b88460435a6
---
# Create content experiments {#content-experiment}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Content experiments - A/B testing"
>abstract="You can now define multiple delivery variants to test which performs best. Vary content, subject, or sender across email elements to determine optimal results."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="See release notes"

## About content experiments {#about-content-experiment}

Content experiments in Adobe Campaign Web allow you to define multiple A/B testing delivery variants in order to measure which performs best for your target audience. You can vary the delivery content, subject, or sender to test different versions and determine which variant produces the best results.

You can conduct A/B tests on various email elements such as:

* **Subject line**: test different email subject lines to see which generates the highest open rate
* **Sender name**: experiment with different sender combinations
* **Email body content**: create multiple content versions to identify which drives the best click-through rate

>[!NOTE]
>
>* Content experiments are currently available for email channel only.
>* A/B testing is not supported for transactional messages.
>* Maximum of 3 treatments (variants) per experiment.

## Create a content experiment {#create-content-experiment}

To add a content experiment to your email delivery, follow these steps:

1. Create an email delivery or open an existing draft delivery. [Learn how to create an email](create-email.md)

1. From the email delivery properties page, click the **[!UICONTROL Create experiment]** button located in the **[!UICONTROL Content]** section.

   ![Screenshot showing the Create experiment button in email properties](assets/ab-testing-1.png){zoomable="yes"}

## Configure the experiment settings {#configure-experiment}

Configure your experiment using the following sections:

![Screenshot showing the Experiment settings](assets/ab-testing-2.png){zoomable="yes"}

### Audience settings {#audience-settings}

Define the percentage of your target population that will receive the experiment variants.

Enter a value to set the audience size. This represents the proportion of recipients who will receive one of the experiment variants during the test phase.

* **Minimum**: 1%
* **Maximum**: 100%
* **Default**: 10%

The remaining audience (90% by default) will receive the winning variant once the experiment concludes and a winner is determined.

For example, with a target audience of 10,000 recipients and an audience size of 10%, 1,000 recipients will be randomly selected to participate in the experiment. The remaining 9,000 recipients will receive the winning variant after the experiment ends.

### Winning strategy {#winning-strategy}

Select the metric that will be used to determine the winning variant:

* **[!UICONTROL Best open rate]** (default): the variant with the highest percentage of email opens wins
* **[!UICONTROL Best click-through rate]**: the variant with the highest percentage of clicks in the email wins  
* **[!UICONTROL Weakest unsubscription rate]**: the variant with the lowest percentage of unsubscribes wins

The system automatically tracks these metrics during the experiment and calculates which variant performs best according to your selected criterion.

### Winner sending method {#sending-method}

Define how long the experiment should run and select the sending method:

1. Enter the duration value in hours. The experiment will run for this period before determining the winning variant.

   * **Minimum**: 3 hours
   * **Maximum**: 240 hours (10 days)
   * **Default**: 24 hours

   >[!NOTE]
   >
   >Ensure your experiment duration is long enough to collect meaningful data. A short duration may not provide sufficient statistical significance, especially for metrics like click-through rate that may take longer to accumulate.

1. Choose how the winning variant should be sent to the remaining population:

   * **[!UICONTROL Automatic sending]** activated: the system automatically sends the winning variant to the remaining audience once the experiment ends.
   * **[!UICONTROL Automatic sending]** deactivated: you must manually click the **[!UICONTROL Send]** button to send the winning variant after reviewing the experiment results.

If no variant achieves significantly better results than the others by the end of the experiment, the system sends the first variant to the remaining population. See this [section](#send-deliveries).

## Define the content treatments {#define-content}

After saving your experiment settings, a first treatment is created by default. You now need to add your other treatments (up to three) and define their specific content.

1. From the delivery properties, click **[!UICONTROL Edit content]**. Treatments are displayed on the left side. 

   ![Screenshot showing the content experiments panel](assets/ab-testing-3.png){zoomable="yes"}

1. Click the **[!UICONTROL Add treatment]** button and define its name. Repeat this operation for all the treatments you need to add. You can then change their name, duplicate and remove them.

1. Click on each treatment and customize the following items:

   * **Sender name**: Customize who the email appears to be from
   * **Subject line**: Write a unique subject line for each treatment
   * **Email body**: Design different content versions using the Email Designer

   ![Screenshot showing several treatments](assets/ab-testing-4.png){zoomable="yes"}

1. Preview each treatment by clicking on the treatment and then clicking **[!UICONTROL Simulate content]**.

## Start the experiment and monitor results {#validate-start}

Once you've defined all your content treatments, you can validate and start the experiment.

1. From the delivery properties, click **[!UICONTROL Review and send]**, then click **[!UICONTROL Prepare]**.

1. Then click **[!UICONTROL Start experimentation]** to begin the A/B test.

   ![Screenshot showing the start experimentation button](assets/ab-testing-5.png){zoomable="yes"}

1. Once your experiment is running, monitor the different metrics displayed in the delivery dashboard.

As the experiment runs, you can click **[!UICONTROL Stop sending]** to end the experiment. You can also decide to send manually before the end of the experiment by clicking **[!UICONTROL Select and send to winner]**.

>[!NOTE]
>
>Results are updated in near real-time as recipients interact with your email. However, early results may not have statistical significance - it's recommended to wait until the experiment duration is complete before making final decisions.

## Send the deliveries {#send-deliveries}

Sending can be performed automatically or manually, according to what you chose in the **[!UICONTROL Winner sending method]** settings. See this [section](#sending-method).

### Automatic sending {#automatic-sending}

For automatic sending, the system analyzes the results based on your winning strategy and determines the winning treatment. The winning treatment is automatically sent to the remaining audience. If no clear winner emerged, the first variant is chosen.

### Manual sending {#manual-sending}

If you configured manual sending, review the results when the experiment ends and click **[!UICONTROL Send]** to send the winning treatment. If no clear winner emerged, the first treatment is selected by default but you can choose a different one.

## View final results {#final-results}

After your experiment completes and the delivery is fully sent, you can access comprehensive reports:

1. From the delivery dashboard, click **[!UICONTROL Reports]**.

1. Navigate to the **[!UICONTROL Experiments]** report tab to display the key performance metrics for each treatment.

## Best practices {#best-practices}

When creating content experiments, consider these recommendations:

* **Test one element at a time**: For clearest results, test variations of a single element (e.g., subject line only, or content only) rather than multiple elements simultaneously.

* **Choose appropriate duration**: Allow enough time for statistical significance:
   * For open rate tests: 12-24 hours is usually sufficient
   * For click-through rate tests: 24-48 hours or more may be needed
   * Larger audiences may require less time; smaller audiences may need longer

* **Size your audience appropriately**: 
   * Ensure your experiment audience (the percentage allocated to testing) is large enough to produce meaningful results
   * General guideline: Minimum of 1,000 recipients per treatment for reliable results

* **Test regularly but not excessively**: Conduct experiments on important campaigns, but avoid testing every single send to focus resources on impactful decisions.

* **Document your learnings**: Keep records of experiment results to inform future campaign strategies.

## Related topics {#related-topics}

* [Create your first email](create-email.md)
* [Configure email content](edit-content.md)
* [Preview and send an email](../monitor/prepare-send.md)
* [Email delivery reports](../reporting/email-report.md)
