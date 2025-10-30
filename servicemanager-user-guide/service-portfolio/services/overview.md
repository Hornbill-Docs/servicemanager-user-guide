---
title: Overview of Services
layout: article
keywords: progressive capture 
---
# Services
The goal of a service is to deliver value to customers and employees through a variety of mechanisms.

## Planning your service catalog
The starting point to building a service catalog is to identify the services that are being offered. This could vary from a single service that offers IT help to users through self-serve, chat, and request management, to a large service catalog offering services across many different areas of the business.

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
