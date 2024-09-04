# Asset Structure

![Asset Structure](_books/servicemanager-user-guide/asset-management/images/asset-structure.png)

## Asset Classes
At the top of the hierarchy are the pre-defined asset classes: Computer, Computer Peripheral, General, Mobile Device, Network Device, Printer, Software, Telecoms. The Asset Classes are predefined and cannot be modified.

The Asset Class is an important consideration when creating a new Asset Type, as the Class chosen dictates which attributes are available to populate when adding your individual Assets beneath an Asset Type.

Each Asset Class has a set of available attributes that can be hidden or made available to each different Asset Type that is created. This ensures only the relevant information is visible on the Asset forms for the different Asset Types.

> If Customers identify additional Asset Classes, or Class specific Attributes that they require, please inform Hornbill and we will review and if accepted look to include in future updates.

## Asset Types
Default Asset Types are provided for each Asset Class for customers to use.

Customers can create any additional Asset Type to sit within an Asset Class. The Asset Type can be created and can be configured to use all, or only the relevant Asset Class Attributes required for the specific Asset Type. When defining the Asset Type, you can also specify which of the Asset Type attributes are mandatory and must be populated when creating an asset of this Type. Asset Types are covered in more detail in the [Manage Asset Types](/servicemanager-user-guide/asset-management/manage-asset-types) documentation.

## Assets
Assets can be created against any available Asset Type. Details on adding, editing, or deleting Assets is covered in the [Manage Asset Types](/servicemanager-user-guide/asset-management/manage-asset-types) documentation.

## Asset Attributes
There are attributes common to all asset records, which are available to all asset Classes. However each asset class also has its own additional attributes that are unique to the class.

:::tip
The list of attributes below has primarily been made available to assist in the import of asset data. The Hornbill database can be explored in more detail using the [Application Entity Viewer](/servicemanager-config/advanced-tools-and-settings/entity-explorer).
:::

### Attributes Common to All Assets

| **Name**         | **Type** | **Required?** | **Description**                                                                            |
|------------------|----------|---------------|--------------------------------------------------------------------------------------------|
| acqMethod        | integer  | required      | The acquisition method of the asset (0 = none, 1 = purchased, 2 = leased, 3 = loaned, 4 = rented).   |
| actualRetireDate | dateTime | optional      | The actual date the asset was retired from service.                                        |
| assetTag         | string   | optional      | The tag number of the asset.                                                               |
| beneficiary      | string   | optional      | The beneficiary for the asset.                                                             |
| building         | string   | optional      | The building the asset is located in.                                                      |
| cost             | decimal  | optional      | The financial cost of the asset.                                                           |
| costCenter       | string   | optional      | The cost center of the asset.                                                              |
| country          | string   | optional      | The country the asset is located in.                                                       |
| deprecMethod     | integer  | optional      | The depreciation method of the asset (0 = none, 1 = straight line, 2 = reducing balance).  |
| deprecStart      | dateTime | optional      | The date that depreciation calculations started on the asset.                              |
| deprecValue      | decimal  | optional      | The amount to depreciate per period for the asset. Depends on the depreciation mode.       |
| description      | string   | optional      | A description of the asset.                                                                |
| disposalPrice    | decimal  | optional      | The disposal price of the asset.                                                           |
| disposalReason   | string   | optional      | The disposal reason for the asset.                                                         |
| floor            | string   | optional      | The floor the asset is located on.                                                         |
| geoLocation      | string   | optional      | The geo location of the asset.                                                             |
| invoiceNumber    | string   | optional      | The invoice number that the asset was purchased on.                                        |
| lastUpdatedBy    | string   | required      | The name of the user who last updated the asset. For CSV upload, specify “admin”.            |
| location         | string   | optional      | The location of the asset.                                                                 |
| maintenanceCost     | decimal     | optional     | The maintenance cost of the asset.                                                            |
| maintenanceRef      | string      | optional     | The maintenance reference for the asset.                                                      |
| name                | string      | required     | The name of the asset.                                                                        |
| notes               | string      | optional     | A free-text notes field (maximum 255 characters).                                                |
| operationalState    | integer     | optional     | The operational state of the asset (0 = operational, 1 = pre-production, 2 = retired).              |
| orderDate           | dateTime    | optional     | The order date of the asset.                                                                  |
| orderNumber         | string      | optional     | The order number of the asset.                                                                |
| ownedById           | string      | optional     | The user ID of the user who owns the asset.                                                    |
| ownedByName         | string      | optional     | The name of the owner of the asset.                                                           |
| ownedByType         | string      | optional     | The owner type of the asset (0 = coworker, 1 = contact).                                       |
| productId           | string      | optional     | The product ID of the asset.                                                                   |
| receivedDate        | dateTime    | optional     | The received date of the asset.                                                               |
| residualValue       | decimal     | optional     | The residual value of the asset.                                                              |
| room                | string      | optional     | The room the asset is located in.                                                             |
| scheduledRetireDate | dateTime    | optional     | The scheduled retirement date for the asset.                                                  |
| site                | string      | optional     | The site the asset is located on.                                                             |
| sourceImage         | string      | optional     | An image of the asset.                                                                        |
| state               | integer     | required     | The state of the asset (0 = current, 1 = active, 2 = archived).                                     |
| supplierId          | string      | optional     | The supplier ID of the asset.                                                                  |
| type                | string      | required     | The type of the asset.                                                          |
| usedById        | string     | optional     | The user ID of the user who uses the asset.                                      |
| usedByName      | string     | optional     | The name of the user of the asset.                                              |
| usedByType      | string     | optional     | The user type of the asset (0 = coworker, 1 = contact).                          |
| version         | string     | required     | The revision number of the asset record. Specify 0 for the initial CSV upload.  |
| warrantyExpires | dateTime   | optional     | The date that the warranty expires for the asset.                               |
| warrantyStart   | dateTime   | optional     | The date that the warranty started for the asset.                               |
| Company         | String     | Optional     | The Company the asset belongs to.                                                |
| Rack            | String     | Optional     | The Rack the asset is located on.                                                |
| U Position      | String     | Optional     | The Position on the rack of the asset.                                           |
| U Height        | String     | Optional     | The height of the asset on the rack.                                             |

### Computer Class

| **Name**           | **Field Type** | **Required?** | **Description**                                                            |
|--------------------|----------------|---------------|-----------------------------------------------------------------------------|
| biosManufacturer   | string         | optional      | Manufacturer of the computer BIOS.                                           |
| biosName           | string         | optional      | Computer BIOS name.                                                          |
| biosReleaseDate    | dateTime       | optional      | Computer BIOS release date.                                                  |
| biosSerialNumber   | string         | optional      | Computer BIOS serial number.                                                 |
| biosVersion        | string         | optional      | Computer BIOS version.                                                       |
| cpuClockSpeed      | string         | optional      | Computer CPU clock speed.                                                    |
| cpuInfo            | string         | optional      | CPU information about the asset.                                            |
| disasterRecovery   | string         | optional      | There is a disaster recovery system for the asset (Yes, No).                 |
| dscCfFingerprint   | string         | optional      | The MD5 fingerprint of the overall asset configuration.                     |
| dscFirstDiscovered | dateTime       | optional      | The date/time the asset was first discovered.                               |
| dscHwFingerprint   | string         | optional      | The MD5 fingerprint of the hardware configuration for the asset.            |
| dscLastChanged     | dateTime       | optional      | The date/time the asset configuration was last detected.                    |
| dscLastDiscovered  | dateTime       | optional      | The date/time the asset was last discovered.                                |
| dscNetFingerprint  | string         | optional      | The MD5 fingerprint of the network configuration for the asset.             |
| dscOsFingerprint   | string         | optional      | The MD5 fingerprint of the operating system configuration for the asset.    |
| dscSiid            | integer        | optional      | The ID of the Site Integration Server that last discovered the asset.       |
| dscSource          | integer        | optional      | The ID of the discovery profile used to discover the asset.                 |
| dscSwFingerprint   | string         | optional      | The MD5 fingerprint of the installed software configuration for the asset.  |
| environment        | string         | optional      | The asset environment (Live, Test, Development, Production).                 |
| lastLoggedOn       | dateTime | optional | The date/time the asset was used by someone to log on to the network.  |
| lastLoggedOnUser   | string   | optional | The user who last logged onto the asset.                               |
| lastPatchDate      | dateTime | optional | The last patch date.                                                    |
| logicalCpus        | integer  | optional | Number of Logical CPUs for the computer.                                |
| macAddress         | string   | optional | Computer MAC address.                                                   |
| manufacturer       | string   | optional | The company that makes the asset.                                      |
| maxMemoryCapacity  | string   | optional | Maximum memory capacity for the computer.                               |
| memoryInfo         | string   | optional | Information about the memory in the asset.                             |
| model              | string   | optional | The model number/name of the asset.                                    |
| monitoring         | string   | optional | There is a monitoring system for the asset (Yes, No.                   |
| monitoringSoftware | string   | optional | The asset monitoring software.                                          |
| netComputerName    | string   | optional | The name/hostname of the asset.                                        |
| netIpAddress       | string   | optional | The IP address(es) of the asset.                                       |
| netName            | string   | optional | The network name the asset is part of.                                  |
| netWinDomRole      | string   | optional | The role within the windows domain the asset plays.                    |
| netWinDomain       | string   | optional | The windows domain this asset is part of.                              |
| nextPatchDate      | dateTime | optional | The next patch date.                                                    |
| numberMemorySlots  | integer  | optional | Number of memory slots on the computer                                 |
| opticalDrive       | string   | optional | The Optical Drive for this computer.                                    |
| osDescription      | string   | optional | Text description of the operating system running on the asset.         |
| osRegisteredTo   | string  | optional | The name of the organization/user the os of the asset reports being registered to.  |
| osSerialNumber   | string  | optional | The serial number of the operating system running on the asset.                     |
| osServicePack    | string  | optional | The service pack of the operating system running on the asset.                      |
| osType           | string  | optional | The type of the operating system, WINNT, Linux, OSX etc for the asset.              |
| osVersion        | string  | optional | The version of the operating system running on the asset.                           |
| physicalCores    | integer | optional | The number of physical cores in this asset                                          |
| physicalCpus     | integer | optional | The number of physical CPUs in this asset                                           |
| physicalDiskSize | string  | optional | The amount of physical disk size in this asset                                      |
| privateIpAddress | string  | optional | The asset private IP address.                                                        |
| publicIpAddress  | string  | optional | The asset public IP address.                                                         |
| serialNumber     | string  | optional | The serial number/tagID number of the asset.                                        |
| subnetMask       | string  | optional | The subnet mask of the asset.                                                       |
| wmacAddress      | string  | optional | The wMAC address for the asset.                                                      |

### Computer Peripheral Class

| **Name**        | **Field Type** | **Required?** | **Description**                                         |
|-----------------|----------------|---------------|----------------------------------------------------------|
| connectionTypes | string         | optional      | The connection types for the asset (USB, HDMI, etc.).     |
| wireless        | string         | optional      | Is the asset capable of a wireless connection (Yes/No).  |
| Manufacturer    | String         | Optional      | Manufacturer for the asset                               |
| Model           | string         | Optional      | Model of asset.                                           |
| Serial Number   | String         | Optional      | Serial number of asset.                                   |

### Network Device Class

| **Name**         | **Field Type** | **Required?** | **Description**                   |
|------------------|----------------|---------------|-----------------------------------|
| macAddress       | string         | optional      | The MAC address for the asset.    |
| manufacturer     | string         | optional      | Name of the manufacturer.          |
| netIpAddress     | string         | optional      | The MAC address for the asset.    |
| physicalDiskSize | string         | optional      | Size of the Hard Disk Drive       |
| serialNumber     | string         | optional      | The serial number for the asset.  |

### Mobile Device Class

| **Name**           | **Field Type** | **Required?** | **Description**                            |
|--------------------|----------------|---------------|--------------------------------------------|
| capacity           | string         | optional      | The storage capacity of the asset.         |
| cpuInfo            | string         | optional      | General CPU information.                    |
| imeiNumber         | string         | optional      | The IMEI number for the asset.             |
| ipAddress          | string         | optional      | The IP address for the asset.              |
| macAddress         | string         | optional      | The MAC address for the asset.             |
| manufacturer       | string         | optional      | The manufacturer of the asset.             |
| model              | string         | optional      | The model of the asset.                    |
| osVersion          | string         | optional      | The version of the installed operating system.  |
| phoneNumber        | string         | optional      | The phone number for the asset.            |
| serialNumber       | string         | optional      | The serial number for the asset.           |
| simNumber          | string         | optional      | The SIM card number for the asset.         |
| simType            | string         | optional      | The SIM card type for the asset.           |
| IMSI Number        | Sring          | Optional      | The IMSI number for the asset.           |
| MTPAS Access Class | String         | Optional      | The MTPAS access class for the asset.               |
| SIM Type           | String         | Optional      | The SIM type for the asset.                         |

### Printer Class

| **Name**              | **Field Type** | **Required?** | **Description**                                                            |
|-----------------------|----------------|---------------|-----------------------------------------------------------------------------|
| averagePagesPerMinute | string         | optional      | The average pages per minute the asset can output.                          |
| dscCfFingerprint      | string         | optional      | The MD5 fingerprint of the overall asset configuration.                     |
| dscFirstDiscovered    | dateTime       | optional      | The date/time the asset was first discovered.                               |
| dscHwFingerprint      | string         | optional      | The MD5 fingerprint of the hardware configuration for the asset.            |
| dscLastChanged        | dateTime       | optional      | The date/time the asset configuration was last detected.                    |
| dscLastDiscovered     | dateTime       | optional      | The date/time the asset was last discovered.                                |
| dscNetFingerprint     | string         | optional      | The MD5 fingerprint of the network configuration for the asset.             |
| dscSiid               | integer        | optional      | The ID of the Site Integration Server that last discovered the asset.       |
| dscSource             | integer        | optional      | The ID of the discovery profile used to discover the asset.                 |
| dscSwFingerprint      | string         | optional      | The MD5 fingerprint of the installed software configuration for the asset.  |
| horizontalResolution  | string         | optional      | The horizontal resolution output of the asset.                              |
| languages             | string         | optional      | The operating languages of the asset.                                       |
| manufacturer          | string         | optional      | The company that makes the asset.                                           |
| markingTechnology     | string         | optional      | The marking technology of the asset, e.g. Laser, Inkjet.                    |
| model                 | string         | optional      | The model number/name of the asset.                                         |
| netIpAddress          | string         | optional      | The IP address of the asset.                                                 |
| netMacAddress         | string         | optional      | The MAC address of the asset.                                                |
| numberOfTrays         | integer        | optional      | The number of input trays the asset has.                                    |
| paperSizes            | string         | optional      | The paper sizes the asset can output.                                       |
| port                   | string | optional | The port number the asset resides on.         |
| printerCapabilities    | string | optional | Any additional capabilities of the asset.     |
| serialNumber           | string | optional | The serial number/tagID number of the asset.  |
| verticalResolution     | string | optional | The vertical resolution output of the asset.  |
| IP Address             | String | Optional | IP Address for printer.                        |
| MAC Address            | String | Optional | The MAC address for the printer.                   |
| wMAC Address           | String | Optional | The wMAC address for the printer.                  |
| Black Toner Code       | String | Optional | Code for the black toner of the printer.       |
| Quantity Black Toner   | String | Optional | Quantity of the black toner.                   |
| Black Toner Level      | String | Optional | Toner level.                                   |
| Cyan Toner Code        | String | Optional | Code for the black Cyan toner of the printer.        |
| Quantity Cyan Toner    | String | Optional | Quantity of the Cyan toner.                    |
| Cyan Toner Level       | String | Optional | Toner level.                                   |
| Magenta Toner Code     | String | Optional | Code for the magenta toner of the printer.     |
| Quantity Magenta Toner | String | Optional | Quantity of the magenta toner.                 |
| Magenta Toner Level    | String | Optional | Toner level.                                   |
| Yellow Toner Code      | String | Optional | Code for the Yellow toner of the printer.      |
| Quantity Yellow Toner  | String | Optional | Quantity of the yellow toner.                  |
| Yellow Toner Level     | String | Optional | Toner level.                                   |
| Image Fuser            | Sting  | Optional | Image Fuser for printer                       |
| Image Transfer Roller  | String | Optional | Image Transfer Roller for the printer.         |

### Software Class

| **Name**               | **Field Type** | **Required?** | **Description**                                                                                                                                                                              |
|------------------------|----------------|---------------|------------------------------------------------------------
| licenseCost            | decimal        | optional      | The cost of the license                                                                                                                                                                       |
| licenseExpiryDate      | dateTime       | optional      | The date the license expires.                                                                                                                                                                  |
| licenseKey             | string         | optional      | The asset license key.                                                                                                                                                                         |
| licenseRenewalDate     | dateTime       | optional      | The date the license has been renewed.                                                                                                                                                         |
| licenseStartDate       | dateTime       | optional      | The date the license starts.                                                                                                                                                                   |
| licenseType            | string         | optional      | The type of license (Single User License, Named User License, Concurrent License, Per Device License, Optimizational based License, Transactional based License, Subscription based License).  |
| registeredEmailAddress | string         | optional      | The registered email address.                                                                                                                                                                  |
| registeredName         | string         | optional      | The registered name.                                                                                                                                                                           |
| swDscFingerprint       | string         | optional      | The MD5 fingerprint of the overall asset configuration.                                                                                                                                       |
| swDscFirstDiscovered   | dateTime       | optional      | The date/time the asset was first discovered.                                                                                                                                                 |
| swDscLastChanged       | dateTime       | optional      | The date/time the asset configuration was last detected.                                                                                                                                      |
| swDscLastDiscovered    | dateTime       | optional      | The date/time the asset was last discovered.                                                                                                                                                  |
| swDscSiid              | integer        | optional      | The ID of the Site Integration Server that last discovered the asset.                                                                                                                         |
| swDscSource            | integer        | optional      | The ID of the discovery profile used to discover the asset.                                                                                                                                   |
| swProductId            | string         | optional      | The software product ID for the asset.      |
| swProductName          | string         | optional      | The software product name for the asset.    |
| swVendorId             | string         | optional      | The vendor ID of the asset.                 |
| swVendorName           | string         | optional      | The vendor name of the asset.               |
| swVersion              | string         | optional      | The software version of the asset.           |

### Telecoms Class

| **Name**      | **Field Type** | **Required?** | **Description**                |
|---------------|----------------|---------------|---------------------------------|
| ipAddress     | string         | optional      | The IP address for the asset.   |
| macAddress    | string         | optional      | The MAC address for the asset.  |
| manufacturer  | string         | optional      | Name of the manufacturer.        |
| Phone Number  | string         | Optional      | Phone number for Telecom asset.  |
| Extension     | String         | Optional      | Phone number extension.          |
| Serial Number | String         | Optional      | Serial number for the asset.     |
| Model         | String         | Optional      | Identifier for the asset.        |
| wMac Address  | String         | Optional      | The wMAC address for the asset.  |


<!-- https://wiki.hornbill.com/index.php?title=Understanding_the_Asset_Structure -->