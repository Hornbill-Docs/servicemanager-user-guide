# Request Sub-Statuses
The Request Sub-statuses lets you define a number of descriptive states of a request that are related to the request being either Active or On-hold. Using the Sub-status can help control the situations under which a request is put On-hold or made Active again. An example of an On-hold Sub-status might be With Customer which when selected could place the request's status to On-hold and stop any allocated Service Level Target timers.

* Create descriptive sub-statuses to enhance the New, Open, and Resolved statuses
* Have better control over placing requests on hold
* Automate the changing of the sub-statuses
* Define Global Request Sub-statuses that are applied to all requests for a specific request type

## Sub-status Configuration
The creation and management of the Request Sub-statuses is done from within each individual Service form. Click on the + New Sub-status button to add a new sub-status, or select the edit icon on an existing sub-status.

Each individual sub-status contains the following options.

* **Sub-status Name**<br>The Name of the sub-status is what will be displayed to an analyst from within a request.
* **Alternative Customer Label**<br>An alternative Label can be provided which will be visible to the customer from within the Customer or Service Portals. This is only applicable to request types that are accessible on the Portals.
* **Request Type**<br>A sub-status can be made available to All requests types or you can select from one of the available request types on which this particular Sub-status will be available.
* **Parent Status**<br>The selection of a sub-status controls if the request is placed in either an Active or On-hold state when the sub-status is selected. A Sub-status that is set with a Parent Status of Active will either keep the request in an active state (New, Open, Resolved) or if the request is On-hold the state will change back to its Active state. A Sub-status that is set with a Parent Status of On-hold will either change the status of the the request to On-hold if it is currently in an active state (New, Open, Resolve) or it will maintain an On-hold state if it already on-hold.
* **Reason Required**<br>This setting is used to enforce an entry by the user that is putting the request on-hold for this particular sub-state.
* **Pause Until Date / Time**<br>If choosing the Parent Status of On-Hold, this option will allow you to determine if the analyst moving the request into a specific sub-status will be prompted to put it on-hold until a defined date and time, after which it will automatically come off-hold, or if you choose No the analyst will not be prompted to set an on-hold until date and time, and instead the request will remain on-hold until it is manually taken off-hold. If choosing this option the analyst will be presented with the option to set a reminder activity when placing the request into this on-hold status.

:::tip
When creating your sub-statuses it is important that at least one Active sub-status exists to allow you to move from an On-hold state to an Active state.
Use Request Settings to control which actions on a request are enabled when a request is on hold.
:::

## On Customer Response Change Sub-Status to...
Sub-statuses can often be used for scenarios where a request has been put on hold as some feedback or an update is required by the customer before proceeding. When the On Customer Response option is set, this allows the sub-status to automatically change to the selected sub-status when one of the following actions is performed on the request:

### Self Service Actions
The sub-status will change automatically when the Customer...
* adds a comment to a post
* adds a post (update)
* adds an attachment
* confirms a resolution has worked
* confirms a resolution hasn't worked

### Email Actions
The sub-status will change automatically when an email is...
* manually applied to a request
* automatically added to a request via email Routing Rules
It's not possible to tailor this behavior beyond the scenarios listed above.

## On Auto Off-hold Change Sub-Status to...
When a request is place on hold by a support person an option can be enabled for each On-hold sub-status that prompts the support person to enter a date and time for the request to become active again. When a sub-status has been set in the On Auto Off-hold field, the sub-status will automatically change to the the selected sub-status when the request comes off-hold.

:::tip
If a request is in an On-hold state at the time it is resolved, the request will automatically be taken off hold. The sub-status set within this configuration will then be applied to the request.
:::

## Plug-ins
### Supplier Manager
With Supplier Manager installed you can automate the starting of Supplier Contract events from Service Manager Requests.

#### Contract Requirements
In order to link a Service Manager request to a Supplier Contract, you must have an active Contract with associated assets.

* **Activate Contract**<br>Be sure that a Supplier has a contract set up and that the contract status is set to Active. The current date must also fall within the Start and End dates of the contract
* **Assets**<br>Link assets to both the supplier and the contract. When an asset is associated to a Service Manager request, the supplier and contract for the asset will be available to select.
* **Events**<br>Optionally, an event can be added to the contract. Within the Event Details section of the contract you can add an Event that has a set target time (in minutes). This can be used as the expected response or fix time from the supplier. The amount of time left in a Supplier Event will be visible on the Service Manager request that is linked to the contract. The Contact Email, also defined in the Event Details section is displayed on a request to allow an agent to get in touch with the supplier when an issue occurs with one of their assets. The setting app.request.stopActiveSupplierContractEventOnResolutionis provided to allow events to automatically end when a linked request is resolved.

#### Sub-status Configuration
The Supplier Manager plug-in is used in conjunction with Service Manager Request Sub-statuses.

* **Enable Supplier**<br>Either on the global sub-status in Admin or on the Service based sub-status, enable this switch.

#### Using the Plug-in
The Supplier Manager plug-in is initiated when a sub-status is selected which has the Supplier Integration enabled.

* **Link Asset**<br>Using the Asset Action on a request, link an asset to the request
* **Sub-status**<br>Select Sub-status (eg With Supplier) that has the plug-in enabled on it.
* **Supplier and Contract**<br>You will be prompted to select the Supplier and the contract that is associated to both the supplier and the linked asset.
* **Supplier Information**<br>Once a request is linked to a supplier and contract, this information will be displayed on the right hand side of the request form.


<!-- https://wiki.hornbill.com/index.php?title=Request_Sub-statuses-->