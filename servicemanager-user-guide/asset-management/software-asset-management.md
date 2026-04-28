# Software Asset Management

View the installed software on your devices. Ratify installed software against license records held across all your vendors.

## Before you begin

The following role is required to view the Software Asset Management.

|Role|Description|
|---|---|
|Software Asset Management User|Needed to access the Software Asset Management views.|

## Filters

* **Select Vendor**: Use the dropdown to select a specific vendor to filter the list of installed software to only show products from that vendor.
* **Partitions**: If you have partitions set up, use the dropdown to select a specific partition to filter the list of installed software to only show products with assets in that partition.

## Installed software

### Installed software chart

The chart at the top of the page gives you a breakdown of the installed software by  product and the number of installations. The chart is interactive, so you can click on a specific product to view the [Software Product Details](#software-product-details).

### Installed software list

The list below the chart gives you a breakdown of the installed software by product, vendor, version, and the number of installs. You can click on a specific product to view the [Software Product Details](#software-product-details).

### Software product details

When you click on a specific product from either the chart or the list, you can view more details about that product in the right-hand side panel. This includes the vendor, version, and the devices it is installed on. You can also view any matching software assets that are held in the Service Manager asset repository for that product.

#### Installed On

The **Installed On** section shows the devices that the software product is installed on. This information is pulled through from the **Installed Software Information** section on the asset record for each device that has the software product installed.

#### Matched Software Assets

This list shows any software assets that are held in the Service Manager asset repository that match the product you have selected. This is based on the attributes you have configured for the software asset type. You can click on a specific asset to view the asset details.

<!-- #JA Needs reviewing to see where this belongs...
## View installed software per device

For asset types created under the Computer System or Mobile Device classes, an asset administrator can enable the Installed Software Information accordion section from the Manage Asset Types menu option. This exposes the Installed Software Information accordion section on any asset records of that asset type.

Data displayed:

* Software Product
* Vendor
* Version
* When Installed

## Manage vendors, products, and versions

For software assets, you can include the attributes for vendor, product, and version. To maintain an accurate set of data for each, here you can define lists of the vendors you work with, the products they provide, and any different versions that are available for each product.

Once the lists are defined, these are presented when adding an asset of the Software class and where you have configured the Software Asset Type to use the Vendor, Product and or Version attributes.

## Adding new vendors, products, and versions

From the Manage Asset Types menu option, click the **+** option on the Software Class title bar.

### Configuration options - Vendor

From the Vendor tab:

* New Vendor. Add the vendor name.
* Alias. Add an alias the vendor may also be known as/

Click **Create** add the vendor to the list of defined vendors.

### Configuration options - Product

From the Product tab:

* Vendor. Select the vendor to which the new product relates.
* New Product: Add the name of the new product.

Click **Create** to add the product to the list of defined products.

### Configuration options - Version

From the Version tab:

* Vendor. Select the vendor to which the new version of a product relates.
* Product. From the vendor's products, select the product to which the new version relates.
* New Version. Add the name of the new version.

Click **Create** to add the version to the list of defined versions for the specific product.

### Edit and delete vendors, products, and versions

* Edit. Click the pencil icon next to the item you wish to edit.
* Delete. Click the **Delete** button (trash can icon) next to the item you wish to delete. If assets are currently linked to the version, product, or vendor, you will not be able to delete the item.
-->
<!-- https://wiki.hornbill.com/index.php?title=Software_Asset_Management -->
<!-- https://wiki.hornbill.com/index.php?title=Manage_Vendors,_Products,_Versions -->

<!-- #JA - Not sure why this is here.  Need to find somewhere in config doc to add this to.

Import installed software

You can import installed software from devices from third-party discovery solutions in two ways:

* Using the [Hornbill Asset Import utility](/data-imports-guide/assets/overview).
* Directly from the Hornbill ITOM app using the scheduled [Asset Import job](/itom-user-guide/jobs/job-queue#creating-new-jobs)
    Do this for managed devices once discovered through the Hornbill ITOM app. (ITOM is a subscribable app, separate to the Service Manager app.)
-->>