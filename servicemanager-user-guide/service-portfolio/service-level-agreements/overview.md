# Corporate Service Level Agreements
Service level agreements (SLAs) allow you to define a combination of service levels and service-level targets that can be used across multiple services sharing the same SLA requirements. Using corporate SLAs can centralize the management of these SLAs into one place rather than on a service-by-service basis.

![Corporate Service Levels](/_books/servicemanager-user-guide/service-portfolio/images/corporate-sla.png)

* Corporate service level agreements can be associated with one or more services.
* A service can be associated with both a corporate SLA and its own SLA.
* A service can have its own SLA without having a corporate SLA.

:::note
Corporate SLAs are read-only when being viewed from an associated service. This is to prevent changes that might impact other services.  Changes to a corporate SLA must be made by accessing the corporate SLA from the Service Level Agreements list. 
:::

## Before you begin
* A user must have the [Services Manager](/servicemanager-config/setup/service-manager-roles#services) 
role to access the Service Portfolio.
 
## Accessing corporate SLAs
1. In the [App toolbar](/esp-user-guide/navigation#app-toolbar), click the Service Management icon.
1. Select **Service Portfolio**.
1. Select the **Service Level Agreements** tab.

## Details
The following SLA Details are required when first creating a new SLA and are available within the SLA form.

* **Name**<br>The name of the Service Level Agreement will be used to fine and link to Services and will be visible on the requests that they are associated to. As an unlimited number of SLAs can be created so it is important to provide a name that is descriptive enough to reflect its use.
* **Description**<br>Define the purpose of the SLA and what it covers. This description may be used to help in the selection of a the SLA.
* **Working Time Calendar**<br>This is the defined work hours for the Service Desk that that is responsible for fulfilling the Service Level Agreement. A Working Time Calendar includes the timezone, days of the week, hours within each day, and exclusion days such as holidays. The calculation of Service Level Targets will be based on the selected Working Time Calendar.