# Resolve and close

Use the **Resolve and Close** action to update a request status to **Resolved** or **Closed**. This action allows you to document the resolution description and select a **Closure Category** to help with reporting and tracking.

![Resolve and Close Action](/_books/servicemanager-user-guide/service-portfolio/requests/images/resolve-and-close-action.png)

## Resolving a request

When a request has an open status, the resolution action is available to record the resolution details and to progress the status to being resolved.

### Resolution description

This field is used to add a description of how the resolution was achieved. It is important to provide detailed and clear information as this resolution may be presented to the customer or used for knowledge article creation.

#### HAi Text Assist

![HAi Assist logo](/_books/servicemanager-user-guide/images/hai-logo-22x22.png) [HAi Text Assist](/servicemanager-user-guide/hai/text-assist) is an AI tool that helps you write the resolution description. Clear and concise resolutions improve communication with your team and customers.

* **Ask HAi**: Enter an open-ended prompt to find solutions for common issues. For example, type "How to set up an email signature in Outlook in Office 365."
* **Change Tone**: Adjust the tone of your text to suit your audience. Options include Apologetic, Professional, Friendly, and Technical.
* **Improve Text**: Correct spelling and grammar mistakes to improve readability.
* **Shorten Text**: Remove unnecessary words from your update.
* **Listify**: Convert blocks of text into a list format.

### Category

A closure category can be selected when the request is being either resolved or closed. This category is often used as a way to specify how the request was resolved, for example, a patch, a setting change, training, or a system restart. This can be a great way to contribute toward reporting and statistics on how requests are being resolved.

* [Mandatory Category Selection](/servicemanager-config/advanced-tools-and-settings/application-settings#category-settings): A setting is available that enforces the selection of a category, before the resolution can be applied.
* [Last Item Selection](/servicemanager-config/advanced-tools-and-settings/application-settings#category-settings): A setting is available that enforces the selection of the last item of a branch.

## Closing a request

Once a request is in a resolved state, additional options are available as part of a request closure.

* **Reopen**: In a case where the resolution didn't solve the issue, the **Reopen** option can set the status of the request back to **Open**.
* **Edit**: Allows for modifications to the resolution description and the category.
* **Knowledge**: This option includes viewing any existing articles and the creation of a new article that is based on the resolution.
  * *Create Article*: Selecting this option will take the request summary and the resolution description and add it to a new knowledge article.
  * ![HAi Assist logo](/_books/servicemanager-user-guide/images/hai-logo-22x22.png) *HAi Generate Article*: Use the [HAi Knowledge Generator](/servicemanager-user-guide/hai/knowledge-generator) to automatically create a knowledge article based on the information stored in the request.

## Locking the resolution and closure

Both the resolve and close on a request can be locked manually or automatically. When locked, only someone with appropriate rights can make any changes to the resolution or closure information.

## Timeline visibility

If you set the visibility to **Customer**, the resolution tab and the resolution text become visible to the customer in the self service portals.

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
