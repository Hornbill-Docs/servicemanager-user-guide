# Request Connections Action
A Request in Service Manager is generally provided to support or fulfill a request for an individual. However, there can often be times when there are other people who may have a connection to a particular request. For example, a change request may have been raised for an individual, but over time, others might ask for the same change. These additional people can be added as Interested connections.

![Request Connections Action](/_books/servicemanager-user-guide/images/request-connections-action.png)

## Before you begin
* Read about the how to [configure connections on a service](/servicemanager-user-guide/service-portfolio/services/service-connections).
* Read about the available [application settings](/servicemanager-config/advanced-tools-and-settings/application-settings#connections-settings).
* Read about the [connections automation](/servicemanager-config/customize/workflows/request-connections-automation) for workflow.

## Adding a Connection
### Search Customer
The Search Customer box allows you to search for both co-workers and contacts, with the option to add one or more as connections in one action.
* Match with first name, last name, or full name.
* Match with the company name of a contact.

### Connection Type
After searching for a customer, you are able to select the connection type from the selection option on the right-hand side of the Customer Search field. There are two included connection types listed as Interested and Impacted. The available list of connection types may vary depending on the setup of Service Manager and can be managed via a simple list in the admin console.

### Add Connection
Once a connection or connections have been found and the connection type has been selected, simply click on the Add button. The customer/s will be added to a Connections section within the request.

If the Connection type for the connection you are adding, will allow the connection to have visibility/access to the request via the employee portal, the agent will be presented with an information message to this effect before they confirm the addition of the connection to the request. This level of visibility to the requests is configured per service, per request type and per connection type on each of the service views. Service Connections

### Add a Comment
You can optionally add a comment when you are adding connections to the request. This comment will be displayed in the Timeline entry once you have completed the action of adding connections. The comment is also added to each entry in the Connections section of the request. Here, the comment can be edited if any changes are needed.

## Managing Connections
All added connections are displayed within a section titled Connections. From here you can use the Actions menu to manage the connection.

### Edit Connection Type
It may be that the connection type was incorrectly set for the customer. Using the Actions menu you can select Edit Connection Type. This makes the Connection Type next to that customer available to now select the correct Connection Type.

### Remove
If a connection is no longer needed you can use the Remove option under the Action menu to remove each connection. When the last connection is removed, the Connections section will no longer be available until another Connection is added.

### Filter
In the top right of the Connections section, an option is provided to allow you to filter on a particular Connection type. The default is set to All Connections.

## Email Communication
On the Email Action item, there is an option to include Connections as part of an email communication. Either All Connections can be added to the To, CC, or BCC fields of the email or you can select from one of the available Connection types. Once the Connections are added to the email, individual recipients can be removed if required.

## Administration

### Service Configuration
The Connections Action Item icon can be added or removed as part of the configuration of the Service that the request is associated with.

### Managing the Connection Types
The list of available Connection Types that are available to select from can be modified or added to within the Administration Portal. A Simple List called requestConnectionType is used to manage these. 

### Workflow Automated Tasks
The Workflow provides some Automated tasks for managing Connections. These allow you to add, remove, and email Connections.

Process

* Scope: Entity
* Entity: RequestConnections
* Type:Connections
* Tasks:
    * Add Connection
    * Email Connections
    * Remove All Connections
    * Remove Connection