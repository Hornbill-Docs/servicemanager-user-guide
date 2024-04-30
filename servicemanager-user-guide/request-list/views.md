---
layout: article-toc
---
# Views
The Views provide a way of defining and storing a number of different views of the requests that you have access to. Using the Views data you can create multiple Charts which can be published to your Dashboard. The criteria builder lets you specify conditions based on information held in the request records, giving you quick access to particular sets of important data.

You can quickly change your Views by selecting from your list of defined views on the Request List toolbar, this list will be made up of your own views, and views that have been shared with you.

## Manage
### Create
1. From the View drop down list located on the Request List tool bar, select Add New.
1. Enter the name of the View. This name will be visible from the Views drop down list once saved.
1. Add the desired #Criteria.

### Copy
1. From the Views drop down list located on Request List tool bar, move your mouse over the desired View and select the 'cog' icon to open the Edit View.
1. Give the View a new name.
1. Change or add any additional criteria.
1. Click on the 'Make a copy' button.
1. Your view will automatically change to your new View.

### Delete
1. From the Views drop down list located on Request List tool bar, move your mouse over the desired View and select the 'cog' icon to open the Edit View.
1. Click on the Delete button.

## Criteria
The Criteria tab lets you add a variety of conditions to produce the desired view. Three options are available for defining a condition: Source, Operator, Value

* **Source**<br>When you select this field you will see a number of familiar title which mostly form the data that is stored on a request.
* **Operator**<br>The available operators will depend on the selected source. Source values that contain...
    * Set values will include the operators is and is not.
    * Dates will include before, before x days, after, today, yesterday, last 7 days, last 30 days, last x days, previous month, and current month.
    * Free text values will include is, is not, is less than, is greater than, contains, and does not contain.
    * Counters will include operators such as is, is not, less than, and greater than.
* **Value**<br>The value to compare the source with, based on the set operator. The value field will use a number of methods for entering a value, including pick lists, free text, auto-complete searches, and numeric inputs. This will vary depending on the Source type.

:::tip
Along with any conditions you specify, the views automatically take into account your team membership and the Services that your team supports. If you are not a member of a team, or not part of a team that supports the service against which the request is raised, then that request will not be visible to you.
:::

:::tip
Custom fields P-T are of type Text and are excluded from being available to build criteria from for performance reasons.
:::

## Columns
The Columns tab lets you define which columns will be available in the request list when you select the View.

* **Available Display Columns**<br>Click on any of the available columns to enable or disable them from being included in the Request List when this View is selected. The order of the columns can also be changed by a drag and drop of each of the available columns
* **Revert**<br>The Revert button will put the list of selected columns back to the original default selection.
* **+ Custom Column**<br>If Custom Fields have been used in the design of your request forms, this option provides the ability to add columns to display the information captured in your custom fields. When adding a custom column you will have the option to
    * *Column*<br>Select one of the available custom fields that contains the information that you would like to display as a column on your View
    * *Visible*<br>Turn this on in order to activate this new column on your Request List
    * *Language*<br>Set the language for your Display Name. This can be useful when sharing your View with other users that might use a different language.
    * *Display Name*<br>Provide a display name of your column which will be shown at the top of the column on the Request List when this View is selected

:::tip
Custom fields P-T are of type Text and are excluded from being available to display for performance reasons.
:::

## Charts
It is possible to create one or multiple Charts against each View that you have defined. Once Charts are created they will be available for use in your own personal dashboard. Charts are also available with any shared Viewed. These charts will need to have the visibility enabled in order to show on the My Dashboards.

## Share
From time to time you may find a combination of criteria that would be useful to others. The Share option lets you give other Service Manager users visibility of your View. The Share option is accessible by hovering over a View in the View selector and selecting the 'cog' icon. Select the Share tab. Shared 'Views will be visible to users from their Views list, under a section title Shared Views.

* **Team**<br>Select this option to share your View with an entire time. When searching for Teams the selection list is split into My Teams which are the teams that you belong to, and then the Supporting Teams which are teams that support the Services that you support.
* **User**<br>Share your View with any other Service Manager User.
* **Service**<br>Share your View with all the teams that support a selected Service
A list of Users, Teams, and Services that you have shared the View with will be displayed on this same form. Remove any of the previous shares by selecting the delete icon next to the user, team, or service that you want to remove.

:::tip
Views can only be edited by the owner, user's who have had the View shared with them can't edit the View criteria nor create charts for their Personal Dashboards from shared views. A shared View in many cases will not result in the same results in the Request List as the user may have different access rights and visibility of requests. A User with whom the View is shared will only be able to view Custom Fields, these will only be available to the Creator of the View when exporting.
:::

## Manage Shared Views
There may be occasions when a user is no longer using Hornbill and they have left behind Views which were shared with other users. A Hornbill User that has the Role Service Desk Admin will have an option from the Views menu, under Shared Views titled Manage from where they can manage all shared Views. These actions include

* Change Owner
* Make Me Owner
* Delete
<!-- https://wiki.hornbill.com/index.php?title=Request_List_Views -->