---
title: Overview of Services
layout: article
keywords: progressive capture 
---
# Services
The goal of a service is to deliver value to customers and employees through a variety of mechanisms.

## Planning your service catalog
The starting point to building a service catalog is to identify the services that are being offered. This could vary from a single service that offers IT help to users through self-serve, chat, and request management, to a large service catalog offering services across many different areas of the business.


## Supporting teams
The Supporting Teams feature is used to assign the service desk teams who will support the service. Each supporting team has the right to view and manage requests for the service. When a service is first created, it is supported by all service desk teams. Once one or more teams have been allocated to a service, only those teams have access to the service.

Only analysts who belong to those teams are able to view and manage requests made against the service.

Members of supporting teams can:

* View all requests raised against the service. Navigate to **Request list > Filters > All My Services**.
* Be assigned a request raised against the service from Intelligent Capture assignment forms, request forms, and multi-select assignment options on the Request List view.
* Assign or reassign a request to another team or analyst in a team (as long as the team or analyst that supports the service).
* Using the global search bar, see results for requests that are logged against services their teams support, or requests that are assigned to them, their teams, or where they have been added as members to the requests.

### Filtering the list of services displayed
Optionally, you can filter the list of services that are displayed on the Intelligent Capture > Services form. This could be to only display those services that belong to the customer they are logging the request for. You could also do this to display only those services the analyst supports (based on being a member of a team that supports one or more services). This could be useful, for example, if you only want the IT team to see the services they support, and equally you want the HR team to only see the services they support, when raising requests via Intelligent Capture.

To filter the list of services displayed, Hornbill administrators can turn on the [`servicemanager.progressiveCapture.servicedetails.enableSupportVisibility` setting](/servicemanager-config/advanced-tools-and-settings/application-settings#service-manager-forms), which is off by default.

## Subscribers
Subscribers are the people who consume the service. You can subscribe customers to a service based on various organization groups. By default, subscription settings allow all customers to use the service.

### Subscription options
* **Company.** Subscribes all internal customers to the service.
* **Department.** Subscribes defined departments to the service.
* **Team.** Subscribes defined teams to the service.
* **General.** Subscribes a defined organizational group to the service.
* **User.** Subscribes individual internal users to the service.
* **Site.** Subscribes all users of a given site to the service.
* **Contact Organization.** Subscribes specific external organizations to the service.
* **Individual Contacts.** Subscribes individual contacts to the service.
* **All Contacts.** Subscribes all defined contacts to all supported external organizations to the service.

:::tip
The Department, Team, and General options only appear in the dropdown list once they have been defined in **Configuration > Platform Configuration**.
:::

### Subscribing sub-groups
By default, each organizational grouping needs to be added individually to a service for its members to be subscribed to the service. If your organizational structure utilizes sub-groups linked to a parent group --- for example, departments under a company grouping, and the members of each department are listed under the relevant department but not also in the company grouping --- you may want to subscribe all the departments and therefore all the members by simply subscribing the parent company grouping. To facilitate this approach you can do the following:

To allow for subscribing of sub-groups, Hornbill administrators can turn on the `com.hornbill.servicemanager.services.subscriptions.allowSubgroupsInclusion` setting, which is off by default.

This enables users to subscribe sub-groups to a service based on the parent grouping being subscribed.

::: note
This will NOT automatically apply to existing group subscriptions and new group subscriptions.

With this setting enabled, you can choose to allow sub-group subscriptions when applying new group subscriptions and managing existing group subscriptions.
:::

When subscribing a new organizational grouping to a service, or managing an existing organizational group subscription to a service, a Sub-Grouping icon will now be visible. By default, this is disabled.

**To enable sub-group subscriptions:**
1. To subscribe all members of the sub-groups to the service based on the parent group's subscription, click the Sub-Grouping icon to enable the setting.
1. (Optional) To disable subgroups and their members' subscription to the service based on the parent group subscription, click the Sub-Grouping icon to disable it.

The sub-group option will not apply to non-organizational-based groupings such as sites, users, and contacts.

Catalog item visibility in the request catalog for sub-group members subscribed via their parent organizational grouping respects the parent's inclusion or exclusion of each catalog item's visibility.