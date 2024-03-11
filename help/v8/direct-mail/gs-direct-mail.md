---
audience: end-user
title: Get started with direct mail deliveries
description: Learn how to create and send direct mail deliveries with Adobe Campaign Web
---

# Get started with direct mail deliveries {#gs-direct-mail}

Overview text



Direct mail deliveries let you generate an extraction file which contains data on the target population. You can then share this file with the provider who will deliver messages to the target populations.




Direct mail is an offline channel that allows you to personalize and generate the extraction files required by direct mail providers to send mail to your customers.

When creating a direct mail campaign, Journey Optimizer automatically generates a file containing all the targeted profiles and selected data, such as postal addresses and profile attributes. This file is sent to the server of your choice so that it is accessible by your chosen direct mail provider, who will handle the actual mailing process for you.




Before creating a direct mail message, make sure you have configured:
A file routing configuration which specifies the server where the extraction file should be uploaded and stored,
A direct mail message surface which will reference the file routing configuration.



A type of direct marketing that’s delivered physically to a prospect’s mailbox through the United States Postal Service or other delivery service. Postcards, flyers, and catalogs are common examples. Email marketingis the digital equivalent.

It allows marketer to produce files to mass deliver personalized letters. The recipient profiles must contain at least their names and postal addresses.





A type of direct marketing that’s delivered physically to a prospect’s mailbox through the United States Postal Service or other delivery service. Postcards, flyers, and catalogs are common examples. Email marketing is the digital equivalent.

The Direct mail delivery activity allows you to configure and prepare a file containing profile data that you want to use for a direct mail campaign. This can be a direct mail that is used just once, or it can be a recurring direct mail.

Standard direct mails are sent once.
Recurring mails allow you to send the same direct mail multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.
Context of use
The Direct mail delivery activity is generally used to automate preparing a file that contains profile data. This file can then be sent to a partner/provider in charge of the mailing.

When linked to a scheduler, you can define recurring direct mails.

Direct mail recipients are defined upstream of the activity in the same workflow, via targeting activities such as queries, intersections, etc. Profiles whose mailing address is not specified are automatically excluded when the direct mail is prepared.

The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.









Steps to generate the file are:

Create the delivery
Define the audience: 

The recipient profiles must contain at least their names and postal addresses.

Postal addresses are calculated fields. An address can contain up to six lines by default: the first contains the first name and last name, the next lines contain the postal address (road etc.), and the last line contains the ZIP/Postal code and town or city. The definition of the default calculated postalAddress field can be reviewed in the nms:recipient schema.

An address is considered to be complete if the name, ZIP/Postal code field, and town/city fields are not empty. Any recipients with incomplete addresses will be excluded from direct mail deliveries.



Define the content of the file: Use the extraction wizard to define the information (columns) to be exported into the output file.

Validate the delivery: Check the result of the analysis and the content of the output file.

Start the delivery: Once you validated the extraction file, click Confirm delivery a confirmation message lets you launch the delivery. The confirmation starts the data extraction in the specified file.



regarder infos surp rocess approval : https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-deliveries.html?lang=en#start-an-offline-delivery




To create direct mail deliveries, you have three options:

* **Workflows**: After adding a Direct mail channel activity to your workflow and configuring the basic settings, you can then craft the content of your direct mail deliveries from your right pane menu. For detailed instructions on how to configure workflow, refer to this page.

* **Campaigns**: Once you have created a campaign, you can create a direct mail delivery. For more information on setting up your campaign, refer to this page.

* **Stand-alone deliveries**: Engage customers directly and instantly with individual direct mail delivery, without the need for workflows or campaigns.

<!--<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="create-push.md">
<img alt="Lead" src="assets/do-not-localize/push_create.jpeg">
</a>
<div><a href="create-push.md"><strong>Create a push delivery</strong>
</div>
<p>
</td>
<td>
<a href="content-push.md">
<img alt="Infrequent" src="assets/do-not-localize/push_design.jpeg">
</a>
<div>
<a href="content-push.md"><strong>Design a push delivery<strong></strong></a>
</div>
<p></td>
<td>
<a href="send-push.md">
<img alt="Validation" src="assets/do-not-localize/push_send.jpeg">
</a>
<div>
<a href="send-push.md"><strong>Send a push delivery</strong></a>
</div>
<p>
</td>
<td>
<a href="send-push.md">
<img alt="Validation" src="assets/do-not-localize/push_report.jpeg">
</a>
<div>
<a href="send-push.md"><strong>Push delivery report</strong></a>
</div>
<p>
</td>
</tr></table>-->
