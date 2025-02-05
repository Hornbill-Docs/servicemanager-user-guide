# Corporate Service Level Agreements
Corporate service level agreements (SLAs) allow you to define a combination of service levels and service-level targets that can be used across multiple services sharing the same SLA requirements. By using corporate SLAs, you can centralize the management of all these SLAs into one place rather than on a service-by-service basis.

![Corporate Service Levels](/_books/servicemanager-user-guide/service-portfolio/images/corporate-sla.png)

## About corporate SLAs
* Corporate SLAs can be associated with one or more services.
* A service can be associated with both a corporate SLA and its own SLA.
* A service can have its own SLA without having a corporate SLA.

:::note
Corporate SLAs are read-only when being viewed from an associated service. This is to prevent changes that might impact other services.  Changes to a corporate SLA must be made by accessing the corporate SLA from the list in the **Service Level Agreements** tab. 
:::

## Before you begin
* A user must have the [Services Manager](/servicemanager-config/setup/service-manager-roles#services) 
role to access the Service Portfolio.
 
## Accessing corporate SLAs
**To access corporate SLAs:**
1. In the [App toolbar](/esp-user-guide/navigation#app-toolbar), click the Service Management icon.
1. Select **Service Portfolio**.
1. Select the **Service Level Agreements** tab.

## Details
The following SLA details are required when first creating a new SLA. These details are available within the SLA form.

* **Name.** The name of the SLA is used to find and link to services and is visible on the requests that it is associated to. An unlimited number of SLAs can be created, so it is important to provide a name that is descriptive enough to reflect its use.
* **Description.** Define the purpose of the SLA and what it covers. This description may be used to help in the selection of the SLA.
* **Working Time Calendar.** This is the defined work hours for the service desk that is responsible for fulfilling the SLA. A Working Time Calendar (WTC) includes the timezone, days of the week, hours within each day, and exclusion days (such as holidays). The calculation of service-level targets is based on the selected WTC.