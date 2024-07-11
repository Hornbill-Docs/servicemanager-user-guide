# Authorization Action
The Authorization Action within a request allows for the selection of authorizers who will be sent an authorization task. Updates are recorded in the Timeline of the request, alongside the other update types to provide an audit trail of all actions for each request. This action item is only displayed when the Wait for List of Request Authorizers node has been used in a Workflow and this node has been reached.

## Authorizer Search
The Authorizer Search lets you search for individual Hornbill Users that you would like to have included in the authorization. Once a user has been located, click on the Add Authorizer button to add the user to the list of Authorizers.

## Associated Owners
The Associated Owners list is automatically populated with the owners of any linked assets, linked services, or the owner of the service that the request has been raised against. The purpose of this list is to present a list of possible users that may be required as part of the authorization. All of the users listed in the Associated Owners list can be added to the Authorizers list by clicking on the Add All button or any individual user can be added by clicking on the Add (+) button.

## Authorizers
The Authorizers list shows all of the users that have been selected for the authorization of this request. Some users may have been automatically added to this list as a result of the workflow pre-selecting the owners of the linked assets, linked services, or the owner of the service that the request is raised against.
