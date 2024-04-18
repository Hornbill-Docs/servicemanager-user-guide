# Configuration Items
Configuration Manager is a repository / data warehouse for information technology (IT) installations (CMDB). It holds data relating to a collection of IT entities (commonly referred to as configuration items (CI)), as well as descriptive relationships between such entities.

A Configuration Item may be:

* A physical entity, such as an Asset (Server, Switch etc), a User, Request or Document
* A logical entity such as an Asset (instance of a database)
* Conceptual, such as a Service

Regardless of the Configuration Item type it is important to understand and manage their attributes and understand the relationships and dependancies between them. For Example if a database instance get's corrupted, this may affect the ERP service and prevent orders from being processed and directly affect the efficiency and productiveness of a businesses employees.

## Features
Configuration Manager allows you to view relationships between Configuration Items via it's graphical Configuration Item Explorer. Configuration Items which can be viewed, and the relationships between them include:

* Assets
* Services
* Requests
* Users
* Documents

You can launch the Explorer from the following Configuration Item views:

* Configuration Manager List
* Asset records
* Service records
* Request records

## In Policy Configuration Items
Certain Configuration Item types can be marked as In Policy, this provides you with the ability to Manage the Configuration Item's which are most important to you, and in some cases enhance and enable additional functionality against the original entity.

You may wish to manage your Server's and understand which Services are dependant on them, this would be an example of why you would want to put those Configuration Item's In Policy
You may want to schedule routine maintenance against business critical infrastructure, and as such enable Activities to manage this work, this would be a reason to put these Configuration Item's in Policy
You may have several thousand computer peripherals such as Mice which are low value and hold no business value in terms dependancies or relationships to other Configurations Items, these may add no value being In Policy

### Assets
You can already records your Assets if you have Service Manager installed on your instance. This includes the following functionality:
* Defining each Assets Class and Type
* Defining the attributes which you wish to record for the Assets
* Automatically track and audit all changes to the Asset's attributes through the History feature
* View all requests raised against the Asset
* Link Assets to other Assets and Services

Individual assets marked as being In Policy will enable the following functionality on such Assets

* The ability via the Configuration Manager Explorer to define the bi-directional dependancies and impact of the Links between the Asset and other Assets and Services it is linked to
* Enable Activities on the Asset record, allowing you to schedule and manage Activities relating to the Asset such as routine maintenance or reviews
* Enable an Activity Stream on the Asset record, allowing for the collaboration and discussion on the asset with other users.
* Post and Comment on the Asset
* Follow the Asset to get updates to its Activity Stream posted to your News Feed, allowing you to keep informed about all discussions around business critical assets

### Services
You can already records your Services if you have Service Manager installed on your instance. This includes the following functionality:

* Creating Services and managing their Catalog Status
* Create Links to Assets

Marking individual Services as being In Policy will enable the following functionality on such Services
* The ability via the Configuration Manager Explorer to define the bi-directional dependancies and impact of the Links between the Service and Assets it is linked to.

## CI Explorer
* **Request record**<br>Launch the CI Explorer directly from any request form. This will put the request as the focus of the explorer and allow you to visualize the related CIs associated to this request.
* **Asset record**<br>Launch the CI Explorer directly from any asset form. This will put the asset as the focus of the explorer and allow you to visualize the related CIs to this asset
* **Services record**<br>Launch the CI Explorer directly from any Service form. This will put the Service as the focus of the explorer and allow you to visualize the related CIs to this.