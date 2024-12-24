# Asset Details
The Asset record will display the configured asset attributes for the given asset type, users with the appropriate rights can edit the attributes of the asset. It is possible to link assets to other assets, services and documents, and add attachments. In conjunction with Configuration Manager, it is also possible to schedule activities against the asset, collaborate on the asset timeline, follow the asset and graphically view the relationships the asset has to other entities.

## Asset Actions
* **Update**<br>The update action will be visible if Configuration Manager has been installed on your instance and the asset is marked as In Policy. Use the update action to post to the asset's timeline, and collaborate on the asset with other users.
* **Link**<br>This Action Item lets you search and link this asset with an existing request within Service Manager.
* **Assets**<br>Link this asset to other related or connected assets.
* **Attachments**<br>Upload files and documents from your local file system.
* **Service**<br>Link to a service that is supported by this asset.
Associating which services an asset supports or underpins can support quicker Incident and or Problem resolutions by making it quick and easy to understand what infrastructure is directly used to provide each service. Change management can benefit from visualizing which Services will be impacted when implementing changes to an asset, where the asset is linked to and supports/underpins one or multiple services.
* **Documents**<br>Link to documents that are stored in Hornbill Document Manager.

## Asset History
View all changes to the asset's attributes by clicking on the History icon.

The asset's Audit History will list actions, including who performed the action.

* **Search**<br>Search on field, from, and to columns.
* **Relationships**<br>Show changes in relationships between this asset and other entities within Hornbill.
* **Generate PDF**<br>Create a PDF document of the audit history. This will automatically be downloaded to your local computer. The document is split into sections for details and relationships.
* **Print**<br>Print the contents of the audit history to a printer.

## Summary
A Summary section maybe visible on the right-hand side of the asset details view. The attributes displayed in the summary section are configurable per asset type and can be managed by the asset administrator, alongside deciding which asset attributes to make visible per asset type, and which asset attributes are mandatory. This is covered in more detail under Asset Types

## Asset Details
View the assets attributes.

The Assets are broken down into logical groupings, which will be specific to the asset type and asset class the asset belongs to.

### Updating/Editing an Asset
To edit an asset's attributes or asset image, select Edit, Make the changes you need and then select the Save button to confirm the changes.

* **Asset Attribute Lookups**<br>Certain Attribute fields will be free text, others will be lookup fields, guidance is given on the key lookup fields below:
    * **Used by**<br>An asset can either be used by a single active user (not contacts), or if the Enable Sharing option is enabled, the used by will display as Shared and a new Shared With option will appear allowing the asset to be shared with multiple users, contacts, internal groupings and external organizations. If an asset is shared, it will appear as a selectable asset on requests and progressive capture asset forms for those it has been shared with.
    * **Owned by**<br>User look up based on active user accounts (not contacts). The users returned in the Owned By look-up will be based on the Company Group specified in the Company field if this is already populated.
    * **Site**<br>The list of sites defined in the Configuration. The list will be filtered by sites linked to a Company Group, if the Company field is already populated.
    * **Company**<br>List of defined Company Groups set up in the Configuration console, under Organization Data.
    * **Vendor**<br>Software Class specific, lookup is defined from Vendors created from the Manage Asset Types and Manage Vendors, Products, Versions button on the Software Asset Class.
    * **Product**<br>Software Class specific, lookup is filtered based on the previously chosen Vendor field. Products are created from the Manage Asset Types and Manage Vendors, Products, Versions button on the Software Asset Class.
    * **Version**<br>Software Class specific, lookup is filtered based on the previously chosen Product field. Versions are created from the Manage Asset Types and Manage Vendors, Products, Versions button on the Software Asset Class.

### Attachments
View, edit the description of, or remove any attachments associated to the asset

### Linked Entities
If the asset has been linked to other entities in Hornbill, they will be visible in the linked entities section
* **Linked Requests**<br>View all requests the asset has been linked too
* **Assets**<br>View any other linked assets (launch a graphical view if configuration manager is installed)
* **Services**<br>View any services the asset is linked too
* **Documents**<br>View, Download or unlink any documents the asset is linked too

## Timeline
Collaborate on and follow assets. The Timeline will be visible on an asset view if Configuration Manager is installed and the asset is marked as under policy.

## Tags
Tags provide a way to specify key words or attributes on an Asset for easy searching for this asset and any other asset using the same tag.

* **Adding a Tag**<br>To add a tag, simply start typing the tag that you wish to add. As you type, existing tags that match will be displayed and can be selected. There are two modes available that control if a user can add their own tags or if the predefined tags must be used.
* **Conditions**<br>Within both the Advanced Filter and the View Criteria on the Asset List, you can add a condition to filter your asset list based on one or more tags
* **Global Search**<br>The Global Search contains two search options. Search by Name and Description (default) or by Tags. Selecting the Tag search will provide a list of results based on the tags provided.

## Activities
Schedule and Manage asset activities such as reviews and PAT testing. The Activities option will be visible if Configuration Manager is installed and the asset is marked as under policy.

## Custom Buttons
It maybe useful to link to external content, or launch 3rd party solutions from asset forms. Custom buttons can be added to asset forms to facilitate this by the asset administrators.

Add, Edit or Remove custom Buttons on the Asset form by using the Custom Buttons option.
* Add a New Custom Button by giving the Custom Button a name, invoke an iBridge option or define a URL to launch from the button by adding an asset attribute field as a variable you want to pass to the the URL.
* Example uses for Asset Custom Buttons may include launching a 3rd party online remote control application, or viewing further asset information held in a 3rd party discovery tool, or simply a link to the vendor's website for more information on the asset.
* Custom Buttons can be set to only show if certain conditions are met i.e. if the asset form being viewed is of a certain type or class, or if an attribute of the asset manages the given condition.