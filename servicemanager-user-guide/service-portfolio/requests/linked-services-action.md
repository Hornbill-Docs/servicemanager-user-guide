# Linked Services Action
The Linked Services Action within a request allows for the linking of other Services to a request, over and above the service against which the request has been logged. This is useful in situations where you might want to record which other services were impacted.

![Linked Services Action](/_books/servicemanager-user-guide/service-portfolio/requests/images/linked-services-action.png)

## Before You Begin
The visibility of the Linked Services Action on a request is controlled by the service that the request is raised under. If the Linked Services Action is not available, the Service Owner for that service will need to [enable it on the service](/servicemanager-user-guide/service-portfolio/request-configuration#request-actions). 


## Linking Services
To link one or more services to a request, select the service you wish to add, then choose the appropriate Relationship Link, and then select the link.
* The list of available Relationships is configured in the Service Manager Configuration under Relationships. Only Active Request to Services Relationship Links will be available.
* A timeline post will audit the adding of the additional services.
Should you wish to change this from the default of Team, alter the Visibility level before selecting the Link button.
* The Linked Services will be visible from a collapsible Linked Services section below the request action items.

## Viewing Linked Services
Once services have been linked to a request, you can view and edit their relationship to the request from a new collapsible section below the action item bar.
* **Edit Relationship**<br>Use this option from the drop-down to select a different Relationship Link. This change will be audited by a post to the request timeline.
* **Remove**<br>Use this option from the drop-down to remove the Service from the request. This action will be audited by a post to the request timeline.

## Services View
Once a service has been linked to a request, under the Services view and the Requests tab, you will see two tabs:
* **Direct Requests**<br>This shows all requests that have been raised directly against the service.
* **Associated Requests**<br>This shows all requests to which the service has been linked, including the specific relationship it has to each request.