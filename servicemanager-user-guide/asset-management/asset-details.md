# Asset record

<!-- #JA rename file to asset-record and add redirect -->

:::note
[[INCLUDE https://raw.githubusercontent.com/Hornbill-Docs/hdoc-library/main/hdoc-library/service-manager/new-assets-note.md]]
:::

The asset record provides a comprehensive overview of the asset's attributes, relationships, and history. The asset record is organized into several sections, each providing different types of information about the asset.

## Summary

The Summary section displays an overview of the most important asset attributes. The attributes displayed here are configurable and can be managed by the asset administrator. This includes deciding which asset attributes to make visible and which asset attributes are mandatory. This is covered in more detail in [Asset Types](/servicemanager-config/assets/manage-asset-types#summary-fields).

![Asset summary section](/_books/servicemanager-user-guide/asset-management/images/asset-record-summary.png)

Each attribute can be updated by selecting the field and entering the new value. Changes are applied without having to select a save button. A revert option is available to return the field to its previous value.

## Details

The Details section provides a comprehensive view of all the asset's attributes, including those not displayed in the Summary section. The attributes are organized into logical groupings, allowing you to easily find and understand the information related to the asset.

![Asset details section](/_books/servicemanager-user-guide/asset-management/images/asset-record-details.png)

Each attribute can be updated by selecting the field and entering the new value. Changes are applied without having to select a save button. A revert option is available after making a change to return the field to its previous value.

## Services

Link to a [service](/servicemanager-user-guide/service-portfolio/services/overview) that is supported by this asset.

Associating the services an asset supports or underpins can provide quicker resolution of incidents and problems by making it easy to understand which assets are used to provide each service. Change management can benefit from visualizing which services will be impacted when implementing changes to an asset, where the asset is linked to, and if it supports one or more services.

![Asset services section](/_books/servicemanager-user-guide/asset-management/images/asset-record-services.png)

## Assets

Link this asset to other related or connected assets. For example, you may want to link a laptop asset to the monitor and docking station assets that are used with it. Or you may want to link a software asset to the hardware asset it is installed on.

![Asset linked assets section](/_books/servicemanager-user-guide/asset-management/images/asset-record-assets.png)

## Requests

View any requests that this asset is linked to. Linking assets to requests can be done to provide more context to the request, and to allow for better reporting on the assets that are most commonly linked to requests. For example, if a particular model of laptop is frequently linked to incident records, this may indicate a common issue with that model that needs to be addressed.

![Asset linked requests section](/_books/servicemanager-user-guide/asset-management/images/asset-record-requests.png)

## Attachments

Upload files and documents from your local file system. Attachments can be added to the asset record to provide additional context and information about the asset. For example, you may want to attach a copy of the purchase receipt, or a document containing the asset's specifications.

![Asset attachments section](/_books/servicemanager-user-guide/asset-management/images/asset-record-attachments.png)

## Asset history

View all changes to the asset's attributes by selecting the **History** icon.

The asset's audit history lists all actions, and who performed the action.

* **Search**: Search on **Field**, **From**, and **To** columns.
* **Relationships.** Show changes in relationships between this asset and other entities within Hornbill.
* **Generate PDF.** Create a PDF document of the audit history. This automatically downloads to your local computer. The document is split into sections for details and relationships.
* **Print.** Print the contents of the audit history to a printer.

![Asset history](/_books/servicemanager-user-guide/asset-management/images/asset-record-history.png)

## Asset Depreciation Calculator

With specific fields enabled and populated, an Asset Depreciation Calculator is shown in the right-hand panel of the asset view.

![Asset depreciation calculator](/_books/servicemanager-user-guide/asset-management/images/asset-depreciation-calculator.png)

The required fields to enable the calculator are:

* **Cost**: The original cost of the asset when it was purchased. This is a crucial input for calculating depreciation, as it serves as the starting point for determining the asset's value over time.
* **Depreciation Method**: The method used to calculate the asset's depreciation over time. Methods include straight-line and reducing balance. The choice of method will determine if the depreciation value is calculated as a fixed amount or as a percentage of the asset's remaining value.
* **Depreciation Value (percentage or amount)**: The amount by which the asset's value decreases over time. If the depreciation method is straight-line, this will be a fixed amount. If the method is reducing balance, this will be a percentage of the asset's remaining value.
* **Depreciation Frequency (months)**: The interval at which depreciation is calculated.
* **Depreciation Start Date**: The date when the asset's depreciation calculations begin.
* **Depreciation Term (months)**: The total duration over which the asset will be depreciated.

Modifying any of the required fields will automatically update the depreciation schedule in the calculator. The calculator will display the current value of the asset based on the depreciation calculations, as well as a schedule showing how the asset's value will change over time.

![Asset depreciation fields](/_books/servicemanager-user-guide/images/asset-depreciation-fields.png)

The location of these fields on the asset record will vary, depending on how the asset type is configured by the asset administrator.

This video explains how to set up and use the calculator:

<iframe width="560" height="315" src="https://www.youtube.com/embed/V-_Bp19m4Ek?si=jz_OoFr53byrUQYh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Used by vs Shared with

An option is available to toggle between the asset being used by a single user or shared among multiple users.

![Used by vs Shared with toggle](/_books/servicemanager-user-guide/asset-management/images/asset-record-used-by.png)

### Used by

When the asset is set to **Used By** the used by field indicates the primary user of the asset. This is typically used for assets that are assigned to a specific individual, such as a laptop or mobile phone.

### Shared with

When the asset is set to **Shared with**, the asset can be shared between multiple users. This is typically used for assets that are not assigned to a specific individual, such as a conference room or a shared printer.

## Tags

Tags provide a way to specify keywords or attributes on an asset for easy searching.

* **Adding a Tag**: To add a tag, start typing the tag that you wish to add. As you type, existing tags that match will be displayed and can be selected. There are two modes available that control if a user can add their own tags or if the predefined tags must be used.
* **Conditions**: Within both the Advanced Filter and the View Criteria on the asset list, you can add a condition to filter your asset list based on one or more tags.
* **Global Search**: The Global Search contains two search options. Search by Name and Description (default) or by Tags.

## Custom buttons

Customizable actions for an asset can be added through what is known as custom buttons.  The availability of custom buttons may vary on each asset.

Asset administrators can add [custom buttons](/esp-config/customize/custom-buttons) to asset records that open a URL, display a popup, or run an [Auto Task](/servicemanager-config/customize/service-manager-auto-tasks) workflow.

![Custom buttons on an asset record](/_books/servicemanager-user-guide/asset-management/images/asset-record-custom-buttons.png)

Example uses for asset custom buttons may include:

* Launching a third-party online remote control application.
* Viewing further asset information held in a third-party discovery tool.
* Link to the vendor's website for more information on the asset.
* Running an Auto Task workflow to perform a specific action on the asset.

Custom buttons can be set to only show if certain conditions are met, for example if the asset has a certain status or if a particular user is viewing the asset record.
