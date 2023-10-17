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

<!-- https://wiki.hornbill.com/index.php?title=Request_List_Views -->