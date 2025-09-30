# Connections configuration
Users and contacts can be added to requests as connections. It is possible to allow those connected users to have visibility of the requests they are connected to via the Employee Portal.

By default, connections do not have access to the requests that they are connected to.  This access has to be configured and enabled on each service.

![Connections Configuration](/_books/servicemanager-user-guide/images/service-connections-configuration.png)

## Before you begin
* Read about the [Connections action](/servicemanager-user-guide/service-portfolio/requests/connection-action) on a request.
* Read about the available [application settings](/servicemanager-config/advanced-tools-and-settings/application-settings#connections-settings).
* Read about the [Connections Automation](/servicemanager-config/customize/workflows/request-connections-automation) for workflow.

## Where can connections view requests?
If a connection is added to a request (via the request connections action, or via the business process connection options), you can define if connections of specific connection types and for specific request types, per service can view those requests via the My Services view or on the Employee Portal

This capability is not available in the following:
* Customer Portal (customer.hornbill.com/<Your Instance>)

A connected user will see a new menu option in their list of requests, called Connections

* A new Connection Type Filter will allow the user to filter the requests they are connected to via the available connection types
Communication with request connections (emails) are managed via business process automation and or via the email action option on the request views.


## Connections visibility options
The default position is that connections of a request have No visibility of requests they are connected too.

Connections can be granted one of two levels of visibility to requests they are connected too, configurable per service.

The two levels can be applied for each of the following:
* **By Request Type**<br>Connections of Incidents, Service Requests and Changes can be configured to be allowed visibility of requests, as these request types are visible via the My Services view or the employee portal.
* **By Connection Type**<br>The available connection types are controlled by the connection types which you have configured on your instance. This is managed via a simple list in the admin console (Home > Service Manager > Simple Lists > RequestConnectionType)

## Connection levels
### View request
If you provide this option for connections of a specific type and for one or all request types against a service, the connections will have the following levels of access on these requests:

* View the request summary, description, status and date logged
* View the Business Process Tracker (Head's Up Display)
* View the questions section of the request
* View who else is a connection to the request
* The connected users will not be able to interact with the request, add updates or comments, add / view attachments, resolve, cancel or provide feedback on closure of the request

### Allow collaboration
If you provide this option for connections of a specific type and for one or all request types against a service, the connections will have all the View Requests visibility options plus the following:

* View the Timeline (Audit trail of the request) and see any updates which are marked at Customer visibility level
* Have the ability to add Comments to any customer facing updates in the request timeline
* Have the ability to add New updates to the request
* The connected users will NOT be able to add attachments, resolve, cancel or provide feedback on closure of the request.

:::tip
In order for Connections to view and download attachments, the setting `guest.servicemanager.portal.request.canConnectionsViewAttachments` needs to be enabled.
:::

### Available to portal users
Enabling this option will allow the customer of a request to add connections to their requests in the Employee Portal.

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
