# Configuration Items
Configuration Management holds data relating to a collection of IT entities called configuration items (CIs); it also holds descriptive relationships between these entities.

A Configuration Item may be:

* A physical asset (e.g. a server, switch, etc.), a user, a request, or an attachment
* A logical asset (e.g. an instance of a database)
* A conceptual asset (e.g. a service)

Regardless of the CI type, it is important to understand and manage the CI's attributes and understand the relationships and dependencies between them. For example, if a database instance gets corrupted, this may affect the ERP service and prevent orders from being processed, which in turn directly affects the efficiency and productiveness of a business's employees.

## Features
Configuration Management allows you to view relationships between CIs via its graphical Configuration Item Explorer. Configuration Items that can be viewed, and the relationships between them, include:

* Assets
* Services
* Requests
* Users
* Attachments

You can launch the Explorer from the following Configuration Item views:

* Configuration Manager List
* Asset records
* Service records
* Request records

## In-Policy Configuration Items
Certain CI types can be marked as In Policy. This allows you to manage the CIs that are most important to you, and in some cases it can enhance and enable additional functionality against the original entity.

Why mark CIs as In Policy? You may wish to manage your servers and understand which services are dependent on them. Or, you may want to schedule routine maintenance against business-critical infrastructure, and as such enable activities to manage this work.

On the other hand, you may have several thousand computer peripherals (e.g. mice) that are worth little and hold no business value in terms dependencies or relationships to other CIs. You may want to mark this kind of CI as Not in Policy.

### Assets
You can already records your assets if you have Service Manager installed on your instance. This includes the following functionality:
* Defining each asset's class and type.
* Defining the attributes that you wish to record for the assets.
* Automatically tracking and auditing all changes to the asset's attributes through the History feature.
* Viewing all requests raised against the asset.
* Linking assets to other assets and services.

Marking individual assets as In Policy enables the following functionality on the assets:

* Using the Configuration Item Explorer to define the bi-directional dependencies and impact of the links between the asset and other assets and services it is linked to.
* Enabling activities on the asset record, allowing you to schedule and manage activities relating to the asset, such as routine maintenance or reviews.
* Enabling an activity stream on the asset record, allowing for collaboration and discussion on the asset with other users.
* Posting and commenting on the asset.
* Following the asset to get updates to its Activity Stream posted to your News Feed, so as to keep informed about all discussions around business-critical assets.

### Services
You can already record your services if you have Service Manager installed on your instance. This includes the following functionality:

* Creating services and managing their catalog status.
* Creating links to assets.

Marking individual services as being In Policy enables the following functionality on the services:
* Using the Configuration Item Explorer to define the bi-directional dependencies and impact of the links between the service and assets it is linked to.

## Configuration Item Explorer
* **Request record**<br>Launch the CI Explorer directly from any request form. This puts the request as the focus of the Explorer and allows you to visualize the related CIs associated to this request.
* **Asset record**<br>Launch the CI Explorer directly from any asset form. This puts the asset as the focus of the Explorer and allows you to visualize the related CIs to this asset.
* **Services record**<br>Launch the CI Explorer directly from any service form. This puts the service as the focus of the Explorer and allows you to visualize the related CIs to this service.