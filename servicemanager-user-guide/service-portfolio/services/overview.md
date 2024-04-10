# Service Overview
The goal of a service is to deliver value to customers and employees through a variety of mechanisms.

## Planning
The starting point to building a service catalog is to identify the services that are being offered. This could vary from a single service that offers IT help to users through self-serve, chat, and request management for a service catalog offering many services across different areas of the business.


## Supporting Teams
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