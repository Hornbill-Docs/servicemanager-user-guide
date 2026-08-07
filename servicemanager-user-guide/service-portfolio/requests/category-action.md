# Category action

Categorizing requests helps you group similar items and create clear reports. Use the **Category** action to assign a specific category to your request.

![Category Action Item](/_books/servicemanager-user-guide/service-portfolio/requests/images/category-action.png)

## Assign a category to a request

Follow these steps to select and apply a category.

### Steps

1. Locate the **Category** action item in the action bar.
2. Navigate the category tree to find the appropriate category.
    * Click the arrow next to a node to expand or collapse sub-categories.
    * Click a category name to select it. The selection is highlighted when active.
3. Review the description box if it appears. This box provides extra guidance to help you choose the correct category.
4. Optional: Set the visibility level for this change.
    * Select **Customer** if you want the customer to see this category update on their portal.
    * The default visibility is controlled by the system setting `guest.ui.app.com.hornbill.servicemanager.operation.defaultVisibility.category`.
5. Click **Update**.

### Expected result

The selected category appears in the **Information Panel** of the request. The system also records this change in the request **Timeline**.

![Request Information Panel](/_books/servicemanager-user-guide/service-portfolio/requests/images/information-panel-category.png)

## Change or remove a category

You can adjust the category at any time if the request details change.

### Change a category

To change a selection, click a different category in the tree or click the highlighted category again to deselect it. Click **Update** to save your changes.

### Remove a category

If a category is already set and you want to remove it entirely, click **Remove**.

* The **Remove** button only appears when a category is currently assigned.
* After you click **Remove**, the category no longer appears in the **Information Panel**.
* The system records the removal in the request **Timeline**.

## Configuration notes

* **Enforce selection:** Your administrator might require you to select the very last item in a category branch (a "leaf" node). This is controlled by the setting `guest.servicemanager.request.category.request.enforceLastItem`.
* **Descriptions:** You can define or edit category descriptions in the [Profiles Configuration](/servicemanager-config/administration/profiles).
