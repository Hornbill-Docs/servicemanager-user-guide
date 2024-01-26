# Category
The Category Action Item lets you select the request category against the request

The category tree can be expanded by clicking on each node. Nodes that display an arrow indicate that there are more categories beneath it. The different levels of the category tree can be expanded or collapsed by clicking on these arrows.

By clicking on a category, the category will become selected. The selection of the last category in a branch can be enforced using the Service Manager setting `guest.servicemanager.request.category.request.enforceLastItem`

Once a category has been selected, it can be changed by either

* Selecting another category
* Selecting the highlighted category a second time
* Clicking on the Remove button

When a category is selected, a description box will appear if a description for that category has been provided. This is to give a user a bit more guidance in selecting the correct category. The description of a category can be defined under the [Profiles in Platform Configuration](/esp-config/data/profiles#editor).

## Update
The update button will apply the selected category to the request. Once updated, the category will be displayed within the Information Panel of the request. Each update to the category will be recorded in the Timeline of the request.

## Visibility
Prior to updating the category, a user can select the visibility level of the update to be added to the Request Timeline. Visibility set to Customer will allow a customer to view the category change on the portals. A default visibility level can be set using the Service Manager setting `guest.ui.app.com.hornbill.servicemanager.operation.defaultVisibility.category`