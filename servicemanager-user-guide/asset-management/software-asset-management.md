# Software Asset Management

View the installed software on your devices. Ratify installed software against license records held across all your [vendors](/servicemanager-config/assets/software-suppliers).

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

![Installed software chart](/_books/servicemanager-user-guide/asset-management/images/sam-install-chart.png)

The chart at the top of the page gives you a breakdown of the installed software by  product and the number of installations. The chart is interactive, so you can select a specific product to view the [Software Product Details](#software-product-details).

### Installed software list

The list below the chart gives you a breakdown of the installed software by product, vendor, version, and the number of installs. You can select a specific product to view the [Software Product Details](#software-product-details).

### Software product details

When you select a specific product from either the chart or the list, you can view more details about that product in the right-hand side panel. This includes the vendor, version, and the devices it is installed on. You can also view any matching software assets that are held in the Service Manager asset repository for that product.

![Software product details](/_books/servicemanager-user-guide/asset-management/images/sam-product-information.png)

#### Installed On

The **Installed On** section shows the devices that the software product is installed on. This information is pulled through from the **Installed Software Information** section on the asset record that has the software product installed. You can select a specific asset to view the full asset record.

When viewing an asset record that has software products installed, an Installed Software list will be displayed.

![Installed Software list](/_books/servicemanager-user-guide/asset-management/images/sam-asset-installed-software-list.png)

#### Matched Software Assets

This list shows any software assets that are held in the Service Manager asset repository that match the product you have selected. You can select a specific software asset to view the full software asset record.
