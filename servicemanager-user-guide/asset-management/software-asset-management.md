# Software Asset Management
Import and view the installed software on our devices. Ratify installed software against license records held across all your vendors.

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
For Asset Types created under the Computer System and, or Mobile Device Classes, an Asset Administrator can enable the:

Installed Software Information accordion section from the Manage Asset Types menu option.
This will expose the Installed Software Information accordion section on any Asset Records, of that Asset Type.

Data displayed:
* Software Product
* Vendor
* Version
* When Installed

<!-- https://wiki.hornbill.com/index.php?title=Software_Asset_Management -->