---
layout: article-toc
---
# Manage asset types
Asset types allow you to define a grouping of particular types of assets that fall under the same class. Creating an asset type allows you to select the fields that will be available for that Asset Type. During the creation of an Asset, you will select the Asset Type to apply the defined fields against that asset.

## Default asset types
Service Manager provides a number of asset types by default so that you can quickly start adding your assets. You can select an asset type when you are manually adding an individual asset; you can also specify asset types as part of an import. The default asset types can be edited or deleted as necessary.

The default asset types include the following:
* Desktop
* Laptop
* Server
* Virtual machine
* Headset
* Keyboard
* Monitor
* Mouse
* Webcam
* Smartphone
* Tablet
* Printer
* Scanner
* Desktop app
* Mobile app
* Desk phone

## Managing asset types
**To add a new asset type:**
1. At the top right of the Asset Types page, click **+ New Asset Type**.
1. In the New Asset Type form, select an asset class for the new asset type.
1. Give the asset type a name and description.

### Asset type fields
* **Class.** The asset class influences the availability of additional asset properties. The additional properties are specific to the asset class selected.
* **Name.** A short descriptive name. This is displayed in lists and used for searches and reports. This name is applied to assets created under this asset type.
* **Prefix.** This is a three-character prefix that is automatically added to the asset ID.
* **Auto Generate Name.** When enabled, for any asset that is created under this asset type, the name will be automatically created and based on the asset ID. This  includes the prefix, if set.
* **Description.** A high-level description to help users understand more about the type and how it should be used.
* **Image.** An image can be added to provide a nice visual identifier of the asset type. Any asset created using this type will also use this image.

### Asset type attributes
Upon selecting an asset class, you will be presented with the attributes that will be available when adding your individual assets later.

Selecting a class exposes the properties. The general properties are common to all asset types. The additional properties are specific to the asset class specified when creating your new asset type.

Click one of the sections beneath the general properties or additional properties to expand the section and expose the attributes (fields) within that section. There are two settings against each attribute: *Visible* and *Mandatory*.

You can configure the following attributes:

* **Visible.** Use this setting to control whether the field is visible when viewing the details of an individual asset, for example, to hide fields that are not used.
* **Mandatory.** Use this setting to control whether information must be provided in the field when adding or editing an individual asset.

Once you are happy with the configuration of your asset type, click **Create** to finish.


### Deleting an asset type
**To delete an asset type:**
1. Hover over the type and click the **Delete** button (trash can icon). If there are assets associated to the type, you will be prevented from deleting it.

## About asset states and substates
Asset states tell you where an asset is in its lifecycle (e.g., *Current*, *Active*, *Archived*). With substates, you can add a customizable layer of detail within those states, allowing you to reflect more specific conditions or workflows.

For example:
* State: Current → Substate: In Stock (for assets awaiting allocation).
* State: Active → Substate: Allocated (for assets assigned to users).

The purpose of substates is to enhance tracking, searching, and reporting by providing more granularity, making it easier to manage assets based on their exact condition or stage.

Substates are global, so you can define them for each state across all asset classes/types. Then you have the flexibility to enable or disable substates for certain asset types, depending on your needs.

## Asset substates
You can manage substates using the configuration button on the top of the Asset Types list in the toolbar. The substates are available to all asset types, but they can be made visible or hidden for each asset type.

**To add an asset substate:**
1. In the toolbar of the Asset Types page, click **Manage Substates**.
1. Select one of the existing states (Current, Active, or Archived).
1. Give your new substate a name.

**To make an asset substate visible:**
1. From the Manage Asset Types option, open an asset type.
1. Click **Edit**.**
1. Expand the section called *General Asset Information*.
1. Select **Visible** if you don't want to hide the field.
1. Select **Mandatory** if information must be entered in the field.

## Asset type settings
Each asset type will contain a variety of fields based on the class selected when the asset type was created. These fields are contained within a number of sections that are determined by the class type. When each section is expanded, there are three options available to configure each field:

* **Summary.** Select this option to display the information stored in this field in a Summary section of the asset form. This is useful to present key information of the asset and it also provides easy access for editing.
* **Visible.** All the provided fields are part of the selected class. It might be that some of the fields are not required for the asset type; for fields not required, use this setting to turn off the visibility.
* **Mandatory.** Making a field mandatory ensures that it is populated by a user. If there is a field that has been set to mandatory but has not yet been populated, a user will be forced to enter a value for that field before any other changes can be saved.

<!-- https://wiki.hornbill.com/index.php?title=Asset_Types -->