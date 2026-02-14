---
title: Overview of Services
layout: article
keywords: progressive capture 
---
# Services

The goal of a service is to deliver value to customers and employees through a variety of mechanisms.

* Communications between the service desk and the customers.
* Incident reporting and management.
* Request fulfillment.
* Service availability.
* Continual service improvements.
* Service level agreements (SLAs).
* Self-service access through portals.

## Portal Visibility

If the Service will be visible on the Employee, Customer and Service Portals for subscribed users.

* **Visible:** Subscribed users will see, and have access to their requests raised against the Service, even if they you have restricted their ability to raise tickets from the portals for this Service.
* **Hidden:** Subscribed users will not see the Service on the Customer or Service portal - Useful when defining a technical Service rather than a business Service.

## Owner

Each Service requires an owner.  When a service is first created, it automatically allocates the creator of the service as the owner.

* Only the owner can change the owner to another user.
* Only the owner can change the Service Access option between `Private` and `Open`.
* When selecting a new owner, only users that have the *[Services Manager](/servicemanager-config/setup/service-manager-roles#services)* role will be available

## Service Access

The Service Access option allows the owner of a service to control who can modify the service details and configuration by using the options `Open` or `Private`.

![Service Access Options](/_books/servicemanager-user-guide/images/service-access-option.png)

* **Open:** Users with the *Services Manager* role who have [visibility of the service](/servicemanager-user-guide/service-portfolio/overview#service-visibility) can update and manage the details and configuration, excluding the ability to change the owner and the service access option.
* **Private:** Users with the *Services Manager* role who have [visibility of the service](/servicemanager-user-guide/service-portfolio/overview#service-visibility) are limited from making configuration changes. They can only add and update FAQs, bulletins, and the operational status. This allows a service owner to maintain full control of the service.

:::tip
A user that is a member of a team that support the service, but doesn't have the *Services Manager* role, will have limited access to the details of the service when accessed from a request or the request list. They can update FAQs, bulletins, and the operational status.
:::

## Activities

The Activities panel lets you create and managed tasks and activities against this service. This can be used for planning updates to any aspect of the service such as updating a workflow or Intelligent Capture.

## Supporting Teams

The Supporting Teams feature is used to assign dedicated [service desk teams](/servicemanager-config/administration/service-desk) that will support the service. Each supporting team has the right to view and manage requests for the service. When a service is first created, it is supported by all service desk teams. Once one or more dedicated teams have been allocated to a service, only those teams can see and manage the requests for that service.

![Supporting Teams](/_books/servicemanager-user-guide/images/service-supporting-teams.png)

#### Members of supporting teams can

* View all requests raised against the service. Navigate to **Request list > Filters > All My Services**.
* Be assigned a request raised against the service from Intelligent Capture assignment forms, request forms, and multi-select assignment options on the Request List view.
* Assign or reassign a request to another team or analyst in a team (as long as the team or analyst that supports the service).
* Using the global search bar, see results for requests that are logged against services their teams support, or requests that are assigned to them, their teams, or where they have been added as members to the requests.

#### Filtering the list of services displayed

Optionally, you can filter the list of services that are displayed on the Intelligent Capture > Services form. This could be to only display those services that belong to the customer they are logging the request for. You could also do this to display only those services the analyst supports (based on being a member of a team that supports one or more services). This could be useful, for example, if you only want the IT team to see the services they support, and equally you want the HR team to only see the services they support, when raising requests via Intelligent Capture.

To filter the list of services displayed, Hornbill administrators can turn on the [`servicemanager.progressiveCapture.servicedetails.enableSupportVisibility` setting](/servicemanager-config/advanced-tools-and-settings/application-settings#service-manager-forms), which is off by default.

## Subscribers

Subscribers are the people who consume the service. You can subscribe customers to a service based on various organization groups. By default, subscription settings allow all customers to use the service.

### Subscription options

* **General.** Search and subscribe groups that belong to the **General** type.
* **Team.** Subscribes defined teams to the service.
* **Department.** Search and subscribe groups that belong to the **Department** type.
* **Cost Center.** Search and subscribe groups that belong to the **Cost Center** type.
* **Division.** Search and subscribe groups that belong to the **Division** type.
* **Company.** Search and subscribe groups that belong to the **Company** type.
* **Business Unit.** Search and subscribe groups that belong to the **Business Unity** type.
* **Directorate.** Search and subscribe groups that belong to the **Directorate** type.
* **Branch.** Search and subscribe groups that belong to the **Branch** type.
* **Board.** Search and subscribe groups that belong to the **Board** type.
* **Subsidiary.** Search and subscribe groups that belong to the **Subsidiary** type.
* **Function.** Search and subscribe groups that belong to the **Function** type.
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

## Timeline

Each service provides an area where users who have access to the service can have a discussion about the service. This is a great way to plan or make suggestions for the service.

## Requests

The Requests list provides a view of all the requests that have been raised and associated with the service.

* **Direct Requests**. The list provided under Direct Requests are requests where the selected service is the primary service for the request.
* **Associated Requests**. The associated requests consist of requests that have had this service selected as a [linked service](/servicemanager-user-guide/service-portfolio/requests/linked-services-action).

## Assets

Associating the assets which support a service helps support quicker Incident and or Problem resolutions by making it quick and easy to understand what infrastructure is directly used to provide each service. Change management can benefit from visualizing impact when considering implementing changes to a service, or assets which support a service.

## Services

Associating services that support or underpin other services can help support incident and or problem resolutions by making it quick and easy to understand how services are related and if there are any dependencies between them. Change management can benefit from visualizing impact when considering implementing changes to a service.
