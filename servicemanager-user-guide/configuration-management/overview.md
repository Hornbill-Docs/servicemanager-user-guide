---
layout: article-toc
---
# Configuration Management
Configuration Management consists of a Configuration Item (CI) list and a graphical explorer used for browsing related CIs. These tools are used to configure and visualize your CMDB. Quickly view the relationships between assets, request, users, and more.


## Configuration Items
Configuration Manager allows you to manage different Configuration Items in Hornbill. Configuration Items are:

* Assets
* Requests
* Co-workers
* Documents
* Services

## Configuration Item Policy List
The CI Policy List is accessed when selecting Configuration Manager from the application bar. The CI List offers the following features

* **CI Type selector**<br>Filter the list by Service or Asset, if selecting Asset, filter the list further by Asset Class and Type.
* **Filter**<br>Search for a specific CI.
* **Policy Filter**<br>Show all CI's, those in and out of policy.

## Configuration Item Explorer
The CI Explorer provides a graphical representation of associated or linked CIs. The CI Explorer can be opened from the CI List or by using on of the Configuration Manager plug-ins.

### Tool Bar

* **Select Impact**<br>Only show CIs that match the selected Impact level.
* **In Policy / Not in Policy**<br>Only display CIs that are either In Policy or Not in Policy.
* **CI Type Filters**<br>Use the CI Filters to hide or show the different types of CIs in the Explorer
* **Launch Explorer**<br>This option will put the selected CI at the root of the CI Explore. This option will only be available when a downstream CI is selected.
* **Legend**<br>Opens a popup that describes the meaning of the different colors represented in the Explorer view.
* **Show / Hide Details**<br>This option will collapse or expand the right hand side information panel.

## Accessing
Configuration Management can be accessed from a number of forms within the Service Manager app. These include the following

* **Request Form**<br>Launch the CI Explorer directly from any request form. This will put the request as the focus of the explorer and allow you to visualize the related CIs associated to this request.
* **Asset Form**<br>Launch the CI Explorer directly from any asset form. This will put the asset as the focus of the explorer and allow you to visualize the related CIs to this asset.
* **Services Form**<br>Launch the CI Explorer directly from any Service form. This will put the Service as the focus of the explorer and allow you to visualize the related CIs to this
* **Asset Timeline**<br>Assets marked as In Policy will have a timeline enabled for collaborating on the Asset.
* **Asset Activities**<br>Assets marked as In Policy will have activities enabled, allowing for the scheduling of activities such as reviews, maintenance, patching etc.