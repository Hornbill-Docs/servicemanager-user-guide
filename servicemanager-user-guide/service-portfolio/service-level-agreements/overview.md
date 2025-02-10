# Corporate Service Level Agreements
A Service Level Agreement (SLA) is a contract between a service provider and a customer that outlines the expected level of service the customer will receive.

Corporate service level agreements (SLAs) allow you to define a combination of service levels and service-level targets that can be used across multiple services sharing the same SLA requirements. By using corporate SLAs, you can centralize the management of all these SLAs into one place rather than on a service-by-service basis.

![Corporate Service Levels](/_books/servicemanager-user-guide/service-portfolio/images/corporate-sla.png)

## About corporate SLAs
* Corporate SLAs can be associated with one or more services.
* A service can be associated with both a corporate SLA and its own SLA.
* A service can have its own SLA without having a corporate SLA.

### When to use a corporate SLA
A corporate SLA can be a great way to have a standard agreement that spans across multiple services.  New services can use a corporate SLA as a starting point. As a service is reviewed and improved, unique service level requirements can be added as part of a service based SLA. 

## Before you begin
* A user must have the [Services Manager](/servicemanager-config/setup/service-manager-roles#services) 
role to access the Service Portfolio.
* Plan. It is important to have an understanding of what an agreement will cover. Which services will come under each SLA? What are the expectations of the customers that consume the service?  What time frames are reasonable for the service desk to be able to respond and resolve issues?
 
## Accessing corporate SLAs
**To access corporate SLAs:**
1. In the [App toolbar](/esp-user-guide/navigation#app-toolbar), click the Service Management icon.
1. Select **Service Portfolio**.
1. Select the **Service Level Agreements** tab.


## Details
The following SLA details are required when first creating a new SLA. These details are available within the SLA form.

* **Name.** The name of the SLA is used to find and link to services and is visible on the requests that it is associated to. An unlimited number of SLAs can be created, so it is important to provide a name that is descriptive enough to reflect its use.
* **Description.** Define the purpose of the SLA and what it covers. This description may be used to help in the selection of the SLA.
* **Working Time Calendar.** This is the defined work hours for the service desk that is responsible for fulfilling the SLA. A [Working Time Calendar (WTC)](/esp-config/customize/working-time-calendars) includes the timezone, days of the week, hours within each day, and exclusion days (such as holidays). The calculation of service-level targets is based on the selected WTC.

## [Service levels](/servicemanager-user-guide/service-portfolio/service-level-agreements/service-levels)
A service level is a measurable performance metric that helps define the quality of a service provided to a customer. 

![Service Levels](/_books/servicemanager-user-guide/service-portfolio/images/sla-levels-targets-events.png)

### [Service level targets](/servicemanager-user-guide/service-portfolio/service-level-agreements/service-levels#service-level-targets)
* **Response Time**. How quickly the service provider responds to a service request or issue.
* **Resolution Time**. The time it takes to resolve a service issue or complete a request.

### [Escalation events](/servicemanager-user-guide/service-portfolio/service-level-agreements/service-levels#escalation-events)
Escalation procedures can be defined for both response and resolution targets using a collection of time-based escalation events. 

These events include:
* Change in priority.
* Communications using email and Hornbill notifications.
* Re-assignments.
* Add to a Board.

## Linked services
The list of linked services provides a view of all services that use the selected SLA.  Additional services can be added through this interface.  

Before making any changes to an SLA, a review of all linked services should be undertaken.  Service owners should be made aware of any planned changes to the SLA.

:::note
Corporate SLAs are read-only when being viewed from a linked service. This is to prevent changes that might impact other services.  Changes to a corporate SLA must be made by accessing the corporate SLA from the list in the **Service Level Agreements** tab. 
:::