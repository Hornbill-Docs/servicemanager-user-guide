# Linked Services Action
The Linked Service Action within a request allows for the linking of other Services to a request, over and above the Service against which the Request has been logged. This is useful in situations where you might want to record which other Services were impacted etc.

![Linked Services Action](_books/servicemanager-user-guide/service-portfolio/requests/images/linked-services-action.png)

## Before You Begin
The visibility of the Linked Services Action on a request is controlled by the service that the request is raised under. If the Linked Services Action is not available, the Service Owner for that service will need to [enable it on the service](/servicemanager-user-guide/service-portfolio/request-configuration#request-actions). 


## Linking Services
Link one or more services to a request, by selecting the service you wish to add, and then choosing the appropriate Relationship Link and then selecting the Link
* The list of available Relationships is configured in the Service Manager Configuration under Relationships. Only Active Request to Services Relationship Links will be available.
* A timeline post will audit the adding of the additional services.
Alter the Visibility level before selecting the Link button, should you wish to change this from the default of Team.
* The Linked Services will be visible from a collapsible Linked Services section below the request action items.

## Viewing Linked Services
Once Services have been linked to a Request, you will be able to view and edit their relationship to the request from a new collapsible section below the action item bar.
* **Edit Relationship**<br>Use this option from the drop-down to select a different Relationship Link, this change will be audited by a post to the request timeline.
* **Remove**<br>Use this option from the drop-down to remove the Service from the request, this action will be audited by a post to the request timeline.

## Services View
Once a Service has been linked to a Request, under the Services view and the Requests tab, you will see two tabs:
* **Direct Requests**<br>This will show all requests which have been raised directly against the service
* **Associated Requests**<br>This will show all requests to which the Service has been linked, including the specific relationship it has to each request.