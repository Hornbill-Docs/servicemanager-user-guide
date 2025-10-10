# Connections configuration
A Request in Service Manager is generally provided to support or fulfill a request for an individual. However, there are times when other people might have a connection to a particular request. For example, an incident may have been raised for an individual, but others users might be impacted by this same incident. These additional people can be added as connections.

This document covers how to set up connections for each service.

![Connections Configuration](/_books/servicemanager-user-guide/images/service-connections-configuration.png)

## Before you begin
* Read about the [Connections Action](/servicemanager-user-guide/service-portfolio/requests/connection-action) on a request.
* Read about the available [application settings](/servicemanager-config/advanced-tools-and-settings/application-settings#connections-settings).
* Read about the [Connections Automation](/servicemanager-config/customize/workflows/request-connections-automation) for workflow.
* Read about the [Connections Intelligent Capture form](/servicemanager-config/customize/service-manager-capture-forms#connections).

## Connection Types
Connection types are a key part to controlling what a connected user can see or do on a request that they are connected to. By default, all visibility options are disabled for each connection type.

:::info
The connection types are defined in a [Simple List](/servicemanager-config/setup/service-manager-simple-lists) called `requestConnectionType`. The entire list of connection types defined in the simple list will be dispayed in the service connections configuration.
:::

When adding a connection to a request, a connection type must be selected.  The selected connection type will determine what access is provided to the connected user.

#### View Request
Each connection type allows you to select from incidents, service requests, and changes as request types that can be viewed by the connected user on the Employee Portal when that connection type is used.

Connections will have the following levels of access on these requests:
* View the request summary, description, status, and date logged.
* View the Business Process Tracker (Head's Up Display).
* View the questions section of the request.
* View who else is a connection to the request.
* The connected users will not be able to interact with the request, add updates or comments, add / view attachments, resolve, cancel or provide feedback on closure of the request.

:::tip
In order for Connections to view and download attachments, the setting `guest.servicemanager.portal.request.canConnectionsViewAttachments` needs to be enabled.
:::

#### Allow Collaboration
If you allow collaboration on any of the available request types, the connections added using this connection type will have all the View Requests visibility options plus the following:

* View the request's Timeline and see any update that is marked as visibile to the customer.
* Have the ability to add comments to any customer facing updates in the request timeline.
* Have the ability to add new updates to the request.
* The connected users will NOT be able to add attachments, resolve, cancel or provide feedback on closure of the request.

:::info
To collaborate on a request the connection must also have view access.  When selecting a request type under collaboration, if the View Request is not enabled for that request type, it will be automatically enabled.
:::

#### Available to portal users
When at least one connection type has the `Available to portal users` enabled, the customer of the request then has the ability to add connections to the request. Only the connection types that have this enable will be available to the customer to select from. 

![Available to Portal User](/_books/servicemanager-user-guide/images/service-connections-portal-access.png)

#### Get Email Request Updates
This option enables two types of email notification.
* Notify the connected user that they have been added as a connection.
* Notify the connected user when there has been a customer facing update to the request and the Notify Customer option has been enabled.

## Where can connections view requests?
Anyone added as a connection can view the request on the Employee Portal, provided that visibility has been set to allow access.  

:::note
While contacts from external organization can be connected to a request, the Customer Portal does not provide visibility of these requests.
:::

A connected user will see a new menu option in their list of requests, called Connections

* A new Connection Type Filter will allow the user to filter the requests they are connected to via the available connection types
Communication with request connections (emails) are managed via business process automation and or via the email action option on the request views.

## Remove connection
Connections will have an option via the Connections section on the request to remove themselves from being a connection to the request.

If a connection removes themselves as a connection to a request, they will no longer have rights to view the request.

## Connection comparison

| **Employee Portal Visibility/Action**              | **Customer** | **Connection (Collaboration)** | **Connection (View)** |
|----------------------------------------------------|--------------|--------------------------------|-----------------------|
| View Summary, Description, Logged Date             | Yes          | Yes                            | Yes                   |
| View Resolution target time, Sub status            | Yes          | Yes                            | Yes                   |
| View Connections                                   | Yes          | Yes                            | Yes                   |
| View Questions                                     | Yes          | Yes                            | Yes                   |
| View Request Owner's Name                          | Yes          | Yes                            | Yes                   |
| View Request Owner's Phone Number                  | Yes          | Yes                            | Yes                   |
| View Timeline                                      | Yes          | Yes                            | No                    |
| Add a new Timeline Post                            | Yes          | Yes                            | No                    |
| Add a new comment to a timeline post               | Yes          | Yes                            | No                    |
| View Attachments                                   | Yes          | Yes                            | No                    |
| Add Attachments                                    | Yes          | No                             | No                    |
| Notification to assigned team/analyst of a post    | Yes          | Yes                            | N/A                   |
| Notification to assigned team/analyst of a comment | Yes          | Yes                            | N/A                   |
| Resolve/Reopen Request                             | Yes          | No                             | No                    |
| Cancel Request                                     | Yes          | No                             | No                    |
| Provide Feedback                                   | Yes          | No                             | No                    |
| Update on Hold status with a post                  | Yes          | Yes                            | N/A                   |
| Update On-hold substatus with a comment            | Yes          | Yes                            | N/A                   |
| Progress a workflow awaiting a customer update     | Yes          | Yes                            | N/A                   |
