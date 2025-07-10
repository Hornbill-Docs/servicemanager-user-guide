---
layout: article-toc
---
# Change Calendar
The Change Calendar provides a view of the scheduled changes and release packages. This indicates the availability of a change or the possible disruption of a change being implemented.

## Calendar
The Calendar provides a month-by-month view of the scheduled changes and releases. Changes and releases will only be visible if a scheduled date has been added manually to the request using the [Schedule Action](/servicemanager-user-guide/service-portfolio/requests/schedule-action) on the request, or automatically using the [change request](/servicemanager-config/customize/workflows/change-request-automation#update-request) and [release record](/servicemanager-config/customize/workflows/release-record-automation#update-request) automations.

### Views
On the toolbar there are several views that have been provided that allow you to filter the calendar to only show particular changes or releases.

* **Changes**<br>This option will only show Change Requests that have been scheduled on the Calendar.
* **Releases**<br>This option will only show Releases that have been scheduled on the Calendar.
* **All**<br>This option will show both Change Requests and Releases which have been scheduled on the Calendar.
* **All Requests**<br>This option will show all requests irrespective of ownership or which Service they have been raised against.
* **My Requests**<br>This option will show all the Changes and Releases that are owned or assigned to the person viewing the calendar.
* **My Services**<br>By selecting the My Services option, only the Changes or Releases that are associated with the services that the user supports are visible. This can be filtered down to an individual Service by selecting a service that is listed under this option.

The calendar can be filtered to show requests that come under a particular authorization status. These include:

* **Not Authorized**<br>View changes where the authorization is still pending.
* **Authorized**<br>View changes that have been authorized.
* **Rejected**<br>View changes that have been rejected.
* **All**<br>When All is selected, requests in the calendar can still be identified as Authorized by the green flag along the left side of the scheduled request, and Not Authorized with a blue flag along the left side of the scheduled change. In addition, the type of request can be identified by its icon on the scheduled entry.

### Status Colors
The status of changes and releases on the calendar can be easily seen by the following color scheme

|Color|Description|
|-|-|
|Blue|The change is in an open state|
|Green|The change has been successfully resolved|
|Gray|The change record has been closed|

## Change Freeze Periods
Users with the Full Change Management Access or the Full Release Management Access roles will be able to add and manage global change freeze periods on the Change Calendar.

:::note
A change freeze does not prevent a change from being raised within the freeze period. The freeze period only affects the scheduling of the change.
::: 

### Adding a new Change Freeze period
Users with the above roles will be able to select the Change Calendar Freeze period icon to add, edit or remove change freeze periods.

#### To add a new change freeze period 
1. select the + icon
1. Provide a start and end date and time
1. Provide a change freeze description

#### Edit or Delete Change Freeze Periods
1. Select the Change Calendar Freeze period icon and either the pencil to edit the date/times or description of the change freeze, or the trash can to permanently delete the change freeze period

All Active change freeze periods will be visible on the change calendar and are indicated by a gray color in the calendar dates.
* Hovering over a change freeze period will display more information
* Change Freeze periods are automatically checked on Change and Release requests when users attempt to schedule dates to the change calendar. Collisions are highlighted and enforced.

## Access
The following roles are required to view and use this feature

|Role|Description|
|-|-|
|Change Calendar Viewer|This role will enable the Change Calendar menu item under Service Manager. View only access to the Request List for changes will also be available.|
|Collaboration Role|This role is required for all users using the Hornbill portal.|