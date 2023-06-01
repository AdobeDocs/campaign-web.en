---
audience: end-user
title: Use the Wait workflow activity
description: Learn how to use the Wait workflow activity
badge: label="Alpha" type="Positive"
---

# Wait {#wait}

The **Wait** activity momentarily suspends executing a part of a workflow. It activates its outbound transition after a delay that may range from a few seconds to several months, which executes the activities placed afterwards.

The **Wait** activity is used to allow a certain amount of time to pass between two activities being executed. For example, to wait several days after an email delivery activity then analyze the opens and clicks generated during this period before performing any follow-up operations (reminder email, creating an audience, etc.).

## Configuration

Follow these steps to configure the **Wait** activity:

1. Add a **Wait** activity into your workflow.

1. Specify the **Duration** of the wait between when the inbound and outbound transitions of the activity are activated.

1. Select the time unit **Period**: seconds, minutes, hours. 

## Example


