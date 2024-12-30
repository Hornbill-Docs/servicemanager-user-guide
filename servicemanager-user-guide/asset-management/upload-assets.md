---
layout: article-toc
---
# Upload Assets
Manually upload multiple assets for specific asset classes from CSV files. This option is provided to allow the insert of new assets into the Service Manager asset repository, this is generally used for static data. If you require the ability to schedule the importing of new or updates to existing assets from discovery tools or MSSQL or MySQL databases, you can find more information about the Asset Import utility in the [Data Imports Guide](/data-imports-guide/assets/overview).

As an Asset Management Administrator, select **Asset Upload** from the Asset Management icon in the application navigation bar.

## Creating the upload template
You can upload assets of different asset types, but only those that are managed under the same asset class from a single CSV template. If you need to upload assets for types that are managed under different asset classes, you must create different CSV templates for each asset class grouping.

**To create your upload template:**
1. From the dropdown control against which you wish to import the new assets, select the asset class. This enables the option to download the related asset class template.
1. Select to download the template file.
1. Populate the template file rows and columns with the attributes for each asset you want to upload. Name and Type are mandatory attributes for each asset you wish to upload, regardless of their type or class.
1. Click **Save**.

While other attributes are not mandatory to perform the import, it is good practice to populate the attribute fields to match those that you enabled for each asset type (when you were defining the asset types). Examples being *Used by* or *Site*, should you want the assets to appear as linked to these entities when performing other Service Manager actions, such as logging requests through Intelligent Capture and having the option to choose from a list of assets associated to the user.

*Used by* requires the *usedById*, *usedByName*, and *usedByType* attributes to be completed. *usedByType* should be populated with either:
* 0 - if *Used By* is a coworker
* 1 - if *Used By* is a contact

*Owned By* requires both the *ownedById*, *ownedByName* and *ownedByType* attributes to be completed. *ownedByType* should be populated with either:
* 0 - if *Owned By* is a coworker
* 1 - if *Owned By* is a contact

Site requires both the *site* and the *siteId* attributes to be completed. *SiteId* refers to the database numerical value not the display name.
Date attributes are required in the following format: yyyy-mm-dd hh:mm:ssZ
Country requires the ISO Alpha 2 codes as per the listing here - [1]
The fields in the CSV file are mapped on the assets database table. To find what values and types need to be populated in the fields, navigate to Home > Applications > Service Manager > Entity Viewer. Select "Database Schema Viewer" and navigate to the the "h_cmdb_assets" table.

## Validation
Against each asset class it is possible to configure which if any fields for that given asset class you wish to perform data validation before uploading the assets from the CSV file into the Service Manager asset repository.

As each customer maybe using different unique identifiers, it is possible for each customer to select from the available fields for each asset class, against which to perform the validation to ensure an asset does not already exist, and therefore avoid the creation of duplicate entries.
1. Select Validation
2. Select one, multiple or all of the available fields to perform the validation checks against and select save.
It is important to appreciate that the upload time for the asset import will be extended if validation is enabled and if multiple checks are required to be performed.

## Select CSV File to Upload
In order to initiate the asset upload, you will need to select the CSV file you wish to use. On selecting the file the import process will automatically begin.

On completion of the import a report will be produced which will summarize:

* Number of records processed
* The number of records successfully uploaded
* Records which failed to upload
If during the import process, specific rows of asset data are not able to be imported, this will be detailed below including:

Which rows failed
The reason for the failures

<!-- https://wiki.hornbill.com/index.php?title=Upload_Assets_CSV -->
