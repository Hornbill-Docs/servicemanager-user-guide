# Service Dependancies
Relating the techincal services which support/underpinning business services helps support quicker Incident and or Problem resolutions by making it quick and easy to understand which services are related. Change management can benefit from visualizing impact when considering implementing changes to the business or techincal services.

## Relating Services
Use the + icon to begin the process of relating services:

Use the following filters to find the services to associate:

* Filter - Text match
* Type - Business or Techincal Service
* Category - Services of a specific category
* Status - Services in a specific status
* Owner - Services owned by a specific owner
* Portfolio Status - Services in Pipeline, Catalog or Retired

From the list of services, choose the Associate option next to each service to select and relate the service using one of the following dependencies:
* With No Dependencies - Relate the services, but indicate no dependencies between the services
* With this depending on xxx - Relate this service and indicate this service depends on the service you are relating it to.
* With xxx depending on this - Relate this service and indicate the service you are relating this to, depend on it
* As Mutually Dependant - Relate the services, and indicate they are mutually dependant on each other

xxx = The name of the service you are viewing when relating other services to it.

Once services are related and dependencies configured, you can edit or remove the dependencies by using the Action icons next to each related service.

## Utilize Service Dependancies
Via the business process designer (Under Requests > Request Services), it is possible in workflows to automate the adding or related services to a request, by leveraging the defined dependencies to the request service. A use case is to automatically associate all business services to a change or problem record, based on the technical service the change or problem record is raised against


It is also possible to automatically update the status of related services, through the business process designer (Under Request > Services). In the workflow of a request, you can leverage the dependencies between services and only update the services status of services related of specific dependency types to the request service. A use case is to automatically update the status of business services related to the request technical service, which in turn would be visible to subscribed users of the business services, notifying them that, the service is impacted by an issue.

## Launch Explorer (Configuration Manager Plugin)
If you have installed the Configuration Manager application on your instance, explore the related services graphically - the Ciexplorer service Asset.png icon will open the configuration explorer in a new tab.