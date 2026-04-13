---
layout: article-toc
---
# Assets overview

:::note
[[INCLUDE https://raw.githubusercontent.com/Hornbill-Docs/hdoc-library/main/hdoc-library/service-manager/new-assets-note.md]]
:::

Use asset management to capture and detail information for your organization's assets. This process includes tracking ownership, costs, relationships, and the life cycle of assets to support strategic decision-making for your IT environment.

Hornbill Service Manager Asset Management records hardware and software inventory information. This data helps IT teams support asset users and make informed decisions about hardware and software purchases and redistribution.

Assets form the foundation of a Configuration Management Database (CMDB). You can use assets within Incident, Problem, and Change processes to assist with incident classification, impact analysis, and change planning.

## Before you begin

To manage assets, you must have one of the following roles and rights:

* The **Asset Management User** role, including the `View Asset Management` application right and either the `Create Assets` or `Edit Assets` right.
* A custom role that includes the `View Asset Management` application right and either the `Create Assets` or `Edit Assets` right.

:::important
If asset records are [in a partition set up by your assets admin](/servicemanager-config/assets/manage-partitions), your actions are limited to your granted permissions. If your permissions do not include creating, editing, or deleting, you can only view those records.
:::

## Key features

* **Manage assets**: Access and update your organization's assets in one central location.
* **Bulk update assets**: Update a field across multiple assets simultaneously.
* **Assets under warranty**: View assets based on their warranty status.

## Accessing Assets

From the left-hand application bar, select **Service Management** > **Assets**.

## Partition selector

An [asset partition](/servicemanager-config/assets/manage-partitions) is a group of assets where the access is restricted to selected users or groups. If asset partitions have been set up, you can select a partition to view the assets within it. Any asset not belonging to a partition can be viewed by selecting the **Un-partitioned assets** option.

![Partition selector](/_books/servicemanager-user-guide/images/assets-partition-selection.png)

## Asset views

Three views are available to display assets: **Dashboard**, **All assets**, and **Assets under warranty**. You can switch between views by selecting the desired view from the navigation bar.

![Assets views](/_books/servicemanager-user-guide/images/assets-views.png)

### Dashboard

The Assets dashboard displays tiles for available [asset types](/servicemanager-config/assets/manage-asset-types). Click any tile to display a list of all assets belonging to that type.

* **Current**: Assets with this status are existing assets but are not currently in use.
* **Active**: Assets with this status are currently in use.
* **Archived**: Assets with this status are no longer in use and have been archived.
  ![Assets dashboard](/_books/servicemanager-user-guide/images/assets-dashboard.png)

### All assets

The All assets view displays all assets for the selected partition.

### Assets under warranty

The Assets under warranty view displays assets that are currently under warranty for the selected partition.

## Asset type navigation

Assets are categorized by type, such as hardware or software. You can navigate to a specific asset type to view and manage assets of that type.
