# Resolve and close

Use the **Resolve and Close** action to update a request status to **Resolved** or **Closed**. This action allows you to document the resolution details and select a **Closure Category** to help with reporting and tracking.

<!-- [Visual Cue: Annotated screenshot showing the Resolve and Close action in the request action bar, highlighting the Closure Category dropdown and Resolution Text field.] -->

## Configuration options

When you use this action, you can interact with the following elements:

* **Resolve**: Sets the request status to **Resolved**.
* **Close**: Sets the request status to **Closed**.
* **Closure Category**: A dropdown menu to categorize why or how the request was finished.
* **Resolution Text**: A text field to provide details about the fix or the reason for the status change.
* **Editing**: Allows for modifications to the resolution details.

:::tip
If you set the visibility to **Customer**, the resolution tab and the resolution text become visible to the customer on the service portal.
:::

## System settings

You can customize how the **Resolve and Close** action behaves by adjusting settings in the administration area.

### Prevent resolution with outstanding activities

This setting stops a user from resolving a request if there are still open activities. You can still add more activities after the request is resolved if necessary.

* **Key**: `webapp.view.ITSM.serviceDesk.requests.resolve.denyWithOpenActivities`
* **Default**: Off
* **Scope**: Applies to all request types and services.

### Enforce closure category selection

This setting requires a user to select a **Closure Category** before they can resolve or close a request.

* **Key**: `servicemanager.request.closureCategory.default.required`
* **Default**: Off
* **Scope**: Applies to all request types and services.

### Enforce last item closure category

This setting requires the user to select the final element (the "leaf" node) in the closure category tree.

* **Key**: `guest.servicemanager.request.category.closure.enforceLastItem`
* **Default**: Off
* **Scope**: Applies to all request types and services.

### Resolve linked requests

This feature allows an analyst to resolve or close multiple requests that are linked to the current request.

* **Key**: `app.request.resolve.enableLinkedRequestAction`
* **Default**: Off

When you enable this setting:

* **Resolve**: The **Resolve** button displays a dropdown menu titled **Resolve Linked Requests**. You can select specific linked requests to resolve simultaneously. The list only shows requests that you have permission to resolve and excludes those already resolved or closed.
* **Close**: The **Close** button displays a dropdown menu titled **Close Linked Requests** (if linked requests are already resolved) or **Resolve Linked Requests** (if linked requests are still open). The list only shows requests you have permission to manage and excludes those already closed.

## Set up a two-stage closure workflow

A two-stage closure routine helps you manage the gap between providing a fix and officially closing the record. This process typically involves setting a request to **Resolved** and then waiting for customer confirmation or a set period (such as 7 days) before the system automatically sets the status to **Closed**.

### Common scenarios

1. **Resolution Accepted**: The customer accepts the resolution via the portal, or an analyst closes it for them. The status moves to **Closed**.
2. **Resolution Rejected**: The customer indicates the issue is not fixed. The status moves to **Open**.
3. **No Action**: The customer does not respond. The system automatically moves the status to **Closed** after a defined number of days.

### Configure the workflow nodes

To implement this, you must configure specific nodes within your request workflow.

**1. Suspend - Wait for Status Change**
Place this node after the request status is set to **Resolved**. This node pauses the automated process until the status changes to **Closed** or **Open**.

* **Expiry Period**: Use this field to set how long the node stays active before moving to the next step. This allows for automatic closure.
* **Note**: The expiry period uses working hours based on your **Working Time Calendar**.

**2. Decision Node**
Place a decision node immediately after the suspend node to branch the process based on the new status.

* **Reopened By Customer**: Create a branch for when the status changes from **Resolved** to **Open**.
* **Expired**: Create a branch for when the **Expiry Period** elapses while the status is still **Resolved**. This branch typically leads to an automated **Close** action.
* **No Match**: Create a branch for when the request status changes to **Closed**.

<!--[Visual Suggestion: Add a workflow diagram showing the "Suspend" node branching into three paths: "Reopened," "Expired/Auto-close," and "Manually Closed."] -->
