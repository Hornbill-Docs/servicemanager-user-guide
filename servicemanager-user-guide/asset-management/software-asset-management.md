# Software Asset Management
Import and view the installed software on your devices. Ratify installed software against license records held across all your vendors.

## Roles
* **Software Asset Management User**<br>Needed to view the Software Asset Management views
* **Asset Management Admin**<br>Needed to enable the Installed Software accordion view for required 


## Import Installed Software - List
Import installed software from devices from third-party discovery solutions using the Asset_Data_Import_Tool, or directly from the Hornbill ITOM App using the scheduled Asset Import job; do this for managed devices once discovered through the Hornbill ITOM app (ITOM is a subscribable App, separate to the Service Manager App).

## View Installed Software
Software installed on devices in your estate - Once installed software is imported against your hardware assets, the list will show all software with the following:
* Vendor
* Product
* Version
* Installs - The count of the number of devices the software is installed on
* Software Assets - The count of any corresponding Software Asset Records
* Actions - Hover over the column to manually create a corresponding Software Asset Record in the CMDB (to record license count, type, date information)

Use the Vendor drop down to filter the installed software list, to only that vendor's products

### View which Devices Software is Installed On
Highlight a software product in the list, to view the right hand side panel, which will show:

* Product Information
* Installed On - which devices the software product is installed on
* Matching Software Assets - Any existing asset records of type Software Asset which match the software product

### Add Corresponding Software License Product
If you don't hold a corresponding Software Asset Record for the installed software, you can manually add one, by hovering over the Actions column for the corresponding software product in the list, and choose `+ New Asset`


## View Installed Software per Device
For Asset Types created under the Computer System and, or Mobile Device Classes, an Asset Administrator can enable the Installed Software Information accordion section from the Manage Asset Types menu option. This will expose the Installed Software Information accordion section on any Asset Records, of that Asset Type.

Data displayed:
* Software Product
* Vendor
* Version
* When Installed

## Manage Vendors, Products, and Versions
For Software Assets it is possible to include the attributes for Vendor, Product and Version. In order to maintain an accurate set of data for each it is possible to define lists of the Vendors you work with, the Products they provide and any different Versions which are available for each product.

Once the Lists are defined these will be presented when adding an Asset of the Software Class and where you have configured the Software Asset Type to use the Vendor, Product and or Version attributes.

## Adding New Vendors, Products, and Versions
From the Manage Asset Types menu option select the + option on the Software Class title bar.

### Configuration Options - Vendor

From the Vendor tab:
* New Vendor: Add the Vendor Name
* Alias: Add an Alias the Vendor may also be known as

Choose Create To add the Vendor to the list of defined Vendors.

### Configuration Options - Product
From the Product tab:

* Vendor: Select the Vendor to which the New Product relates
* New Product: Add the New Product Name

Choose Create To add the Product to the list of defined Products.

### Configuration Options - Version
From the Version tab:

* Vendor: Select the Vendor to which the new version of a Product relates
* Product: Select the Product, from the Vendors Products to which the New Version relates
* New Version: Add the New Version Name

Choose Create To add the Version to the list of defined Versions for the specific Product.


### Edit and Delete Vendors, Products, and Versions
* Edit: Select the Pencil icon next to the item you wish to edit
* Delete: Select the Trash Can icon next to the item you wish to delete. If Assets are currently linked to the Version, Product or Vendor you will not be able to delete the item.

<!-- https://wiki.hornbill.com/index.php?title=Software_Asset_Management -->
<!-- https://wiki.hornbill.com/index.php?title=Manage_Vendors,_Products,_Versions -->