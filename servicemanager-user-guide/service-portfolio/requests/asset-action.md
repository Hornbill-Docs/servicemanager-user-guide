# Assets
The Assets Action within a request provides the ability to search for and associate assets to a request.

![Asset Action](/_books/servicemanager-user-guide/images/request-asset-action.png)

## Assets and Asset Types
From the Assets Action Item, you can use the drop-down to navigate between an Asset Search and an Asset Type search, giving you the ability to associate both individual assets and also associate a specific type of asset with a request.

### Assets
* **Used by**. If there is a customer associated with the request, any asset directly associated with the customer will be visible, with an option to link the asset to the request, or to show if a customer's assets are already linked to the request.
* **Shared with**. If there is a customer associated with the request, any asset shared with the customer directly or through a grouping or organization that they belong to will be visible, with an option to link the assets to the request or to show if the assets are already linked to the request.
* **Location**. If a location has been associated with the request, a free text search box will be available to find assets that are associated with the site. You can search using the asset's name, class or tag. Leave 
* **Service**. If a request is associated with a service, a free text search box will be available to find assets that are associated with a service. You can search using the asset's name, class or tag.
* **Search**. A free text search box will be available to search using the asset's name, class or tag. Additional filters include asset class, asset type, and an advanced filter option to search specific asset fields.

### Asset Type
* Switching the drop-down to the Asset Type provides you with a search field, where you can search for an asset type and use the Link option to associate the Asset Type with the request.

## Visibility
The default timeline visibility level is **Customer**.  When set to **Customer** the timeline entry for linking the asset to the request will be visible to the customer of the request when viewed in the Customer or Employee portals. You can change the visibility level to say team or owner before posting if you do not wish for the post to be visible on the timeline to the customer of the request.

### Application Setting
The default timeline visibility level can be changed by a Hornbill Administrator using the Service Manager Advanced Settings.
|Name|Description|Default Setting
|-|-|-|
|guest.ui.app.com.hornbill.servicemanager.operation.defaultVisibility.assets|Default timeline visibility value when associating an asset to a request|Customer|