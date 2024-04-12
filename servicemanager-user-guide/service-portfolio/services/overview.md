# Service Overview
The goal of a service is to deliver value to customers and employees through a variety of mechanisms.

## Planning
The starting point to building a service catalog is to identify the services that are being offered. This could vary from a single service that offers IT help to users through self-serve, chat, and request management for a service catalog offering many services across different areas of the business.


## Support Teams
The Supporting Teams feature is used to assign the Service Desk teams who will be supporting this service. Supporting teams will have the right to view and manage requests for this service. When a service is first created, it is supported by all Service Desk teams. Once one or more teams have been allocated to a service, only those teams will have access to the service.

Members of Supporting Teams can:

* View All requests raised against the Service from the Request list > Filters > All My Services.
* Be Assigned a request raised against the Service from Progressive Capture assignment forms, Request forms, and multi-select assignment options on the Request List view.
* Only analysts who belong to those teams will be able to view and manage requests made against the Service.
* It will only be possible to assign or reassign a request to another team or analyst in a team that supports the Service
* Using the global search bar, analysts will only see results for requests that are logged against services their teams support, or requests that are assigned to them, their teams or where they have been added as members to the requests.

Optionally you can also filter the list of Services that are displayed on the Progressive Capture > Services Form, to only display those that belong to the customer they are logging the request for, but also just to those services which the Analyst supports (based on being a member of a team that Supports one or more Services). This could be useful if you only want the IT team to see the Services they Support, and equally the HR team to only see the Services they support when raising requests via Progressive Capture.

To enable this feature the following system setting needs to be turned on (is defaulted to Off). The Setting is accessible from the admin tool under Home > Service Manager > Application Settings
servicemanager.progressiveCapture.servicedetails.enableSupportVisibility

## Subscribers
Subscribers refer to those that consume the service.  It is possible to subscribe customers to a service based on various organization groups. The default position for a service is that all customers will be entitled to use the Service.

### Subscription Option Types
* Company - Use this option to subscribe all internal customers to the Service
* Department - Use this option to subscribe defined Departments to the Service
* Team - Use this option to subscribe defined Teams to the Service
* General - Use this option to subscribe a defined organizational group to the Service
* User - Use this option to subscribe individual internal users to the Service
* Site - Use this option to subscribe all users of a given site to the Service
* Contact Organization - Use this option to subscribe specific external organizations to the Service
* Individual Contacts - Use this option to subscribe individual contacts to the service
* All Contacts - Use this option to subscribe all defined contacts to all supported external organizations to the Service

:::tip
Department, Team and General options will only appear in the drop list once they have been defined under the Platform Configuration.
:::

### Subscribing Sub-Groups
By default each organizational grouping needs to be added individually to a service, for it's members to be subscribed to the service. In the case where you have an organizational structure where you are utilizing sub-groups linked to a parent group - i.e Departments under a Company grouping, and the members of each department are listed under the relevant department but not also in the Company Grouping, you may want to subscribe all the departments and therefore all the members by simply subscribing the parent company grouping. To facilitate this approach you can do the following:

* Enable the com.hornbill.servicemanager.services.subscriptions.allowSubgroupsInclusion system setting
This will enable the ability to subscribe sub-groups to a service based on the parent grouping being subscribed - but it will not automatically:
    * Apply to existing Group Subscriptions
    * Apply to new Group Subscriptions

    With the setting enabled, you can now choose to allow sub-group subscriptions when applying new group subscriptions, and managing existing group subscriptions to a service.

#### Enabling Sub-Group Subscriptions
When subscribing a new organizational grouping to a service, or managing an existing organizational group subscription to a service, a Sub-Grouping Icon will now be visible.

* By Default this will be set to Disabled
* To Subscribe all members of the sub-groups to the service, based on their parent groups subscription, click on the icon to Enable.
* To disable subgroup and their member's subscription to the service, based on the parent grouping subscription simply click on the Icon to disable it.
* The sub-group option will not apply to non-organizational based groupings i.e sites, users, and contacts.

Catalog Item Visibility in the Request Catalog for Sub-Group members subscribed via their Parent Organizational Grouping, will respect the parent's inclusion or exclusion of each catalog item's visibility.