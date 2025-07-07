# Assets
The Assets Action on a request provides the ability to search for [assets](/servicemanager-user-guide/asset-management/overview) and link them to the request.  Linking an asset that is related to an issue can help provide solutions faster and give a better understanding of where issues might be recurring.  Once an asset is linked, the details of that asset can be easily accessed.  Does the asset have any other outstanding issues?  Has there been a recent change to the asset? Is the asset linked to other important assets that might cause a greater impact?

![Asset Action](/_books/servicemanager-user-guide/images/request-asset-action.png)

## Before you begin
* **Is the asset action enabled on the service?** The asset action can be enabled or disabled for each request type under the [Service Configuration](/serviceemanager-user-guide/service-portfolio/request-configuration#request-actions). If you can’t see the asset action, this might be because the service owner has disabled this feature.

## Assets and Asset Types
From the Assets Action, you can use the drop-down to navigate between an Asset Search and an Asset Type search, giving you the ability to associate both individual assets and also associate a specific type of asset with a request.

### Assets
* **Used by**. If there is a customer associated with the request, any asset directly associated with the customer will be visible, with an option to link the asset to the request or to show if a customer's assets are already linked to the request.
* **Shared with**. If there is a customer associated with the request, any asset shared with the customer directly or through a grouping or organization that they belong to will be visible, with an option to link the assets to the request or to show if the assets are already linked to the request.
* **Location**. If a location has been associated with the request, a free text search box will be available to find assets that are associated with the site. You can search using the asset's name, class, or tag.
* **Service**. If a request is associated with a service, a free text search box will be available to find assets that are associated with a service. You can search using the asset's name, class or tag.
* **Search**. A free text search box will be available to search using the asset's name, class or tag. Additional filters include asset class, asset type, and an advanced filter option to search specific asset fields.

### Asset Type
* Switching the drop-down to the [Asset Type](/servicemanager-user-guide/asset-management/asset-structure#asset-types) provides you with a search field, where you can search for an asset type and use the Link option to associate the Asset Type with the request. This can be useful on change requests when applying a change to all the assets of a particular type, or if there is a known issue with a type of asset.

## Visibility
The default timeline visibility level is **Customer**.  When set to **Customer**, the timeline entry for linking the asset to the request will be visible to the customer of the request when viewed in the Customer or Employee portals. You can change the visibility level to **Team** or **Owner** before posting if you do not want the customer to be able to see the timeline entry and any comments that get added to it.

### Application Settings
The default timeline visibility level can be changed by a Hornbill Administrator using the [Service Manager Advanced Settings](/servicemanager-config/advanced-tools-and-settings/application-settings).

|Name|Description|Default Setting
|-|-|-|
|guest.ui.app.com.hornbill.servicemanager.operation.defaultVisibility.assets|Default timeline visibility value when associating an asset to a request|Customer|