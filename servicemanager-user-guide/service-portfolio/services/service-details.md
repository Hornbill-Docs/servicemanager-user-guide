---
layout: article-toc
---
# Service Details
The details of a service provide key values and settings necessary to make the service operational. These options include setting the name, description, status, and more. Some of this information is mandatory when creating a service, so it is important to plan your service before starting.

![Service Details](/_books/servicemanager-user-guide/images/service-details-tab.png)

### Name
The name of your service is a simple yet crucial aspect of the service. The service name is mandatory for its creation. When naming your service, consider the following:
* The name is visible to subscribed customers on the Employee and Customer Portals.
* The name is visible to support staff within Intelligent Capture when using the Services Capture form.
* The name is visible within the Services column of the Request List.
* The name is visible on each request that has been raised for that service.
* Consider the length of the name and how it may be displayed in these different areas.
* A unique service name is not enforced so it is possible for two distinct areas of a business to have a service by the same name.
* If you need to support multiple languages for users of the service, ensure that you create different language versions of the service name and description. Users will see the provided translation version based on the language assigned to their profile.

### Description
You can add a brief description to your service, allowing you to provide additional information about its purpose or use. This description is available for customers to read on both the Employee and Customer Portals when they view their service information. It is also accessible to support staff on the Services Intelligent Capture form, providing extra information to ensure they select the correct service when raising a request.

### Type
The service types include the options *business* and *technical*. 
* **Business Services**. A business service has a focus on supporting business users.  These services help businesses run more efficiently, reduce costs, and improve productivity by providing specialized support to essential functions such as IT, accounting, marketing, HR, legal, cleaning, or logistics.
* **Technical Services**. A technical service is a specialized, often hands-on activity, providing technical knowledge, engineering expertise, or IT infrastructure support to enable business operations, maintenance, or systems functionality. These services include troubleshooting, repairing, installing, and managing technical systems to ensure operational continuity. Technical services are often put in place to underpin and support business services.

### Category
Used to group your services. Select one from the pre-defined list.

:::tip
The [list of categories](/servicemanager-config/setup/service-manager-simple-lists#service-manager-simple-lists) can be modified within the Service Manager configuration. The categories are stored in a [Simple List](/servicemanager-config/setup/service-manager-simple-lists) called `serviceCategories`.
:::

### Portfolio Status
The Service Portfolio Status employs several industry-standard conventions for determining the state of a service. These statuses include Pipeline, Catalog, and Retired.

* **Pipeline**<br>This status is typically used as a planning phase. While the status is set to "Pipeline", the service will remain hidden from customers and support staff to allow for its planning and setup.
* **Catalog**<br>Once all the required configurations and setup are complete, a service status can be set to "Catalog". Once the status is set to "Catalog," the service will be live and available for selection by support staff when raising a request on the Services form in Intelligent Capture. It will also be available to subscribers of the service who are raising requests via the Employee or Customer Portals.
* **Retired**<br>When a service is no longer needed, its status can be changed to "retired." This action will remove the service from the support staff and its subscribers.

### Employee Portal
These options are needed for publishing your services to the Employee Portal.

* **Service Domain**<br>Associated this service to a Service Domain. Domains are used for grouping related services that fall under areas such as IT, HR, and Facilities.
* **Service Domain Category**<br>Select a category for this service. Service Domain Categories provide a category option for all applications that publish services to this Domain.

### Default Mailbox
Define which mailbox any manually sent emails will be sent from on requests logged against the service.
* If no mailbox is selected then manually send emails will be sent from the mailbox selected by the agent sending the email on the request raised against the service.
* Agents need to have the rights to send emails from the default service, otherwise it will default to a mailbox the agent does have the rights to send from.
* Agents can manually override which mailbox emails are sent from when sending emails manually from a request logged against the service if they have the rights to more than one mailbox.

### Service Icon
The Icon which will be used to represent the service on the Service and Customer Portals for the subscribers to this service.