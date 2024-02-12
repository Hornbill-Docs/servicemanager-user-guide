---
layout: article-toc
---
# Services
The goal of a service is to deliver value to customers and employees through a variety of mechanisms.

## Planning
The starting point to building a service catalog is to identify the services that are being offered. This could vary from a single service that offers IT help to users through self serve, chat, and request management to a service catalog offering many servcies across different areas of the business.

## Details
The details of a service provides some key values and settings to make a service operational. These options include setting the name, description, status, visibility, and more. Some of this information is mandatory on the creation of a Service so it is important to plan your service before starting.
### Name
The name of your Service is a simple yet very important aspect of a service. The Service Name is mandatory for the creation of a service. When naming your service, some things to consider are:
* The name is visible to subscribed customers on the Self Service Portals
* The name is visible to support staff within Intelligent Capture when using the Services Capture form
* The name is visible within the Services column of the Request List
* The name is visible on each request that has been raised for that service
* Consider the length of the name and how it may be displayed in these different areas.
* A unique service name is not enforced so it is possible for two distinct areas of a business to have a service by the same name.
* If you need to support more than one language for users of the Service, be sure to create different language versions of your Service Name and Description. Users of the Service will see the appropriate one based on the language assigned to their profile (if you provide the translation).

### Description
A brief description of your service can be added to your Service. This allows you to add some additional information to describe the purpose or use of the service. This description is available for customers to read on the Self Service Portals when viewing their service information. It is also available to support staff on the Services Progressive Capture form when raising a request to provide that bit of extra information to make sure they are selecting the correct service.

### Category
Used to group your Services. Select one from the pre-defined list

### Portfolio Status
The Service Portfolio Status uses some industry standard conventions for determining the state of the service. These statuses include Pipeline, Catalog, and Retired.

* **Pipeline**<br>This status is generally used as a planning state. While the status is Pipeline, the service will remain hidden from customers and support staff to allow for planning and setup of the service.
* **Catalog**<br>Once all of the required configuration and setup is complete a service status can be set to Catalog. Once in the status of Catalog, the service will be live and available for selection by support staff when raising a request on the Services form in Progressive Capture, or for subscribers of the Service raising requests via the Self Service Portals.
* **Retired**<br>When a service is no longer required the status can be changed to Retired. This will remove the service from support staff and subscribers of the service.

### Employee Portal
These options are used with the Employee Portal. These options will be needed for publishing your services to the Employee Portal.

* **Service Domain**<br>Associated this service to a Service Domain. Domains are used for grouping related services that fall under areas such as IT, HR, and Facilities.
* **Service Domain Category**<br>Select a category for this service. Service Domain Categories provide a category option for all applications that publish services to this Domain.

### Default Mailbox
Define which mailbox any manually sent emails will be sent from on requests logged against the service
* If no mailbox is selected then manually send emails will be sent from the mailbox selected by the agent sending the email on the request raised against the service
* Agents need to have the rights to send emails from the default service, otherwise it will default to a mailbox the agent does have the rights to send from
* Agents can manually override which mailbox emails are sent from when sending emails manually from a request logged against the service if they have the rights to more than one mailbox

### Portal Visibility
If the Service will be visible on the Employee, Customer and Service Portals for subscribed users.
* **Visible**<br>Subscribed users will see, and have access to their requests raised against the Service, even if they you have restricted their ability to raise tickets from the portals for this Service.
* **Hidden**<br>Subscribed users will not see the Service on the Customer or Service portal - Useful when defining a technical Service rather than a business Service.

### Service Icon
The Icon which will be used to represent the service on the Service and Customer Portals for the subscribers to this service

### Owner
Each Service allows for an individual owner to be assigned. Being allocated as an owner offers some additional controls to how other Services Managers interact with the service.

* When a service has no owner, any user with the Services Manager role can set an owner
* Only the owner can change the owner to another user once the owner has been set
* Only the owner can change the Access option between Private and Open
* When selecting an owner, only users that have the Services Manager role will be available

### Access
The Access option allows an owner of a service to control who can see and update information for the selected service by using the options of Open or Private.

* **Open**<br>All users with the role of Services Manager can update and manage the details and other options within a service excluding the removing or changing an existing Service Owner and setting the Access. The Service will be visible in the Services List to all users with the Services Manager role. Members of a team that supports the service will be able to add and update FAQs, Bulletins, and the Operational Status.
* **Private**<br>This restricts the visibility in the Services List to just the owner and the members of the teams that support the service who have the Services Manager role. Only the owner will have the right to modify the service details and configuration. Members of a team that supports the service will be able to add and update FAQs, Bulletins, and the Operational Status. Only the owner can add or remove Supporting Teams and only the owner can add or remove subscriptions

### Activities
The Activities panel lets you create and managed tasks and activities against this service. This can be used for planning updates to any aspect of the service such as updating a BPM workflow or Progressive Capture.

## Request Configuration
Each Service allow you to configure the different the types of requests which will be available. These included Incidents, Service Requests, Problems, Known Errors, and Changes. Each request type can be configured to meet the particular needs for the service, including BPM workflow, available actions, custom fields, and Request Catalog Itesm.
Requests
Any Requests which the Service has been raised directly against, or where it has an associated relationship to Requests will be displayed here.

## Assets
Associating the assets which support a service helps support quicker Incident and or Problem resolutions by making it quick and easy to understand what infrastructure is directly used to provide each service. Change management can benefit from visualizing impact when considering implementing changes to a service, or assets which support a service.

## Services
Associating technical services which support/underpin business services helps support quicker Incident and or Problem resolutions by making it quick and easy to understand how services are related. Change management can benefit from visualizing impact when considering implementing changes to a technical or business service.

## FAQs
Define Frequently Asked Questions (FAQs) which will be helpful to subscribers of the service on both the Customer and Service Portals.

## Bulletins
Define Service specific announcements or news which will be shared with the subscribers of the Service on both the Customer and Service Portals

## Documents
Documents that are held within Document Manager can be associated to a Service. This is designed to provide document access to the subscribers of the service through the Customer and Employee Portals.

:::note
It is important to ensure that the documents linked to the service are held within a library that has been configured for access on the portals. Linking a document that is held in a library that is not configured for portal access will result in the document being listed, but not accessible by the service subscriber.
:::

### Sharing a Library with the Portals
The option for sharing libraries is managed from within the Document Manager app.

1. From the main Hornbill Tile Menu, select Document Manager -> Libraries.
1. From the list of libraries, find the library that you would like to make available to the portals and select Properties.
1. On the Share option start by selecting Role and then search for the Docmanager Portal.
1. Select Can View Library Contents and then click Share.
1. Repeat for each library that you would like make accessible on the portals

### Library Visibility Options

On the Library properties, visibility can be controlled so that a library is only visible to customers when viewing the Service details. By default, a library is visible within the Portals' Library List. In order remove the library from the library list and only have it show associated documents on the Service form, the two following options in Document Manager Libraries need to be un-checked.

* **Show in User Library List**<br>Untick to hide the library in the employee portal and collaboration, this will only take effect if the user has been shared the library with read-only access (users with modify permissions will still be able to see this library). You will still be able to share documents in this library with users with read only permissions by giving them a direct link to the document
* **Show in Customer Portal Library List**<br>Untick to hide the library in the customer portal, (the library must be shared with a guest role before it can be accessed in the customer portal). You will still be able to share documents in this library with customers even if this setting is unticked by giving them a direct link to the document.

### Adding a Document to a Service
On each Service form within the Service Portfolio, a Documents option lets you browse the list of all documents that belong to a particular library and link or unlink documents to the service. This action only be performed by the Service's owner.

* **Select Library**<br>Select from the list of available libraries that you want to browse
* **Order By**<br>To help locate a document, you can change the order of the list by
    * Title
    * Owner
    * File Type
    * Creation Date
    * Updated Date

Each document will have a Link option. When clicked, this will associate the document with the service. Documents already linked to a service ill have an option to Un-link. When clicked, this will remove the document from the service.

## SLAs
Service Level Agreements can be linked to each service, and rules defined to manage which SLA and Service Level's will be invoked when requests are raised against each service.
It is possible to associate one or more Corporate Service Level Agreements to each Service, and or create Service Level Agreements which are specific to each service.
Use the Manage Rules options to determine which Service Level agreement is invoked under different conditions when raising requests against a Service.

## Supporting Teams
The Supporting Teams feature is used to assign the Service Desk teams who will be supporting this service. Supporting teams will have the rights to view and manage requests for this service.

## Subscribers
It is possible to subscribe customers to a service based on various organization groups. The default position for a service is that all customers will be entitled to use the Service.

## Service Status
It is possible to set the status of each service, and an accompanying message so that subscribers to the service and those supporting the service can see the status and any supporting message.

* Available
* Impacted
* Unavailable

As the Status changes from one state to another, information is collected to provide availability metrics. This includes mean time between failures, average time to recovery, and percentage break down of the different statuses over a selected time period. The availability metrics can be accessed using the chart icon next to the service status. At least one change in the status is required in order to view the metrics.

## Timeline
Each service provides an area where users who have access to the service can have a discussion about the service. This is a great way to plan or make suggestions for the service.