# Overview of request actions 
The action bar at the top of each request contains the actions you can apply to a request. 

![Request Actions](/_books/servicemanager-user-guide/service-portfolio/requests/images/action-bar.png)

* The actions available on a request can be configured within the service they are associated with.
* The supporting workflow that sits behind the request can control the focus of an action when that action is required to be completed.
* Use the [Access Control automation](/servicemanager-config/customize/workflows/service-manager-workflows#access-control) to lock or unlock individual actions at any point within a workflow.
* [Request Settings](/servicemanager-config/administration/request-settings#on-hold-settings) control which of these options are enabled when an incident is on hold.

## Visibility
Each time an action is used, an entry is added to the timeline.  Each action has a "visibility level" associated with it that controls who can see the entry in the timeline. This will typically be "Team" or "Customer". The user can select the visibility to decide if the timeline entry will be customer facing ("customer" visibility) or private to the team working on the request ("team" visibility).
![Visibility of actions in timeline](/_books/servicemanager-user-guide/service-portfolio/requests/images/visibility-request-action.png)

While a user can change this at the time of performing the action, the default visibility for each action item can be configured in Service Manager settings. The default visibility settings can be easily found by typing the word "visibility" in the Configuration Search. 

<!--
## Linked Services
Link other related Services to the request
## Authorisers
Add Authorisers to a Request
## Email
Send an email directly from the request
## Customer
Change the customer that is associated to this request
## Assign
Reassign the request to another team or user
## Connections
Add other users that might have an interested in this request and keep them updated by email
## Escalate
Reset the Priority for this request
## Category
Set the Request Category
## Assets
Associate One or more assets to this request
## Boards
See what Boards this request is on or add it to a Board
## Solutions
If linked to a Problem Record this will present possible solutions
## Resolve and Close
Capture resolution details
## Cancel
Raised by mistake? Use this option to cancel a request
## Print
Select and Print details of the request -->