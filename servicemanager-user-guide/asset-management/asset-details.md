# Asset record

<!-- #JA rename file to asset-record and add redirect -->

:::note
[[INCLUDE https://raw.githubusercontent.com/Hornbill-Docs/hdoc-library/main/hdoc-library/service-manager/new-assets-note.md]]
:::

The asset record provides a comprehensive overview of the asset's attributes, relationships, and history. The information displayed is based on the asset type and class, and can be configured by the asset administrator.

## Summary

The Summary section displays a overview of the most important asset attributes. The attributes displayed here are configurable and can be managed by the asset administrator. This includes deciding which asset attributes to make visible and which asset attributes are mandatory. This is covered in more detail in [Asset Types](/servicemanager-config/assets/manage-asset-types#summary-fields).

![Asset summary section](/_books/servicemanager-user-guide/asset-management/images/asset-record-summary.png)

Each attribute can be updated by clicking in the field and entering the new value. Changes are applied without having to click a save button. A revert option is available to return the field to its previous value.

## Details

The Details section provides a comprehensive view of all the asset's attributes, including those not displayed in the Summary section. The attributes are organized into logical groupings based on the asset type and class. This allows users to easily find and understand the information related to the asset.

![Asset details section](/_books/servicemanager-user-guide/asset-management/images/asset-record-details.png)

Each attribute can be updated by clicking in the field and entering the new value. Changes are applied without having to click a save button. A revert option is available to return the field to its previous value.

## Services

Link to a service that is supported by this asset.

Associating the services an asset supports or underpins can support quicker resolution of incidents and problems by making it quick and easy to understand which infrastructure is directly used to provide each service. Change management can benefit from visualizing which services will be impacted when implementing changes to an asset, where the asset is linked to, and if it supports one or more services.

![Asset services section](/_books/servicemanager-user-guide/asset-management/images/asset-record-services.png)

## Assets

Link this asset to other related or connected assets. For example, you may want to link a laptop asset to the monitor and docking station assets that are used with it. Or you may want to link a software asset to the hardware asset it is installed on.

![Asset linked assets section](/_books/servicemanager-user-guide/asset-management/images/asset-record-assets.png)

## Requests

View any requests that this asset is linked to. This includes any requests that have been linked to the asset from the request form. Linking assets to requests can be done to provide more context to the request, and to allow for better reporting on the assets that are most commonly linked to requests. For example, if a particular model of laptop is frequently linked to incident records, this may indicate a common issue with that model that needs to be addressed.

![Asset linked requests section](/_books/servicemanager-user-guide/asset-management/images/asset-record-requests.png)

## Attachments

Upload files and documents from your local file system. Attachments can be added to the asset record to provide additional context and information about the asset. For example, you may want to attach a copy of the purchase receipt, or a document containing the asset's specifications.

![Asset attachments section](/_books/servicemanager-user-guide/asset-management/images/asset-record-attachments.png)

## Asset history

View all changes to the asset's attributes by clicking on the **History** icon.

The asset's audit history lists all actions, and who performed the action.

* **Search**: Search on **Field**, **From**, and **To** columns.
* **Relationships.** Show changes in relationships between this asset and other entities within Hornbill.
* **Generate PDF.** Create a PDF document of the audit history. This automatically downloads to your local computer. The document is split into sections for details and relationships.
* **Print.** Print the contents of the audit history to a printer.

![Asset history](/_books/servicemanager-user-guide/asset-management/images/asset-record-history.png)

## Used by vs Shared with

An option is available to toggle between the asset being used by a single user or shared among multiple users.

![Used by vs Shared with toggle](/_books/servicemanager-user-guide/asset-management/images/asset-record-used-by.png)

### Used by

When the asset is set to **Used By** the used by field indicates the primary user of the asset. This is typically used for assets that are assigned to a specific individual, such as a laptop or mobile phone.

### Shared with

When the asset it set to **Shared with**, the asset can be shared between multiple users. This is typically used for assets that are not assigned to a specific individual, such as a conference room or a shared printer.

## Tags

Tags provide a way to specify keywords or attributes on an asset for easy searching.

* **Adding a Tag**: To add a tag, start typing the tag that you wish to add. As you type, existing tags that match will be displayed and can be selected. There are two modes available that control if a user can add their own tags or if the predefined tags must be used.
* **Conditions**: Within both the Advanced Filter and the View Criteria on the asset list, you can add a condition to filter your asset list based on one or more tags.
* **Global Search**: The Global Search contains two search options. Search by Name and Description (default) or by Tags.

## Custom buttons

Customizable actions for an asset can be added through what is known as custom buttons.  The availability of custom buttons may vary on each asset.

Asset administrators can add [custom buttons](/esp-config/customize/custom-buttons) to asset records that open a URL, displays a popup, or runs an Auto Task workflow. s

![Custom buttons on an asset record](/_books/servicemanager-user-guide/asset-management/images/asset-record-custom-buttons.png)

Example uses for asset custom buttons may include:

* Launching a third-party online remote control application.
* Viewing further asset information held in a third-party discovery tool.
* Link to the vendor's website for more information on the asset.
* Running an Auto Task workflow to preform a specific action on the asset.

Custom buttons can be set to only show if certain conditions are met, for example if the asset has a certain status or if a particular user is viewing the asset record.

<!-- #JA Items for review 

* **Asset Attribute Lookups.** Certain attribute fields will be free text, others will be lookup fields. Guidance is given on the key lookup fields that follow.
  * **Used by.** An asset can either be used by a single active user (not a contact), or if the Sharing option is enabled. The used asset by will display as shared and a new Shared With option will appear, allowing the asset to be shared with multiple users, contacts, internal groupings, and external organizations. If an asset is shared, it will appear as a selectable asset on requests and Intelligent Capture asset forms for those it has been shared with.
  * **Owned by.** User lookup based on active user accounts (not contacts). The users returned in the Owned By lookup will be based on the Company Group specified in the Company field if this is already populated.
  * **Site.** The list of sites defined in Configuration. The list will be filtered by sites linked to a Company Group if the Company field is already populated.
  * **Company.** List of defined Company Groups set up in  Configuration, under Organization Data.
  * **Vendor.** Software-class specific, lookup is defined from vendors created from the Manage Asset Types and Manage Vendors, Products, Versions button on the Software Asset Class.
  * **Product.** Software-class specific, lookup is filtered based on the previously chosen Vendor field. Products are created from the Manage Asset Types and Manage Vendors, Products, Versions button on the Software Asset Class.
  * **Version.** Software-class specific, lookup is filtered based on the previously chosen Product field. Versions are created from the Manage Asset Types and Manage Vendors, Products, Versions button on the Software Asset Class.

  ### Linked entities

If the asset has been linked to other entities in Hornbill, they will be visible in the Linked Entities section.

* **Linked Requests.** View all requests the asset has been linked to.
* **Assets.** View any other linked assets.
* **Services.** View any services the asset is linked to.
* **Documents.** View, download or unlink any documents the asset is linked to.

## Timeline

Collaborate on and follow assets. The timeline will be visible on an asset view if Configuration Manager is installed and the asset is marked as under policy.

## Activities

Schedule and manage asset activities such as reviews and PAT testing. The Activities option will be visible if Configuration Manager is installed and the asset is marked as under policy.

-->