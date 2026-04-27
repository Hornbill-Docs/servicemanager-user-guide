---
layout: article-toc
---
# Assets overview

:::note
[[INCLUDE https://raw.githubusercontent.com/Hornbill-Docs/hdoc-library/main/hdoc-library/service-manager/new-assets-note.md]]
:::

Use asset management to capture and detail information for your organization's assets. This includes tracking ownership, costs, relationships, and the life cycle of assets to support strategic decision-making for your IT environment.

Asset data helps IT teams support asset users and make informed decisions about hardware and software purchases and redistribution.

Assets form the foundation of a Configuration Management Database (CMDB). You can use assets within incident, problem, and change processes to assist with incident classification, impact analysis, and change planning.

## Before you begin

To manage assets, you must have one of the following roles and rights:

|Role|Description|
|---|---|
|Asset Management User|This role allows users to view and manage assets. It includes the `View Asset Management`, `Create Assets` and the `Edit Assets` application rights.|
|Custom role|A custom role can be created with the necessary application rights to view and manage assets. This allows for more granular control over who can access and modify asset information.|

## Accessing Assets

From the left-hand application bar, select **Service Management** > **Assets**.

## Partition selector

An [asset partition](/servicemanager-config/assets/manage-partitions) is a group of assets where the access is restricted to selected users or groups. If asset partitions have been set up, you can select a partition to view the assets within it. Any asset not belonging to a partition can be viewed by selecting the **Un-partitioned assets** option.

![Partition selector](/_books/servicemanager-user-guide/images/assets-partition-selection.png)

Each partition has its own set of permissions.  The ability to view, create, update, and delete assets within a partition will depend on the permissions that you have been given.

## Asset views

Three views are available to display assets: **Dashboard**, **All assets**, and **Assets under warranty**. You can switch between views by selecting the desired view from the navigation bar.

![Assets views](/_books/servicemanager-user-guide/images/assets-views.png)

### Dashboard

The Assets dashboard displays tiles for available [asset types](/servicemanager-config/assets/manage-asset-types). Click any tile to display a list of all assets belonging to that type.

* **Current**: Assets with this status are existing assets but are not currently in use.
* **Active**: Assets with this status are currently in use.
* **Archived**: Assets with this status are no longer in use and have been archived.

  ![Assets dashboard](/_books/servicemanager-user-guide/images/assets-dashboard.png)

#### Home view

![Home view](/_books/servicemanager-user-guide/asset-management/images/asset-home-view.png)

The Home view defines which area of the assets is displayed when you first open assets.  The drop-down lets you set the current view as the Home view.  Clicking on the Home icon will take you back to this view at any time. This option is available from any list and on the dashboard.

### All Assets

The All Assets view displays all assets for the selected partition in a flexible [Asset List](/servicemanager-user-guide/asset-management/asset-list)

### Assets under Warranty

The Assets under Warranty view displays assets that are currently under warranty for the selected partition. This view helps you quickly identify which assets are still covered by warranty, allowing you to manage maintenance and support effectively.

![Assets warranty expiry counter](/_books/servicemanager-user-guide/images/assets-warranty-expiry-counters.png)

## Asset navigation

Use the Assets navigation to browse assets by selecting from the list of available [asset types](/servicemanager-config/assets/manage-asset-types). Related asset types can be grouped under definable [categories](/servicemanager-config/assets/manage-asset-types#asset-categories) to make navigation easier. Selecting an asset type displays a [list](/servicemanager-user-guide/asset-management/asset-list) of all assets belonging to that type.

![Assets navigation](/_books/servicemanager-user-guide/images/assets-navigation.png)