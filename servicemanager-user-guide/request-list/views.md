---
layout: article-toc
---
# Views
With Request List Views, you have a way of defining and storing a number of different views of the requests to which you have access. Using the views' data, you can create multiple charts that can be published to your dashboard. The criteria builder lets you specify conditions based on information held in the request records, giving you quick access to particular sets of important data.

You can quickly change your views by selecting from your list of defined views on the Request List toolbar. This list is made up of your own views as well as any views that have been shared with you.

## Managing your views
**To create a new view:**
1. From the Views dropdown list in the Request List tool bar, click **Add New**.
1. Give the view a name. This name will be visible from the Views dropdown list once saved.
1. Add your [criteria](/servicemanager-user-guide/request-list/views#criteria).

**To copy a view:**
1. From the Views dropdown list in Request List toolbar, move your mouse over the view you want to copy and click the cog icon to open the Edit View dialog.
1. Give the copied view a new name.
1. Change or add any additional criteria.
1. Click **Make a copy**.
The view automatically changes to your new, copied view.

**To delete a view:**
1. From the Views dropdown inn Request List toolbar, move your mouse over the view you want to delete and click the cog icon to open the Edit View dialog.
1. Click **Delete**.

## Criteria
The Criteria tab lets you add a variety of conditions to produce the desired view.

Along with any conditions you specify, the views automatically take into account your team membership and the services that your team supports. If you are not a member of a team, or are not part of a team that supports the service against which the request is raised, then that request will not be visible to you.

The following options are available for defining a condition:

* **Source.** Select this first field to find a list of familiar titles that form the data stored on a request.
* **Operator.** The available operators depend on the selected source. Source values that contain:
    * Set values will include the operators IS and IS NOT.
    * Dates will include *before*, *before x days*, *after*, *today*, *yesterday*, *last 7 days*, *last 30 days*, *last x days*, *previous month*, *current month*, and *last x months*.
    * Free text values will include *is*, *is not*, *is less than*, *is greater than*, *contains*, and *does not contain*.
    * Counters will include operators such as *is*, *is not*, *is less than*, and *is greater than*.
* **Value.** The value to compare the source with, based on the set operator. The value field will use a number of methods for entering a value, including drop-down lists, free text, auto-complete searches, and numeric inputs. This will vary depending on the selected source.

:::note
Custom fields P-T are of type Text. For performance reasons, these fields are excluded from being available to build criteria from.
:::

## Columns
The Columns tab lets you define which columns will be available in the request list when you select the view.

* **Available display columns.** Click on any of the available columns to enable or disable them from being included in the request list when this view is selected. Here, you can also change the order of the columns by dragging and dropping the columns.
* **Revert.** Clicking the **Revert** button puts the list of selected columns back to the original default selection.
* **+ Custom column.** If custom fields have been used in the design of your request forms, this option provides the ability to add columns to display the information captured in your custom fields. When adding a custom column, you will have options as follows:
    * **Column.** Select one of the available custom fields that contains the information that you want to display as a column on your view.
    * **Visible.** Toggle this ON to activate this new column on your request list.
    * **Language.** Set the language for your display name. This can be useful when sharing your view with other users that might use a different language.
    * **Display Name.** Provide a display name of your column, which will be shown at the top of the column on the request list when this view is selected.

:::tip
Custom fields P-T are of type Text and are excluded from being available to display for performance reasons.
:::

## Charts
You can create one or more charts against each view that you have defined. Once charts are created, they are available for use in your own personal dashboard. Charts are also available with any shared view. These charts need to have the visibility enabled in order to show in *My Dashboards*.

You can toggle between your request list view and your *My Dashboards* using the **Switch to My Dashboards** and **Switch to Request List** buttons.

### Creating charts
In order to create a chart, you first must have [defined a view on the request list](/servicemanager-user-guide/request-list/views#managing-your-views).

**To create a chart:**

1. From an existing view, click the Charts tab. Criteria for the chart is inherited from the view; you can review the criteria from the Criteria tab when creating a chart.
1. Give the chart a name.
1. From the Chart Type dropdown, select the type of chart you wish to create. Depending on the type selected, the Y and X axis titles for the chart will be visible or be hidden based on their relevance.
1. Decide how you want the chart data to be displayed. Select the appropriate column from the X-Axis dropdown. Depending on the column you select here, more selection criteria options may be presented. An example of this would be date columns such as *Date Closed* or *Last Updated*. If date columns are selected, an additional Date Type dropdown (e.g. *Month*) will be available, then once another date type is selected here , a further date type-specific dropdown will be available (e.g. for *Month* you get *Year*).
1. Click **Preview Chart** to preview the data.
   By default, the chart will immediately be visible on your dashboard. This is represented by the green **Chart Visible** button.
1. (Optional) To hide a specific chart from your dashboard, click the **Chart Visible** button so that it toggles to a gray **Chart is Hidden** button. You can adjust chart visibility at any time.
1. (Optional) In the Add Dashboard field, select a dashboard on which to display this chart. When no dashboard is selected here, the chart displays only on your own dashboard.
1. Click **Save** to activate your chart and make it visible on your dashboard.

![Chart Properties](/_books/servicemanager-user-guide/request-list/images/chart-dashboard-selection.png)

:::tip
Custom fields P-T are of type Text and are excluded from being available to group chart data by, for performance reasons.
:::

### Creating multiple charts per view
You can reuse the defined criteria of a view, and create multiple charts based on this, in order to present the data from different perspectives. One example could be a series of charts looking at a change view by *Source*, *Owner*, or *Priority*.

Once you have created your first chart for a view, you have the option to create further charts. Subsequent charts will appear in the Charts tab of the view, and can be viewed, edited, and deleted from there.

## Share
From time to time, you may find a combination of criteria that would be useful to others. In the Share tab of the Edit View dialog, you can give other Service Manager users visibility of your view. Shared views are visible to users from their Views list, under a section titled *Shared Views*.

* **Team.** Select this option to share your view with an entire time. In the Team dropdown, the selection list is split into *My Teams*, which are the teams that you belong to, and *Supporting Teams* which are teams that support the services that you support.
* **User.** Share your view with any other Service Manager user.
* **Service.** Share your view with all the teams that support a selected service.

A list of users, teams, and services that you have shared the view with will be displayed on this same form. Remove any of the previous shares by clicking the **X** button next to the user, team, or service that you want to remove.

:::tip
Views can only be edited by the owner. Users who have had a view shared with them can't edit the view's criteria; nor can they create charts for their personal dashboards from shared views.

A shared view in many cases will not result in the same results in the request list, because the user may have different access rights and visibility of requests. A user with whom the view is shared will only be able to view custom fields; these will only be available to the creator of the view when exporting.
:::

### Managing shared views
There may be occasions when a user is no longer using Hornbill and they have left behind views that were shared with other users. A Hornbill user that has the role Service Desk Admin will have an option from the Views menu, under *Shared Views*, titled *Manage*. Here, the admin can manage all shared views. The admin can take the following actions: **Delete**, **Change Owner**, and **Make Me Owner**.
<!-- https://wiki.hornbill.com/index.php?title=Request_List_Views -->
<!-- https://wiki.hornbill.com/index.php?title=Charts -->