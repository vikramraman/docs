---
title: Managing Maintenance Windows
keywords: alerts
tags: [alerts]
sidebar: doc_sidebar
permalink: maintenance_windows_managing.html
summary: Learn how to use maintenance windows to prevent alerts from firing when systems are undergoing maintenance.
---
A maintenance window is a time window when disruptive operations occur as a result of system maintenance or testing. These disruptive operations create a high likelihood of causing [alerts](alerts_managing.html#creating-an-alert) to fire. A maintenance window allows you to identify when maintenance is scheduled and prevent affected alerts from firing.

You can close (end) maintenance windows before they are due to end and you can extend the end time by various increments.

To view and manage maintenance windows, select **Browse > Maintenance Windows**.

<div markdown="span" class="alert alert-info" role="alert">While every Wavefront user can view maintenance windows, you must have [Alert Management permission](permissions_overview.html) to [manage](maintenance_windows_managing.html) maintenance windows. If you do not have permission, the UI menu selections, buttons, and links you use to perform management tasks are not visible.</div>

## Creating a Maintenance Window

To create a maintenance window:

1. Click **Alerts** or **Browse > Maintenance Windows**.
1. Click the **Create Maintenance Window** button located at the top of the filter bar.
1. Fill in the maintenance window properties:

    <table>
    <thead>
    <tr><th width="20%">Property</th><th width="80%">Description</th></tr>
    </thead>
    <tbody>
    <tr>
    <td>Name</td>
    <td>The name of the maintenance window.</td>
    </tr>
    <tr>
    <td>Description</td>
    <td>Additional information about the maintenance window. Information entered into this field appears directly below the maintenance window in the Maintenance Windows browser.</td>
    </tr>
    <tr>
    <td>Start Time</td>
    <td>The start time of the maintenance window:
    <ul><li><strong>Now</strong> - The maintenance window starts immediately.</li>
    <li><i class="fa fa-calendar"></i> - The maintenance window starts on the specified date and time. Click the text field and choose a date and time or type a date and time in the format MM/DD/YYYY HH:MM [AM|PM].</li></ul></td>
    </tr>
    <tr>
    <td>End Time</td>
    <td><i class="fa fa-calendar"></i> The end time of the maintenance window. The end time must be after the start time. Click the text field and choose a date and time or type a date and time in the format MM/DD/YYYY HH:MM [AM|PM].</td>
    </tr>
    <tr>
    <td>Affected Alerts and Sources</td>
    <td>The alerts and sources to suppress during the maintenance window. All alerts that have tags in the <strong>Alert Tags</strong> field are suppressed. An alert is suppressed if at least one of sources identified by the <strong>Source Tags</strong> and <strong>Sources</strong> fields causes the alert condition to be met. You must configure at least one alert tag, source, or source tag.</td>
    </tr>
    </tbody>
    </table>
1. Click **Save**.


## Extending, Closing, Editing, and Deleting Maintenance Windows

You can extend the duration of a maintenance window or close the window before it is scheduled to finish. To extend or close one or more maintenance windows:

1. Select **Browse > Maintenance Windows**.
1. Check the checkboxes next to the maintenance windows.
1. Click the **Extend** dropdown and select the desired duration or click the **Close** button.
1. Click the confirmation.
 
To extend the duration of a single maintenance window, select **Extend > Duration** at the far right of the window.

To close, edit, or delete a single maintenance window, select ![action menu](images/action_menu.png#inline) > **\[Close \| Edit \| Delete\]** at the far right of the window.
