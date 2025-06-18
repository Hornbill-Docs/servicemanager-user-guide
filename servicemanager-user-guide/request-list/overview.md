---
layout: article-toc
---
# Overview
The Request List provides the visibility and management of the different request types in Service Manager. This includes Incidents, Service Requests, Problems, Known Errors, Changes, and Releases. Each member of the Service Desk will use the Request List to manage their queues. Which requests are available to each user is determined by the roles and teams that a user belongs to, in conjunction with the services their teams support.

![Request List](/_books/servicemanager-user-guide/request-list/images/request-list.png)

## Accessing the Request List
**To get to the Request List:**
1. Locate the Service Manager icon on the left-hand vertical tool bar.
1. Click the Service Manager icon to display the sub-menu.
1. Select **Request List**.

## Making the Request List your default view
The Request List can be a place where users spend most of their time working. For quick access, a user can set the Request List as their default view.

**To make the Request List your default view:**
1. Access the Request List.
1. Click your profile picture in the top right to open the Profile menu.
1. Under *Actions*, click **Make this my default view**.

Once set, you will be automatically taken to the request list after you log in to Hornbill.  Also, now that this is your default view, you can click the Hornbill logo to return to the Request List.

## Toolbar filters
With filters, you can control the information displayed in the Request List and you can quickly locate requests.

### Status filter
Clickable links are available for the different statuses. Click any of link to filter the list by the selected status. 

![Status Filter](/_books/servicemanager-user-guide/request-list/images/status-filter.png)

The available statuses include:

* Total
* New
* Open
* Resolved
* On-hold

:::tip
The statuses of Closed and Canceled are not listed as filters, because these typically represent archived requests that are no longer active or being addressed. To locate closed or canceled requests, use the Advanced filter or [Views](/servicemanager-user-guide/request-list/views) options.
:::
<br>

### Quick filter
You can use the quick filter to refine your list to show only requests that contain the typed text.

![Request List](/_books/servicemanager-user-guide/request-list/images/quick-filter.png)

The fields in the requests that the quick filter uses to compare are:
* Reference
* Summary
* Details
* Owner
* Customer
* External Reference
* Priority

::: warning 
To ensure that views remain responsive when using multiple criteria and filters, be careful when using the quick filter. Make sure you [understand how the quick filter works](/servicemanager-user-guide/request-list/filter-usage).
:::

### Request Type filters
The Request Type Filter options are represented by the icons that are associated to each request type.

The available request types include incidents, problems, known errors, changes, and service requests. Depending on the rights you have, there may be one or more of these request types visible. Provided that you have rights to more than one request type, you will also see an 'All' option that displays all requests, independent of the type, in one list.

:::tip
To select more than one request type for display in your request list, hold down the Shift key on your keyboard and click each request type you want.
:::

### Group filters
The Group filters provide quick access to requests based on the relationship to you or by the teams that you belong to.

* **My Requests.** Displays requests where you are the owner.
* **I'm Following.** Displays requests that you are following.
* **I'm a Member.** Displays requests that you are a member of.
* **No Team Assigned.** Displays requests without a team assigned. A link is also added to the status bar to provide additional visibility of requests that have been raised with no team. This link is displayed only when there is one or more requests with no teams assigned.
    :::note
    This filter is only available to users with the Service Desk Admin role. To make this available to all users, enable the setting `webapp.view.ITSM.serviceDesk.requests.list.enableNoTeamAllUsers`.
    :::
* **All My Teams.** Displays requests belonging to all of your teams.
* **All My Services.** Displays requests belonging to any of the services your teams support. Included on this list are the names of all the teams that you belong to. To display all requests assigned to a team, select one of the teams in the list; this displays all requests that are assigned to that team, including requests assigned to you, to other team members, or those that are assigned to that team but that do not have an owner.

## Views
Create and configure your own lists of requests.

## My Dashboards
View a list of charts that are created using Views.

## Home view
The Home view allows you to create a preferred or default view of your Request List. Your Home view is displayed when you first visit your Request List, and with a single click you can return to your Home view from any other filter or view that you have applied.

### Setting your Home view
**To set your Home view:**
1. Select the combination of views and filters that you would like to use as your Home view.
1. Click the drop-down arrow next to the Home icon and select **Set current view as my Home**.

### Applying your Home view
Click the Home view icon (the house).

## Exporting a list
**To export the list that you are currently viewing to a CSV file:**
1. From the toolbar, click the **Export list** button. A form is provided with all the available columns for your list items.
1. Select one or more of the available columns that you would like to export.
1. Click **Export**. Your browser will download the file in CSV format to your local file system where it can then be opened with a spreadsheet application of your choice.

## Configuration
### Customize Columns
Each Service Manager user has the ability to select which columns are visible on the Request List. This is a per-user setting so that each individual can have their own list. This allows a user to display the information that is most important for them and the role that they have.
### Refresh Rate
Each Service Manager user has the ability to select how often their Request List is automatically refreshed. This is a per-user setting so that each individual can have their own refresh interval. To disable the refresh, set this to 0.

## Sorting requests
Each column within the list can be sorted in either descending or ascending order by clicking on the column header. Arrows next to each column header indicate the currently applied order.

Click once on the column name to sort in descending order. Click a second time, and the sort order is reversed. The column on which the list is currently sorted by has the column's name highlighted in blue, with an arrow showing whether the order is ascending or descending.

## Scrolling
A maximum of 50 requests are loaded into the list at a time. If you have more than 50 requests, scroll down the list to continue the loading. By not loading all requests at one time, the performance is improved.

## Multi-select options
By manually selecting one or more checkboxes in each row, or by holding down the Shift key and selecting multiple checkboxes in one go, some options are provided that can be applied to each of the selected records.

When multiple requests are selected, you can:

* **Assign.** Assign the requests to another team or analyst.
* **Boards.** Add the requests to one of your boards or a board that you have permissions to access. Select the board and the specific list on the board to which you wish to add the requests.
* **Update.** Apply an update to multiple requests at once.
* **Priority.** Set the priority, including an escalation reason.
* **Resolve.** Resolve the requests. A resolution reason must be provided.
* **Cancel.** Cancel the requests.

## Color coding
The background color of each row represents a particular state of the request.

### Read / Unread
This focuses on the owner of the request. All users will see the read/unread state based on whether the owner has read or not read the request since the last update.  Being a collaborative environment, it allows for someone to contribute to a request and be aware when the owner has read their update.
* **Yellow.** Requests that have been updated by anyone other than the owner of the request, and for which the owner has not yet read the update.
* **White.** Requests where all the updates have been read by the owner.
 
 :::tip
 The default unread color is yellow, but you can change the color  globally using this system setting: `webapp.view.ITSM.serviceDesk.requests.list.unreadColour`. Available colors include alice blue, beige, blanched almond, honeydew, khaki, light cyan, light yellow, pale turquoise, and white.
:::

### On-hold requests
Any request that has been put on hold can be displayed in a different format from the active requests. There are three choices for the display of on-hold requests:

* Bold
* Italic (default)
* Opaque

Set this display in the Admin portal using the Service Manager `setting webapp.view.ITSM.serviceDesk.requests.list.onHoldFontStyle`.

## Last Updated By
This field can be added to the request to help identify who last updated the request. This can also color-coded to help quickly identify whether the update was done by a customer, a support person, or an automatic update.

Select your color using the following Service Manager settings. By default, the colors are turned off.

|Name|Description|
|-|-|
|`webapp.view.ITSM.serviceDesk.requests.list.lastUpdateByColor.analyst`|Color to use as background of Updated By when user is an analyst.|
|`webapp.view.ITSM.serviceDesk.requests.list.lastUpdateByColor.system`|Color to use as background of Updated By when user is a system user.|
|`webapp.view.ITSM.serviceDesk.requests.list.lastUpdateByColor.customer`|Color to use as background of Updated By when user is a customer.|

## Service Level indicators
Response and Fix Timer indicators can be displayed on the request list by exposing the Service Level column from the column selector.

|Color|Description|
|-|-|
|Clear|Timer not in use|
|Green|Met|
|Blue|Ongoing|
|Red|Breached and still open|

<!-- https://wiki.hornbill.com/index.php?title=Export_List -->
<!-- https://wiki.hornbill.com/index.php?title=Request_List_Filters -->