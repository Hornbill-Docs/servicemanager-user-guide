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

## Two Stage Closure
Many customers like to operate what is known as a “Two Stage Closure” routine after a resolution to a request has been established. This typically involves changing the status of the request to “Resolved” when the initial resolution has been provided to the customer and closing the request only when either a confirmation of the resolution has been received from the customer, or a certain period has elapsed without action or response, and the request should be automatically closed e.g. 7 days. This can be incorporated into Hornbill Service Manager using the configured Business Processes against your requests and this article explains how to set this up.

### Scenarios
Before configuring, its useful to consider the different scenarios when resolving and closing a request. What will be the same for every request is that it will be Resolved (i.e. have its status set to Resolved). This is typically performed by an Analyst entering a resolution within the Hornbill request, which may notify the customer.

1. **Resolution Accepted**<br>The customer accepts the resolution, either via the Service portal or the Analyst closing on their behalf. This moves the status of the request to Closed
2. **Resolution Rejected**<br>The customer advised the issue is not resolved or the resolution didn’t work, either by actioning this on the Service Portal or informing the Analyst who will reopen on their behalf. This moves the status of the request to Open
3. **No Action**<br>There is no response from the customer. Instead of the analysts having to remember to manually close these requests, the system will automatically close any resolved request after “X” number of days. This moves the status of the request to Closed

### Two Stage Closure Workflow
The above scenarios need to be configured within the Business Process of your request. 

* **Suspend - Wait for Status Change**<br>The first node to be set up is “Suspend - Wait for Status Change”. We know that by the time it reaches this node, the status of the request will be “Resolved”. This pauses the process until the status changes to either Closed or back to Open – as per the scenarios above.

    Within the configuration of this node, you will also have the option to set an Expiry Period. This is the period that this Suspend node will stay active for, before it automatically moves on to the next node in the process – which is how it possible to set up the automatic closure after a defined number of days. The expiry period is in working hours and will adhere to the hours configured in the Working Time Calendar.

* **Decision Node**<br>Following the suspend node, the decision node will determine the status that the request has been changed to. 

    1. **Reopened By Customer**<br>This decision criteria is based on if the status has been changed from Resolved to Open.
    2. **Expired**<br>This decision criteria is based on if the status has remained as resolved and Expiry Time we provided has elapsed. The expiry time is in working hours and will adhere to the hours configured in the "ServiceDeskDefaultCalendar" working time calendar found in Hornbill Administration.
    3. **No Match**<br>This refers to the only other option, which is that the request has been closed – and the criteria is based on if the status has been changed from resolved to closed.

<!--https://wiki.hornbill.com/index.php?title=Two_Stage_Closure -->