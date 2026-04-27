---
layout: article-toc
draft: false
---
# Asset list

:::note
[[INCLUDE https://raw.githubusercontent.com/Hornbill-Docs/hdoc-library/main/hdoc-library/service-manager/new-assets-note.md]]
:::

Asset lists are available when selecting the [All Assets view](/servicemanager-user-guide/asset-management/overview#asset-views) or when an [asset type](/servicemanager-user-guide/asset-management/overview#asset-navigation) is selected from the navigation panel.

![Asset list](/_books/servicemanager-user-guide/images/asset-list.png)

## Filter

![Filter in assets list](/_books/servicemanager-user-guide/images/asset-list-filter.png)

Use the filter to find specific asset records in your current list. This tool helps you locate the exact information you need by searching for matching values across asset attributes.

### Searchable attributes

The attributes available for filtering depend on your current view:

* **All Assets**: When you view the [All Assets](/servicemanager-user-guide/asset-management/overview#all-assets) list, the filter searches through common attributes shared by every asset type.
* **Asset Type**: When you select a specific asset type from the [Asset navigation panel](/servicemanager-user-guide/asset-management/overview#asset-navigation), the filter searches through both common attributes and attributes unique to that asset type.

### Excluded attributes

You cannot filter by the following attributes:

* Acquisition method
* Date-time values
* Depreciation method
* Location type
* State

## Advanced filter

![Advanced filter in assets list](/_books/servicemanager-user-guide/images/asset-list-advanced-filter.png)

The **Advanced** filter allows you to build one of more conditions to filter the list of assets. When more than one condition is added, all conditions must be met for an asset to be included in the results.

![Advanced filter conditions](/_books/servicemanager-user-guide/images/asset-list-advanced-filter-condition.png)

### Available identifiers

* **All Assets**: When the advanced filter is used in the [All Assets](/servicemanager-user-guide/asset-management/overview#all-assets) list, the available identifiers for building conditions are common attributes shared by every asset type.
* **Asset Type**: When the advanced filter is used in a specific asset type list, the available identifiers for building conditions include both common attributes and attributes unique to that asset type.

### Saving advanced filters as views

When you have built an advanced filter, you can save it as a **[View](#adding-views-of-assets)**. This allows you to quickly access the same set of conditions in the future without having to rebuild them each time.

## Creating new assets

![New Asset button](/_books/servicemanager-user-guide/images/assets-new-button.png)

You can add an asset individually, or you can add assets in bulk.

If you are creating assets in bulk, the batch will include one new asset (per your configuration in the New Asset dialog), plus copies of that asset.

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

1. In the Assets list, select the checkbox for an asset, then click the **Copy** button.
1. In the Copy Asset dialog, enter a number for how many copies you want to create.
1. Click **Duplicate**.
1. When you are finished reading the confirmation message, click **Close**.

## Doing bulk updates

You can make changes to multiple asset records at once. You can update shared asset fields across assets of any type from the asset list.

* **Common (shared) fields.** These can be updated across mixed asset types.
* **Class-specific fields.** These can be updated when all selected assets share the same class.

![Creating assets in bulk](/_books/servicemanager-user-guide/asset-management/images/bulk-update-asset.png)

**To do a bulk update:**

1. In the Assets list, select the checkbox for the assets you want to update, or to select the whole list, select the **Select All** checkbox at the top.
1. Make changes as necessary.

    1. From the Asset Bulk Update dialog, from the dropdown, select one or more fields that you want to change. For each one, click **Add Field**.
    1. When you are finished making changes to fields, run the update by clicking one of the two **Update** buttons:
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

## Home view

![Home view](/_books/servicemanager-user-guide/asset-management/images/asset-home-view.png)

The Home view defines which area of the assets is displayed when you first open assets.  The drown lets you set the current view as the Home view.  Clicking on the Home icon will take you back to this view at any time. This option is available from any list and on the dashboard.

## Exporting the asset list

Export the contents of the asset list to CSV. Choose which of the available columns on the list you wish to export (the available options are specific to the asset class).

**To export the asset list:**

1. Click the **Export** button (the down arrow).
1. In the dialog, in the Columns tab, select the columns you want to export.
1. In the Settings tab, specify the export format and the number of records to export.
1. When finished, click **Export**.

## Displaying columns in the asset list

The available columns are specific to the asset type the list is using. The available columns are a combination of the common attributes that all asset types share, and the type-specific attributes for the selected asset type. If you choose to display all assets, only the shared asset attributes will be available to select from.

**To configure the display of columns in the asset list:**

1. Click the cog icon next to the down arrow.
1. In the Table Configuration dialog, in the Visibility tab, select the columns you want to show.
1. In the Order tab, drag and drop the columns into your preferred order.
1. In the Settings tab, use the dropdown to set the row density.
1. When finished, click **Close**.
