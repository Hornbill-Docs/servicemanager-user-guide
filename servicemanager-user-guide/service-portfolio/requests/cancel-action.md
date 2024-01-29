# Cancel
The Cancel Action within a request provides the facility to cancel the request.

## Cancelation Reasons
A number of default cancelation reasons are provided, and one needs to be chosen and a supporting description provided before the request can be canceled.

Cancelation reasons:

* Created in error
* Duplicate
* Not needed
* Other

## Roles
Only users with the appropriate Cancel application right will see the option to cancel a request. By default this includes the following roles:

* Incident Management Full Access (can cancel Incidents)
* Problem Management Full Access (can cancel Problems and Known Errors)
* Change Management Full Access (can cancel Change requests)
* Release Management Full Access (can cancel Releases)
* Service Desk Admin (can cancel all request types)

## System Settings
The following system settings can be managed by your system administrator to control the behavior once a request has been canceled. 

|Setting|Description|
|-|-|
|webapp.view.ITSM.serviceDesk.requests.cancel.cancelRelatedActivities|This will cancel related activities when a request is canceled|
|guest.app.requests.notification.notificationType.cancelTeam|Notification type for the team that a canceled request is assigned to|
|guest.app.requests.notification.notificationType.cancel|Notification type for the owner that a canceled request is assigned to|