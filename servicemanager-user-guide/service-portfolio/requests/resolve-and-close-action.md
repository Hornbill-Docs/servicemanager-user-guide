# Resolve and Close
The Resolve and Close Action Item is used to set the request status to either Resolved or Closed. In addition to changing the status, information about the solution or information supporting the status change can be added along with the selection of a Closure Category.

## Options
* Resolve
* Close
* Closure Category
* Resolution Text
* Editing

:::tip
If the visibility is set to Customer, the resolution tab along with the resolution text is made available to the customer on the portal.
:::

## Settings

**Prevent resolution when there are outstanding Activities**
This setting prevents a request from being resolved when there are outstanding activities. Additional activities can be added after the request has been resolved if required.

`webapp.view.ITSM.serviceDesk.requests.resolve.denyWithOpenActivities`
* Default Setting is Off.
* This will apply to all request types for all services.

**Enforce the selection of a closure category**
This setting prevents a request from being resolved or closed until a Closure Category has been selected.

`servicemanager.request.closureCategory.default.required`
* Default is set to 'Off.
* This will apply to all request types for all services.

**Enforce the selection of a last item closure category**
Whether the user is forced to select the last tree element for the closure category.

`guest.servicemanager.request.category.closure.enforceLastItem`
* Default is set to Off.
* This will apply to all request types for all services.

**Resolve Linked Requests**
A Service Manager setting is available which enables a feature within the Request Close Action Item that allows an analyst to resolve one or more requests that are linked to the request that you are resolving or closing.

`app.request.resolve.enableLinkedRequestAction`
* Default is set to Off
* Resolve
    When this setting is enabled, the Resolve button will include an additioal drop-down option to Resolve Linked Requests. A list of the requests that are currently linked to the request you are resolving will be displayed. From this list, you can select which requests you would like to resolve at the same time.
    * The requests displayed will be filtered to those that you have the right to resolve, based on if the linked requests are logged against Services that your teams support.
    * Resolved/closed requests will not appear in the list.
* Close
    When this setting is enabled, the close button will include an additional drop-down option to Close Linked Requests if there are requests linked with the status of resolved. An additional option will be available to resolve requests if there are any linked requests that have a status of Open.
    * The requests displayed will be filtered to those that you have the rights to close/resolve, based on if the linked requests are logged against Services which your teams support.
    * Closed requests will not appear in the list.