---
layout: article-toc
draft: false
---
# Manage Assets
::: note
This article is new, to support the preview release of the new Asset Management and its new UI. You can find documentation for the legacy UI [here](/servicemanager-user-guide/asset-management/manage-assets).
:::
The Manage Assets feature lets you add, update, and remove assets. You do this within an asset list, where you can search for assets, then open and view them.

You can also copy asset records, create asset records in a batch, and apply changes to asset records in a batch. 

## Before you begin
To manage assets, a user requires the following roles and rights.

* The Asset Management User role including the `View Asset Management` application right, plus one or both of the rights `Create Assets` or `Edit Assets`; *or*
* A custom role that includes the `View Asset Management` application right, plus one or both of the rights `Create Assets` or `Edit Assets`.

    ::: important
    If the asset records you are working with are [in a partition set up by your assets admin](/servicemanager-config/assets/manage-partitions), then what you can do with assets is limited to the permissions granted to you. For example, if the permissions you have been granted do not include creating, editing, and deleting asset records, then you can view asset records, but take no other actions on them.
    :::

## Assets landing page
To access the Manage Assets feature, navigate to **Service Management > Assets**. A tiled Assets dashboard is displayed, showing the available asset types. Clicking on any of the tiles displays an asset list with all the assets belonging to that type.

## Assets list
The Assets list lets you access all the available assets. <!--The following features are available to help you locate your assets and view and export information about these assets.-->

### Toolbar features
This section describes the actions you can take using the toolbar in the assets list.
<br>

![Toolbar in assets list](/_books/servicemanager-user-guide/asset-management/images/toolbar-in-assets-list.png)
* **Quick filter.** Use this filter to quickly focus on those asset records that are important to you. The filter operates on the asset records in the current list and returns records where a match is found in any of the asset attributes.

    To search on the [class-specific attributes](/servicemanager-config/assets/asset-structure#asset-classes) of an asset record, you must be viewing a class-specific list. The quick filter searches all asset attributes regardless of whether the attribute is displayed in your list view. The filter does not operate on attributes containing a date-time value, state, location type, acquisition method, or depreciation method. (You can, however, sort on these columns to identify the records of interest).

* **Advanced search.** Click **Advanced** (the search button to the right of the quick filter) to filter assets based on one or more conditions that you define. <!--Before adding your first condition, make sure you select the appropriate asset class from the class selector. -->Once you start adding the first condition, the asset class will be locked to the current asset class and the matching fields for that asset class will be available when adding conditions. Once conditions are set, use the quick filter to filter the results, or save the search as one of your views.
<!--* **Class selector.** Switch between Asset Classes or All Assets by selecting the relevant option. (Note that the list columns will change to reflect those configured for each asset class).-->
* **Create assets.** See [Creating assets manually](/servicemanager-user-guide/asset-management/assets#creating-assets-manually).
* **Delete assets.** See [Deleting assets](/servicemanager-user-guide/asset-management/assets#deleting-assets).
* **Copy assets.** See [Copying assets](/servicemanager-user-guide/asset-management/assets#copying-assets).
* **Bulk update.** See [Doing bulk updates](/servicemanager-user-guide/asset-management/assets#doing-bulk-updates).
* **Reload list.** To manually refresh the assets list, click **Reload list**.
* **Views.** See [Adding views of assets](/servicemanager-user-guide/asset-management/assets#adding-views-of-assets).
* **Export List.** See [Exporting the assets list](/servicemanager-user-guide/asset-management/assets#exporting-the-assets-list).<!--* **Home View.** Click **Home View** > **Set current view as my Home** to create a preferred or default view of your Assets List. Your Home View is displayed when you first visit your Assets List, and with a single click you can return to your Home View from any other filter or view that you have applied.-->
* **Table Configuration.** See [Displaying columns in the assets list](/servicemanager-user-guide/asset-management/assets#displaying-columns-in-the-assets-list).

### List features
* **Column sorting.** On each column header, you can re-order the list by clicking the column name.
* **View an asset.** Each asset in the list contains links to open the asset details and the type details.

## Creating assets manually
You can add an asset individually, or you can add assets in bulk.

If you are creating assets in bulk, the batch will include one new asset (per your configuration in the New Asset dialog), plus copies of that asset.

![Creating assets in bulk](/_books/servicemanager-user-guide/asset-management/images/bulk-create-asset.png)

**To create one or more assets manually:**
1. Click **+ New Asset**.
    ::: note
    If your Asset Management Admin has enabled partitioning on your Hornbill instance, then in the New Asset dialog, from the dropdown, select a partition to create the asset(s) in, or keep the default (Un-partitioned Assets).
    :::
1. From the dropdown, select the asset type of the asset(s) you want to create.
1. Enter a name for the asset(s).
    * If you are creating a single asset, click **Create & Open**.
    * If you are creating multiple assets, click **Create & Open > Bulk create asset**.
    * If you are creating multiple assets, in the Bulk Create Asset dialog, enter the number of copies you want.
1. Click **Create**.
1. In the dialog, when you receive confirmation, click **Close**.

:::tip
* Another way to add multiple assets as a batch is by using the [Upload Assets CSV](/servicemanager-config/assets/upload-assets).
* You can do automated processing using an external data source via the [Hornbill Asset Import utility](/data-imports-guide/assets/overview).
:::

## Deleting assets
The **Delete** button is invisible until at least one asset has been selected using the multi-select checkboxes.

**To delete one or more assets:**
1. Select one or more assets.
1. Click **Delete**.
:::tip
To select multiple assets, click on one asset, and then while holding down the Shift key, select another asset. All assets between these two assets will be selected and available for deleting.
:::

## Copying assets
The **Copy** button is invisible until one and only one asset has been selected using the multi-select checkboxes.

**To copy an asset:**
1.	In the Assets list, select the checkbox for an asset, then click the **Copy** button.
1.	In the Copy Asset dialog, enter a number for how many copies you want to create.
1.	Click **Duplicate**.
1.	When you are finished reading the confirmation message, click **Close**.

## Doing bulk updates
You can make changes to multiple asset records at once. You can update shared asset fields across assets of any type from the asset list.

* **Common (shared) fields.** These can be updated across mixed asset types.
* **Class-specific fields.** These can be updated when all selected assets share the same class.

![Creating assets in bulk](/_books/servicemanager-user-guide/asset-management/images/bulk-update-asset.png)

**To do a bulk update:**
1.	In the Assets list, select the checkbox for the assets you want to update, or to select the whole list, select the **Select All** checkbox at the top. 
1.	Make changes as necessary.

    1.	From the Asset Bulk Update dialog, from the dropdown, select one or more fields that you want to change. For each one, click **Add Field**.
    1.	When you are finished making changes to fields, run the update by clicking one of the two **Update** buttons:
        * **Batch Update.** This update is very fast. It performs a direct database write.
        * **Audited Update.** This is an API update that is slightly slower, but still fast. This one updates assets one at a time, creating a full audit history, including who made the change, when it occurred, and what data was modified.

## Adding views of assets
You can define and store a number of different views of the assets.

**To define views of assets:**
1. Click **Views > Add New**.
1. In the Create New View dialog, in the Criteria tab, you can specify conditions based on information held in the asset records.
1. In the Columns tab, select the columns you want to show in your view. 
1. When finished, click **Save**.
    
Now you can quickly access particular sets of important data by selecting from your list of defined views.

## Exporting the assets list
Export the contents of the assets list to CSV. Choose which of the available columns on the list you wish to export (the available options are specific to the asset class).

**To export the assets list:**
1. Click the **Export** button (the down arrow).
1. In the dialog, in the Columns tab, select the columns you want to export.
1. In the Settings tab, specify the export format and the number of records to export.
1. When finished, click **Export**.

## Displaying columns in the assets list
The available columns are specific to the asset type the list is using. The available columns are a combination of the common attributes that all asset types share, and the type-specific attributes for the selected asset type. If you choose to display all assets, only the shared asset attributes will be available to select from.

**To configure the display of columns in the assets list:**
1. Click the cog icon next to the down arrow.
1. In the Table Configuration dialog, in the Visibility tab, select the columns you want to show.
1. In the Order tab, drag and drop the columns into your preferred order.
1. In the Settings tab, use the dropdown to set the row density.
1. When finished, click **Close**.