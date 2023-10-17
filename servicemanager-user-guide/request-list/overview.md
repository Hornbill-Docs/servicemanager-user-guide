---
layout: article-toc
---
# Overview
The Request List provides the visibility and management of the different request types in Service Manager. This includes Incidents, Service Requests, Problems, Known Errors, Changes, and Releases. Each member of the Service Desk will use the request list to manage their queues. The requests available to each user is determined by the roles and teams that a user belongs to, in conjunction with the Services their teams support.

## Tool Bar
### Filters
Quickly filter your list to find and view requests

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

:::tip
The Request List does not include Closed or Canceled requests when using the standard Filters. Closed and Canceled Requests can only be accessed by creating a View or by using the Global Search for Requests
:::

<!-- https://wiki.hornbill.com/index.php?title=Export_List -->