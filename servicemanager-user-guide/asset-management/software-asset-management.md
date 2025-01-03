# Software Asset Management
Import and view the installed software on your devices. Ratify installed software against license records held across all your vendors.

## Roles
* **Software Asset Management User.** Needed to view the Software Asset Management views.
* **Asset Management Admin.** Needed to enable the Installed Software accordion view.


## Import installed software
You can import installed software from devices from third-party discovery solutions in two ways:
* Using the [Hornbill Asset Import utility](/data-imports-guide/assets/overview).
* Directly from the Hornbill ITOM app using the scheduled [Asset Import job](/itom-user-guide/jobs/job-queue#creating-new-jobs)
    Do this for managed devices once discovered through the Hornbill ITOM app. (ITOM is a subscribable app, separate to the Service Manager app.)

## View installed software
Here you can see software installed on devices in your estate/ Once installed software is imported against your hardware assets, the list will show all software with the following:
* Vendor
* Product
* Version
* Installs. This is the count of the number of devices the software is installed on.
* Software Assets. This is the count of any corresponding software asset records.
* Actions. Hover over the column to manually create a corresponding software asset record in the CMDB (to record license count, type, and date information).

Use the **Vendor** dropdown to filter the installed software list to see only that vendor's products.

### View which devices software is installed on
Highlight a software product in the list to open the right-hand side panel, which shows:

* Product Information
* Installed On. The devices the software product is installed on.
* Matching Software Assets. Any existing asset records of type *Software Asset* that match the software product.

### Add corresponding software license product
If you don't hold a corresponding software asset record for the installed software, you can manually add one. Hover over the Actions column for the corresponding software product in the list, and click **+ New Asset**.


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
* Product. Select the product, from the Vendors Products to which the New Version relates
* New Version. Add the name of the new version.

Click **Create** to add the version to the list of defined versions for the specific product.


### Edit and Delete Vendors, Products, and Versions
* Edit: Select the Pencil icon next to the item you wish to edit
* Delete: Select the Trash Can icon next to the item you wish to delete. If Assets are currently linked to the Version, Product or Vendor you will not be able to delete the item.

<!-- https://wiki.hornbill.com/index.php?title=Software_Asset_Management -->
<!-- https://wiki.hornbill.com/index.php?title=Manage_Vendors,_Products,_Versions -->