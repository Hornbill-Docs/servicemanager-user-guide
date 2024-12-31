# Asset Details
The asset record displays the configured asset attributes for the given asset type. Users with the appropriate rights can edit the attributes of the asset. You can link assets to other assets, services and documents, and add attachments. 

In Configuration, you can schedule activities against the asset, collaborate on the asset timeline, follow the asset, and graphically view the relationships the asset has to other entities.

## Asset actions
* **Update.** The update action is visible if Configuration Manager has been installed on your instance and the asset is marked as In Policy. Use the update action to post to the asset's timeline and collaborate on the asset with other users.
* **Link.** This action item lets you search and link this asset with an existing request within Service Manager.
* **Assets.** Link this asset to other related or connected assets.
* **Attachments.** Upload files and documents from your local file system.
* **Service.** Link to a service that is supported by this asset.

    Associating the services an asset supports or underpins can support quicker resolution of incidents and problems by making it quick and easy to understand which infrastructure is directly used to provide each service. Change management can benefit from visualizing which services will be impacted when implementing changes to an asset, where the asset is linked to, and if it supports one or more services.

* **Documents.** Link to documents that are stored in Hornbill Document Manager.

## Asset history
View all changes to the asset's attributes by clicking on the **History** icon.

The asset's audit history lists all actions, and who performed the action.

* **Search.** Search on Field, From, and To columns.
* **Relationships.** Show changes in relationships between this asset and other entities within Hornbill.
* **Generate PDF.** Create a PDF document of the audit history. This automatically downloads to your local computer. The document is split into sections for details and relationships.
* **Print.** Print the contents of the audit history to a printer.

## Summary
A Summary section may be visible on the right-hand side of the Asset Details view. The attributes displayed in the summary are configurable per asset type and can be managed by the asset administrator. This includes deciding which asset attributes to make visible per asset type, and which asset attributes are mandatory. This is covered in more detail in [Asset Types](/servicemanager-user-guide/asset-management/manage-asset-types).

## Asset details
View the assets' attributes.

The assets are broken down into logical groupings, which are specific to the asset type and asset class the asset belongs to.

### Updating an asset
**To edit an asset's attributes or asset image:**
1. Click **Edit**.
1. Make the changes you need.
1. Click **Save**.

* **Asset Attribute Lookups.** Certain attribute fields will be free text, others will be lookup fields. Guidance is given on the key lookup fields that follow.
    * **Used by.** An asset can either be used by a single active user (not a contact), or if the Sharing option is enabled. The used asset by will display as shared and a new Shared With option will appear, allowing the asset to be shared with multiple users, contacts, internal groupings, and external organizations. If an asset is shared, it will appear as a selectable asset on requests and Intelligent Capture asset forms for those it has been shared with.
    * **Owned by.** User lookup based on active user accounts (not contacts). The users returned in the Owned By lookup will be based on the Company Group specified in the Company field if this is already populated.
    * **Site.** The list of sites defined in Configuration. The list will be filtered by sites linked to a Company Group if the Company field is already populated.
    * **Company.** List of defined Company Groups set up in  Configuration, under Organization Data.
    * **Vendor.** Software-class specific, lookup is defined from vendors created from the Manage Asset Types and Manage Vendors, Products, Versions button on the Software Asset Class.
    * **Product.** Software-class specific, lookup is filtered based on the previously chosen Vendor field. Products are created from the Manage Asset Types and Manage Vendors, Products, Versions button on the Software Asset Class.
    * **Version.** Software-class specific, lookup is filtered based on the previously chosen Product field. Versions are created from the Manage Asset Types and Manage Vendors, Products, Versions button on the Software Asset Class.

### Attachments
View, edit the description of, or remove any attachments associated to the asset.

### Linked entities
If the asset has been linked to other entities in Hornbill, they will be visible in the Linked Entities section.
* **Linked Requests.** View all requests the asset has been linked to.
* **Assets.** View any other linked assets.
* **Services.** View any services the asset is linked to.
* **Documents.** View, download or unlink any documents the asset is linked to.

## Timeline
Collaborate on and follow assets. The timeline will be visible on an asset view if Configuration Manager is installed and the asset is marked as under policy.

## Tags
Tags provide a way to specify keywords or attributes on an asset for easy searching.

* **Adding a Tag.** To add a tag, start typing the tag that you wish to add. As you type, existing tags that match will be displayed and can be selected. There are two modes available that control if a user can add their own tags or if the predefined tags must be used.
* **Conditions.** >Within both the Advanced Filter and the View Criteria on the asset list, you can add a condition to filter your asset list based on one or more tags.
* **Global Search.** The Global Search contains two search options. Search by Name and Description (default) or by Tags.

## Activities
Schedule and manage asset activities such as reviews and PAT testing. The Activities option will be visible if Configuration Manager is installed and the asset is marked as under policy.

## Custom buttons
It may be useful to link to external content or launch third-party solutions from asset forms. Asset administrators can add custom buttons to asset forms to facilitate this.

Add, edit, or remove custom buttons on the asset form by using the Custom Buttons option.

**To add a new custom button:**
1. Give the custom button a name. 
1. Invoke an iBridge option, or define a URL to launch from the button by adding an asset attribute field as a variable you want to pass to the the URL.

Example uses for asset custom buttons may include launching a third-party online remote control application, or viewing further asset information held in a third-party discovery tool, or simply a link to the vendor's website for more information on the asset.

Custom buttons can be set to only show if certain conditions are met, for example if the asset form being viewed is of a certain type or class, or if an attribute of the asset manages the given condition.