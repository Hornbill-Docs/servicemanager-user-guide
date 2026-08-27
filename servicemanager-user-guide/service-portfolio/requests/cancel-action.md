# Cancel action

The Cancel Action allows you to cancel the request. The cancellation of a request is a permanent action and canceled requests can't be reinstated.  

When a request is canceled:

* The status is changed to **Canceled**.
* The workflow is canceled.
* The active tasks are canceled.  

![Cancel Action](/_books/servicemanager-user-guide/service-portfolio/requests/images/cancel-action.png)

## Cancellation reasons

A number of default cancellation reasons are provided, and one needs to be chosen and a supporting description provided before the request can be canceled.

Cancellation reasons:

* Created in error
* Duplicate
* Not needed
* Other

## Roles

Only users with the appropriate Cancel application right will see the option to cancel a request. By default this includes the following roles:

* Incident Management Full Access (can cancel Incidents).
* Problem Management Full Access (can cancel Problems and KnownErrors).
* Change Management Full Access (can cancel Change requests).
* Release Management Full Access (can cancel Releases).
* Service Desk Admin (can cancel all request types).

## System settings

The following system settings can be managed by your system administrator to control the behavior once a request has been canceled.

|Setting|Description|
|-|-|
|webapp.view.ITSM.serviceDesk.requests.cancel.cancelRelatedActivities|This will cancel related activities when a request is canceled|
|guest.app.requests.notification.notificationType.cancelTeam|Notification type for the team that a canceled request is assigned to|
|guest.app.requests.notification.notificationType.cancel|Notification type for the owner that a canceled request is assigned to|
