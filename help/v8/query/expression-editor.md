---
audience: end-user
title: Build your first query using the query modeler
description: Learn how to build your first query in Adobe Campaign Web query modeler.
exl-id: f9a365ac-c8be-423f-a99d-40ad5492223c
---
The content has been reviewed and formatted according to the specified rules. Below is the updated documentation:

---

# Edit expressions {#expression}

Editing an expression involves manually entering conditions to form a rule. This mode allows you to use advanced functions, which let you manipulate the values used to carry out specific queries, such as manipulating dates, strings, numerical fields, and sorting.

>[!IMPORTANT]
>
>The section below provides information on how to work with the expression editor to build rules. Keep in mind that the syntax used to build rules differs from the one used to add personalization.

## Work with the expression editor {#edit}

The expression editor is available from the query modeler **[!UICONTROL Edit expression]** button, available for the **[!UICONTROL Attribute]** and **[!UICONTROL Value]** fields when configuring a custom condition.

| Access from the **Attribute** field | Access from the **Value** field |
| --- | --- |
| ![Expression editor for Attribute field](assets/expression-editor-attribute.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} | ![Expression editor for Value field](assets/edit-expression.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |

The expression editor provides:

* An **input field (1)** where the expression is defined.
* A list of available **fields (2)** that can be used in the expression and correspond to the targeting dimension of the query.
* **Helper functions (3)**, sorted by category.

Edit the expression by entering an expression directly in the input field. To add a field or a helper function, place your cursor in the expression where you want to add it and click the + button.

![Expression editor interface](assets/expression-editor.png){zoomable="yes"}

When your expression is ready, click the **[!UICONTROL Confirm]** button. The expression displays in the selected field. To edit it, open the expression editor and make the desired changes.

The example below shows an expression configured for the **[!UICONTROL Value]** field. To edit it, open the expression editor using the **[!UICONTROL Edit expression]** button.

![Example of editing expression for Value field](assets/edit-expression-value.png){zoomable="yes"}

## Helper functions

The query editing tool allows you to use advanced functions to carry out complex filtering depending on the desired results and the types of manipulated data. The following functions are available:

### Aggregate

Aggregate functions perform calculations on a set of values.

<table>
<tbody>
<tr>
<td><strong>Name</strong></td>
<td><strong>Description</strong></td>
<td><strong>Syntax</strong></td>
</tr>
<tr>
<td><strong>Avg</strong></td>
<td>Returns the average of a number type column</td>
<td>Avg(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>Count</strong></td>
<td>Counts the non-null values of a column</td>
<td>Count(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>CountAll</strong></td>
<td>Counts the values returned (all fields)</td>
<td>CountAll()</td>
</tr>
<tr>
<td><strong>Countdistinct</strong></td>
<td>Counts the distinct non-null values of a column</td>
<td>Countdistinct(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>Max</strong></td>
<td>Returns the maximum value of a number, string, or date type column</td>
<td>Max(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>Min</strong></td>
<td>Returns the minimum value of a number, string, or date type column</td>
<td>Min(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>StdDev</strong></td>
<td>Returns the standard deviation of a number, string, or date column</td>
<td>StdDev(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>StringAgg</strong></td>
<td>Returns the concatenation of the values of a string type column, separated by the character in the second argument</td>
<td>StringAgg(&lt;Value&gt;, &lt;String&gt;)</td>
</tr>
<tr>
<td><strong>Sum</strong></td>
<td>Returns the sum of the values of a number, string, or date type column</td>
<td>Sum(&lt;value&gt;)</td>
</tr>
</tbody>
</table>

### Date

Date functions manipulate date or time values.

<table>
<tbody>
<tr>
<td><strong>Name</strong></td>
<td><strong>Description</strong></td>
<td><strong>Syntax</strong></td>
</tr>
<tr>
<td><strong>AddDays</strong></td>
<td>Adds a number of days to a date</td>
<td>AddDays(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>AddHours</strong></td>
<td>Adds a number of hours to a date</td>
<td>AddHours(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>AddMinutes</strong></td>
<td>Adds a number of minutes to a date</td>
<td>AddMinutes(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>AddMonths</strong></td>
<td>Adds a number of months to a date</td>
<td>AddMonths(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>AddSeconds</strong></td>
<td>Adds a number of seconds to a date</td>
<td>AddSeconds(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>AddYears</strong></td>
<td>Adds a number of years to a date</td>
<td>AddYears(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>ConvertNTZ</strong></td>
<td>Converts timestamp NTZ (timestamp without timezone) into TZ (timestamp with timezone) applying defined session TZ</td>
<td>ConvertNTZ(&lt;date+time&gt;)</td>
</tr>
<tr>
<td><strong>DateCmp</strong></td>
<td>Compares two dates</td>
<td>DateCmp(&lt;date&gt;, &lt;date&gt;)</td>
</tr>
<tr>
<td><strong>DateOnly</strong></td>
<td>Returns the date only (with time at 00:00)</td>
<td>DateOnly(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>Day</strong></td>
<td>Returns the number representing the day of the date</td>
<td>Day(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>DayOfYear</strong></td>
<td>Returns the number of the day in the year of the date</td>
<td>DayOfYear(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>DaysAgo</strong></td>
<td>Returns the date corresponding to the current date minus n days</td>
<td>DaysAgo(&lt;number&gt;)</td>
</tr>
<tr>
<td><strong>DaysAgoInt</strong></td>
<td>Returns the date (integer yyyymmdd) corresponding to the current date minus n days</td>
<td>DaysAgoInt(&lt;number&gt;)</td>
</tr>
<tr>
<td><strong>DaysDiff</strong></td>
<td>Returns the number of days between two dates</td>
<td>DaysDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>DaysOld</strong></td>
<td>Returns the age in days of a date</td>
<td>DaysOld(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>GetDate</strong></td>
<td>Returns the current system date of the server</td>
<td>GetDate()</td>
</tr>
<tr>
<td><strong>Hour</strong></td>
<td>Returns the hour of the date</td>
<td>Hour(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>HoursDiff</strong></td>
<td>Returns the number of hours between two dates</td>
<td>HoursDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>Minute</strong></td>
<td>Returns the minutes of the date</td>
<td>Minute(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>MinutesDiff</strong></td>
<td>Returns the number of minutes between two dates</td>
<td>MinutesDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>Month</strong></td>
<td>Returns the number representing the month of the date</td>
<td>Month(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>MonthsAgo</strong></td>
<td>Returns the date corresponding to the current date minus n months</td>
<td>MonthsAgo(&lt;number&gt;)</td>
</tr>
<tr>
<td><strong>MonthsDiff</strong></td>
<td>Returns the number of months between two dates</td>
<td>MonthsDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>MonthsOld</strong></td>
<td>Returns the age in months of a date</td>
<td>MonthsOld(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>Oldest</strong></td>
<td>Returns the oldest date in a range</td>
<td>Oldest(&lt;date, date&gt;)</td>
</tr>
<tr>
<td><strong>Second</strong></td>
<td>Returns the seconds of the date</td>
<td>Second(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>SecondsDiff</strong></td>
<td>Returns the number of seconds between two dates</td>
<td>SecondsDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>SubDays</strong></td>
<td>Subtracts a number of days from a date</td>
<td>SubDays(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>SubHours</strong></td>
<td>Subtracts a number of hours from a date</td>
<td>SubHours(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>SubMinutes</strong></td>
<td>Subtracts a number of minutes from a date</td>
<td>SubMinutes(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>SubMonths</strong></td>
<td>Subtracts a number of months from a date</td>
<td>SubMonths(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>SubSeconds</strong></td>
<td>Subtracts a number of seconds from a date</td>
<td>SubSeconds(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>SubYears</strong></td>
<td>Subtracts a number of years from a date</td>
<td>SubYears(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>ToDate</strong></td>
<td>Converts a date + time as a date</td>
<td>ToDate(&lt;date + time&gt;)</td>
</tr>
<tr>
<td><strong>ToDateTime</strong></td>
<td>Converts a string to a date + time</td>
<td>ToDateTime(&lt;string&gt;)</td>
</tr>
<tr>
<td><strong>ToTimestamp</strong></td>
<td>Converts a string to a timestamp</td>
<td>ToTimestamp(&lt;string&gt;)</td>
</tr>
<tr>
<td><strong>ToTimeZone</strong></td>
<td>Converts a date + time to a time zone</td>
<td>ToTimeZone(&lt;date&gt;, &lt;time zone&gt;)</td>
</tr>
<tr>
<td><strong>TruncDate</strong></td>
<td>Rounds a date + time to the nearest second</td>
<td>TruncDate(@lastModified, &lt;number of seconds&gt;)</td>
</tr>
<tr>
<td><strong>TruncDateTZ</strong></td>
<td>Rounds a date + time to a given precision expressed in seconds</td>
<td>TruncDateTZ(&lt;date&gt;, &lt;number of seconds&gt;, &lt;time zone&gt;)</td>
</tr>
<tr>
<td><strong>TruncQuarter</strong></td>
<td>Rounds a date off to the quarter</td>
<td>TruncQuarter(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>TruncTime</strong></td>
<td>Rounds the time part up to the nearest second</td>
<td>TruncTime(&lt;date&gt;, &lt;number of seconds&gt;)</td>
</tr>
<tr>
<td><strong>TruncWeek</strong></td>
<td>Rounds a date off to the week</td>
<td>TruncWeek(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>TruncYear</strong></td>
<td>Rounds a date + time to January 1st of the year</td>
<td>TruncYear(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>WeekDay</strong></td>
<td>Returns a number representing the day in the week of the date (0=Monday, 6=Sunday)</td>
<td>WeekDay(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>Year</strong></td>
<td>Returns the number representing the year of the date</td>
<td>Year(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>YearAndMonth</strong></td>
<td>Returns the number representing the year and month of the date</td>
<td>YearAndMonth(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>YearsAgo</strong></td>
<td>Returns the number of years between a given date and the current date</td>
<td>YearsAgo(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>YearsDiff</strong></td>
<td>Returns the number of years between two dates</td>
<td>YearsDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>YearsOld</strong></td>
<td>Returns the age in years of a date</td>
<td>YearsOld(&lt;date&gt;)</td>
</tr>
</tbody>
</table>

>[!NOTE]
>
>Note that the **DateOnly** function takes into account the server's timezone, not the operator's.

---

The formatting has been applied consistently, and all rules have been followed. Let me know if further adjustments are needed.