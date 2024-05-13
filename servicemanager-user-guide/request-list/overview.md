---
layout: article-toc
---
# Overview
The Request List provides the visibility and management of the different request types in Service Manager. This includes Incidents, Service Requests, Problems, Known Errors, Changes, and Releases. Each member of the Service Desk will use the request list to manage their queues. The requests available to each user is determined by the roles and teams that a user belongs to, in conjunction with the Services their teams support.

![Request List](/_books/servicemanager-user-guide/request-list/images/request-list.png)

## Accessing the Request List
1. Locate the Service Manager icon on the left hand vertical tool bar.
1. Click on the Service Manager icon to display the sub-menu.
1. Select `Request List`.

## Making the Request List Your Default View
The request list can be a view where many users spend most of their time working. For quick access a user can set the request list as their default view.

1. Access the request list.
1. Click on your profile picture in the top right to open the Profile Menu.
1. Select `Make this my defualt view`.

Once set, you will be automatically taken to the request list when you log in to Hornbill.  You can also click on the Hornbill logo at any time to return to this view.

## Tool Bar
### Filters
A variety of filters let you control the information displayed in the Request List and can be used to quickly locate requests. The options for filtering are represented by a number of buttons in the Request List Toolbar. The active filter can be determined by which filter buttons are colored gray.

#### Status Filter
Links are available for the different statuses. Clicking on any of these links will filter the list by the selected status. 

![Status Filter](/_books/servicemanager-user-guide/request-list/images/status-filter.png)

* Total
* New
* Open
* Resolved
* On-hold

:::tip
The statuses of "closed" and "canceled" are not listed as filters, as they are typically considered archived requests that are no longer active or being addressed. To locate closed or canceled requests, the Advanced Filter or [Views](/servicemanager-user-guide/request-list/views) options can be utilized.
:::

#### Quick Filter
The quick filter is used to refine your list to only show requests that contain the typed text. The fields in the requests which the quick filter uses to compare are:
* Reference
* Summary
* Details
* Owner
* Customer
* External Reference
* Priority

:::tip
An additional keyboard short-cut (CTRL+SHIFT+F) will present a popup search box for directly accessing a particular request. The full request ID must be entered. This can be accessed from anywhere in Hornbill.
:::

#### Request Type Filters
The Request Type Filters options are represented by the icons that are associated to each request type.

The available request types include incidents, problems, known errors, changes, and service requests. Depending on the rights you have, there may be one or more of these request types visible. Provided that you have rights to more than one request type, you will also see an 'All' option which will display all requests, independent of the type, in one list.

:::tip
By holding down the Shift key on the keyboard and clicking on the different request types, you can have more than one request type selected and displayed in your request list
:::

#### Group Filters
The Group Filters provide quick access to requests based on the relationship to you or by the teams that you belong to.

* **My Requests**<br>Displays requests where you are the owner
* **I'm Following**<br>Displays requests that you are following
* **I'm a Member**<br>Displays requests that you are a member of
* **No Team Assigned**<br>Displays requests without a team assigned. This filter is only available to users who possess the Service Desk Admin role. If preferred, this can be made available to all users by enabling the setting webapp.view.ITSM.serviceDesk.requests.list.enableNoTeamAllUsers. A link is also added to the status bar to provide additional visibility of requests that have been raised with no team. This link will only be displayed when there is 1 or more requests with no teams assigned.
* **All My Teams**<br>Displays requests belonging to all of your teams
* **All My Services**<br>Displays requests belonging to any of the services your teams support

Included on this list are the names of all the teams that you belong to. Selecting one of the teams in the list will display all requests that are assigned to that team, including requests assigned to you, other team members, or that are assigned to that team but do not have an owner.

## Views
Create and select configurable your own lists of requests

## My Dashboards
View a list of charts that are created using Views

## Home View
The Home View allows you to create a preferred or default view of your Request List. Your Home View is displayed when you first visit your Request List and with a single click you can return to your Home View from any other filter or view which you have applied.

### Setting Your Home View
1. Select the combination of Views and Filters which you would like to use as your Home View
1. Using the drop down menu next to the Home Icon, select 'Set current view as my Home'
1. Your Home View is now set

### Applying Your Home View
Click on the Home View Icon (House) from the icon menu

## Export List
Export the list that you are currently viewing to a CSV file

1. From the Tool Bar click on the Export List button.
1. A form is provided with all the available columns for your list items.
1. Select one or more of the available columns that you would like to export.
1. Click on the 'Export' button.
1. Your browser will download the file in CSV to your local file system where it can then be opened with a spreadsheet application of your choice.

## Configuration
### Customize Columns
Each Service Manager user has the ability to select which columns are visible on the request list. This is a per user setting so that each individual can have their own list. This allows a user to display the information which is most important for them and the role that they have.
### Refresh Rate
Each Service Manager user has the ability to select how often their request list is automatically refreshed. This is a per user setting so that each individual can have their own refresh interval. Setting this to 0 will disable the refresh.

## Sorting
Each column within the list can be sorted in both descending and ascending order by clicking on the column header. Arrows next to each column header indicate the currently applied order.

Click once on the column name to sort in descending order
Click a second time and the sort order is reversed
The column on which the list is currently sorted by will have the column's name highlighted in blue, with an arrow showing whether the order is ascending or descending.

## Scrolling
A maximum of 50 requests are loading onto the list at a time. If you have more than 50 these will automatically load as you scroll down the list. By not loading every request at one time, the performance is improved.

## Multi-Select Options
By manually selecting one or more check boxes in each row or using the select and Shift key to select multiple check boxes in one go, some options are provided which can be applied to each of the selected records.

When multiple requests are selected you will be able to:

* **Assign**<br>Assign the requests to another team or analyst.
* **Boards**<br>Add the requests to one of your boards or a board that you have permissions to access. Select the Board, and the specific list on the Board, to which you wish to add the requests.
* **Update**<br>Apply an update to multiple requests at once.
* **Priority**<br>set the priority including an escalation reason.
* **Resolve**<br>Resolve the requests. A resolution reason must be provided.
* **Cancel**<br>Cancel the requests.

## Color Coding
The background color of each row represents a particular state of the request.

### Read / Un-read
This focuses on the owner of the request. All users will see the read/unread state based on if the owner has read or not read the request since the last update.  Being a collaborative environment, it allows for someone to contribute to a request and be aware when the owner has read their update.
* **Yellow**<br>Requests which have been updated by anyone but the owner of the request, and the owner has not yet read the update.
* **White**<br>Requests where all the updates have been read by the Owner.
 
 :::tip
 The default un-read color is set to Yellow, however the color can be changed globally using this system setting webapp.view.ITSM.serviceDesk.requests.list.unreadColour. Available colors include alice blue, beige, blanched Almond, boneydew, khaki, light cyan, light yellow, pale turquoise, white
:::

### On-hold Requests
Any request that has been put on hold can be displayed in a different format from the active requests. There are three choices for the display of on-hold requests.

* Bold
* Italic (default)
* Opaque

This display can be set in the Admin portal using the Service Manager setting webapp.view.ITSM.serviceDesk.requests.list.onHoldFontStyle

## Last Updated By
This field can be added to the request to help identify who last updated the request. These can also color coded to help quickly identify if the update was done by a customer, support person, or an automatic update.

Select your color using the following Service Manager settings. By default, the colors are turned off.

|Name|Description|
|-|-|
|webapp.view.ITSM.serviceDesk.requests.list.lastUpdateByColor.analyst|Colour to use as background of updated by when user is an analyst|
|webapp.view.ITSM.serviceDesk.requests.list.lastUpdateByColor.system|Colour to use as background of updated by when user is a system user|
|webapp.view.ITSM.serviceDesk.requests.list.lastUpdateByColor.customer|Colour to use as background of updated by when user is a customer|

## Service Level Indicators
Response and Fix timer indicators can be displayed on the request list by exposing the SL column from the column selector.

|Color|Description|
|-|-|
|Clear|Timer not in use|
|Green|Met|
|Blue|Ongoing|
|Red|Breached and still open|

<!-- https://wiki.hornbill.com/index.php?title=Export_List -->
<!-- https://wiki.hornbill.com/index.php?title=Request_List_Filters -->