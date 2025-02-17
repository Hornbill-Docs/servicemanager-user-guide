---
layout: article-toc
---
# Manage Assets
The Manage Assets feature lets you add, update, and remove assets. You do this within an asset list, where you can search for assets, then open and view them.

## Assets landing page
When you first select the Manage Assets option, a tiled Assets landing page is displayed, showing the different available asset classes. Clicking on any of the tiles  displays an asset list with all the assets belonging to that class.

The available classes include:

* **All Assets.** All assets, independent of their class. The available information in this view is generic to all asset classes.
* **Computer Peripherals.** Keyboards, monitors, and other types of computer peripherals.
* **Computer Systems.** Servers, desktop computers, and other types of computer systems.
* **General.** Assets types that don't fall under the standard classes can be listed here. This can be things like desks and other office equipment.
* **Mobile Devices.** Assets such as smartphones and tablets.
* **Network Devices.** Routers, switches, physical firewalls, and other network devices.
* **Printers.** Laser printers, inkjet printers, scanners, and fax machines.
* **Software.** Software applications.
* **Telecoms.** Phone systems, desk phones, and other communication assets.
* **Systems.** Business information such as ownership and authorizing contacts.
* **Data Processing Record.** Record of Processing Activity (ROPA).


## Assets list
The Assets List lets you access all the available assets. The following features are available to help you locate your assets and view and export information about these assets.

### Toolbar features
* **Add a new asset.** You can add an asset manually. Click **+ New Asset** to create an asset.
    :::tip
    * You can add multiple assets as a batch using the [Upload Assets CSV](/servicemanager-user-guide/asset-management/upload-assets).
    * You can do automated processing using an external data source via the [Hornbill Asset Import utility](/data-imports-guide/assets/overview).
    :::
* **Quick filter.** Use this filter to quickly focus on those asset records that are important to you. The filter  operates on the asset records in the current list and  returns records where a match is found in any of the asset attributes.
    :::tip
    To search on the class-specific attributes of an asset record, you must be viewing a class-specific list. The quick filter searches all asset attributes regardless of whether  the attribute is displayed in your list view. The filter does not operate on attributes containing a date-time value, state, location type, acquisition method, or depreciation method. (You can, however, sort on these columns to identify the records of interest).
    :::
* **Advanced search.** Click **Advanced** (the search button to the right of the quick filter) to filter assets based on one or more conditions that you define. Before adding your first condition, make sure you select the appropriate asset class from the class selector. Once you start adding the first condition, the asset class will be locked to the current asset class and the matching fields for that asset class will be available when adding conditions. Once conditions are set, use the quick filter to filter the results, or save the search as one of your views.
* **Class selector.** Switch between Asset Classes or All Assets by selecting the relevant option. (Note that the list columns will change to reflect those configured for each asset class).
* **Views.** The Views feature lets you define and store a number of different views of the assets. The criteria builder lets you specify conditions based on information held in the asset records, giving you quick access to particular sets of important data. In the the Assets List toolbar, you can quickly change views by selecting from your list of defined views.
* **Export List.** Export the contents of the assets list to CSV. Choose which of the available columns on the list you wish to export (the available options are specific to the asset class).
* **Home View.** Click **Home View** > **Set current view as my Home** to create a preferred or default view of your Assets List. Your Home View is displayed when you first visit your Assets List, and with a single click you can return to your Home View from any other filter or view that you have applied.
* **Customize columns.** The available columns are specific to the asset type the list is using. The available columns are a combination of the common attributes that all asset types share, and the type-specific attributes for the selected asset type. If you choose to display all assets, only the shared asset attributes will be available to select from.

## List features
* **Column sorting.** On each column header, you can re-order the list by clicking the column name.
* **View an asset.** Each asset in the list contains links to open the Asset Details form.
* **Delete an asset.** Using the multi-select check boxes, select one or more assets. Once selected, the **Delete** button becomes available next to the **Advanced** button. To select multiple assets, click on one asset, and then while holding down the Shift key, select another asset. All assets between these two assets will be selected and available for deleting.

<!-- https://wiki.hornbill.com/index.php?title=Manage_Assets -->