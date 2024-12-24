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
* **General.** Assets types that don't fall under the standard classes can be listed here. This can things like desks and other office equipment.
* **Mobile Devices.** Assets such as smartphones and tablets.
* **Network Devices.** Routers, switches, physical firewalls, and other network devices.
* **Printers.** Laser printers, InkJet printers, scanners, and fax machines.
* **Software.** Software applications.
* **Telecoms.** Phone systems, desk phones, and other communication assets.
* **Systems.** Business information such as ownership and authorizing contacts.
* **Data Processing Record.** Record of Processing Activity (ROPA).


## Assets List
The Assets List lets you access all the available assets. The following features are available to help you locate your assets and view and export information about these assets.

### Toolbar features
* **Add a New Asset.** The New Asset button allows for the manual creation of an asset. This button is located on both the Asset Landing Page and the Asset List. Adding an Asset Manually.
    :::tip
    * You can add multiple assets as a batch using the Upload Assets CSV.
    * You can do automated processing using an external data source via the [Hornbill Asset Import utility](/data-imports-guide/assets/overview).
    :::
* **Quick Filter.** The filter can be used to quickly focus on those asset records that are important to you. The filter will operate on the asset records that appear in the current list and will return records where a match is found in any of the asset attributes.
    :::tip
    To search on the class-specific attributes of an asset record, you must be viewing a class-specific list. It will search all asset attributes regardless of whether  the attribute is displayed in your list view. The filter does not operate on attributes containing a date-time value, state, location type, acq. method, or depreciation method. (However, sorting on these columns should allow effective identification of the records of interest).
    :::
* **Advanced Search.** Use the advanced search option to filter assets based on multiple definable conditions. Before adding your first Condition make sure you select the appropriate Asset Class from the Class Selector. Once you start adding the first Condition, the Asset Class will be locked to the current Asset Class and the matching fields for that Asset Class will be available when adding conditions. Once Conditions are set use either the search option to filter the results and or saved the search as one of your views.
* **Class Selector.** Switch between Asset Classes or All assets by selecting the relevant option (Note the list columns will change to reflect those configured for each Asset Class).
* **Views.** The Views provide a way of defining and storing a number of different views of the assets. The criteria builder lets you specify conditions based on information held in the asset records, giving you quick access to particular sets of important data. You can quickly change your Views by selecting from your list of defined views on the Asset List toolbar.
* **Export Assets.** Export the contents of the Asset list to CSV. Choose which of the available columns on the list you wish to export (the available options will be specific to the asset class).
* **Home View.** The Home View allows you to create a preferred or default view of your Asset List. Your Home View is displayed when you first visit your Asset List and with a single click you can return to your Home View from any other filter or view which you have applied.
* **Customize Columns.** The available columns will be specific to the Asset Type the list is using. The available columns will be a combination of the common attributes which all Asset Types share, and the Type Specific attributes for the selected Asset Type. If choosing to display All Assets only the shared asset attributes will be available to select from.

## List features
* **Column Sorting.** Each column header allows the order of the list to be changed by clicking on the title of each column
* **View an Asset.** Each Asset in the list contains links to open the Asset Details form
* **Delete an Asset.** Using the multi-select check boxes, one or more assets can be selected. Once selected the Delete button becomes available in the Asset List tool bar. Multiple assets can be selected by clicking on one asset, and then while holding down the Shift key and select another asset. All assets between these two assets will be selected and available for deleting.

<!-- https://wiki.hornbill.com/index.php?title=Manage_Assets -->