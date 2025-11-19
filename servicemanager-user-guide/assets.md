---
layout: article-toc
---
# Manage Assets
The Manage Assets feature lets you add, update, and remove assets. You do this within an asset list, where you can search for assets, then open and view them.

You can also copy asset records, create asset records in a batch, and apply changes to asset records in a batch. 

## Assets landing page
<!--When you first select the Manage Assets option, a tiled Assets landing page is displayed, showing the different available asset classes. Clicking on any of the tiles  displays an asset list with all the assets belonging to that class.-->

To access the Manage Assets feature, navigate to **Service Management > Assets**. A tiled Assets dashboard is displayed, showing the available asset types. Clicking on any of the tiles displays an asset list with all the assets belonging to that type.

<!--The available classes include:

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
* **Data Processing Record.** Record of Processing Activity (ROPA).-->


## Assets list
The Assets list lets you access all the available assets. <!--The following features are available to help you locate your assets and view and export information about these assets.-->

### Toolbar features
This section describes the actions you can take using the toolbar in the assets list.
<br>

![Toolbar in assets list](/_books/servicemanager-user-guide/asset-management/images/toolbar-in-assets-list.png)
* **Quick filter.** Use this filter to quickly focus on those asset records that are important to you. The filter operates on the asset records in the current list and returns records where a match is found in any of the asset attributes.
    :::tip
    To search on the class-specific attributes of an asset record, you must be viewing a class-specific list. The quick filter searches all asset attributes regardless of whether the attribute is displayed in your list view. The filter does not operate on attributes containing a date-time value, state, location type, acquisition method, or depreciation method. (You can, however, sort on these columns to identify the records of interest).
    :::
* **Advanced search.** Click **Advanced** (the search button to the right of the quick filter) to filter assets based on one or more conditions that you define. <!--Before adding your first condition, make sure you select the appropriate asset class from the class selector. -->Once you start adding the first condition, the asset class will be locked to the current asset class and the matching fields for that asset class will be available when adding conditions. Once conditions are set, use the quick filter to filter the results, or save the search as one of your views.
<!--* **Class selector.** Switch between Asset Classes or All Assets by selecting the relevant option. (Note that the list columns will change to reflect those configured for each asset class).-->
* **Add assets manually.** You can add an individual asset, or you can add assets in bulk by configuring one new asset and creating copies in the same batch. If you are creating assets in bulk, the batch will include one new asset (per your configuration in the New Asset dialog), plus copies of that asset.
    **To create one or more assets manually:**
    1. Click **+ New Asset**.
    1. In the New Asset dialog, from the dropdown, select a partition to create the asset(s) in, or keep the default (Un-partitioned Assets).
    1. From the dropdown, select the asset type of the asset(s) you want to create.
    1. Enter a name for the asset(s).
    1. If you are creating a single asset, click **Create & Open**.
    1. If you are creating multiple assets, click **Create & Open > Bulk create asset**.
    1. If you are creating multiple assets, in the Bulk Create Asset dialog, enter the number of copies you want.
    1. Click **Create**.
    1. In the dialog, when you receive confirmation, click **Close**.

    :::tip
    * Another way to add multiple assets as a batch is by using the [Upload Assets CSV](/servicemanager-config/assets/upload-assets).
    * You can do automated processing using an external data source via the [Hornbill Asset Import utility](/data-imports-guide/assets/overview).
    :::
* **Delete assets.** (This button is invisible until at least one asset has been selected using the multi-select checkboxes.)
    1. Select one or more assets.
    1. Click **Delete**.
    :::tip
    To select multiple assets, click on one asset, and then while holding down the Shift key, select another asset. All assets between these two assets will be selected and available for deleting.
    :::
* **Copy assets.** (The **Copy** button is invisible until one and only one asset has been selected using the multi-select checkboxes.)
    **To copy an asset:**
    1.	In the Assets list, select the checkbox for an asset, then click the **Copy** button.
    2.	In the Copy Asset dialog, enter a number for how many copies you want to create.
    3.	Click **Duplicate**.
    4.	When you are finished reading the confirmation message, click Close.
    
* **Bulk update.** You can make changes to multiple asset records at once.

   **To do a bulk update:**
    1.	In the Assets list, select the checkbox for the assets you want to update, or to select the whole list, select the **Select All** checkbox at the top. 
    If the assets you are updating all belong to the same asset class and asset type, then you can bulk update all the general fields and class-type fields. <!--What happens when they’re not of the same class and type?-->
    2.	Make changes as necessary.
        a.	From the Asset Bulk Update dialog, from the dropdown, select one or more fields that you want to change. For each one, click Add Field.
        b.	When you are finished making changes to fields, run the update by clicking one of the two Update buttons.
        *	**Batch Update (Fast).** This is a raw SQL statement: update these columns where assets match this.
        *	**Audited Update (Slow).** This updates assets one at a time,creating an audit history record for the asset.
    
* **Reload list.** To manually refresh the assets list, click **Reload list**.
* **Views.** You can define and store a number of different views of the assets.
    1. Click **Views > Add New**.
    1. In the Create New View dialog, in the Criteria tab, you can specify conditions based on information held in the asset records.
    1. In the Columns tab, select the columns you want to show in your view. 1. When finished, click **Save**.
    
    Now you can quickly access particular sets of important data by selecting from your list of defined views.
* **Export List.** Export the contents of the assets list to CSV. Choose which of the available columns on the list you wish to export (the available options are specific to the asset class).
    1. Click the **Export** button (the down arrow).
    1. In the dialog, in the Columns tab, select the columns you want to export.
    1. In the Settings tab, specify the export format and the number of records to export.
    1. When finished, click **Export**.
<!--* **Home View.** Click **Home View** > **Set current view as my Home** to create a preferred or default view of your Assets List. Your Home View is displayed when you first visit your Assets List, and with a single click you can return to your Home View from any other filter or view that you have applied.-->
* **Table Configuration.** The available columns are specific to the asset type the list is using. The available columns are a combination of the common attributes that all asset types share, and the type-specific attributes for the selected asset type. If you choose to display all assets, only the shared asset attributes will be available to select from.
    1. Click the cog icon next to the down arrow.
    1. In the Table Configuration dialog, in the Visibility tab, select the columns you want to show.
    1. In the Order tab, drag and drop the columns into your preferred order.
    1. In the Settings tab, use the dropdown to set the row density.
    1. When finished, click **Close**.

## List features
* **Column sorting.** On each column header, you can re-order the list by clicking the column name.
* **View an asset.** Each asset in the list contains links to open the asset details and the type details.


<!-- https://wiki.hornbill.com/index.php?title=Manage_Assets -->