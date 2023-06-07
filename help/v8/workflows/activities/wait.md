---
audience: end-user
title: Use the Wait workflow activity
description: Learn how to use the Wait workflow activity
badge: label="Alpha" type="Positive"
---

# Wait {#wait}

The **Wait** activity is a **Flow control** activity. It is used to allow a certain amount of time to pass between two activities being executed. For example, to wait several days after an email delivery activity then analyze the opens and clicks generated during this period before performing any follow-up operations (reminder email, creating an audience, etc.).

## Configuration

Follow these steps to configure the **Wait** activity:

1. Add a **Wait** activity into your workflow.

1. Specify the **Duration** of the wait between the inbound and outbound transitions.

1. Select the time unit in the **Periods** field: seconds, minutes, hours. 

## Example

The following example illustrates the **Wait** activity in a typical use case. An email invitation to an event is sent. 24 hours after it was sent, an SMS delivery is sent to the same population.

![](../assets/workflow-wait-example.png)
