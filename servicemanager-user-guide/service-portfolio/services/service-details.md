---
layout: article-toc
---
# Service details

Service details define the settings and values required to make a service work. Set the name, description, status, and other required options when creating the service.

![Service Details](/_books/servicemanager-user-guide/images/service-details-tab.png)

## Name

The service name is required. It appears in several places:

- Visible to [subscribed customers](/servicemanager-user-guide/service-portfolio/services/overview#subscribers) on the Employee and Customer portals.
- Visible to support staff in [Intelligent Capture](/esp-config/automation/intelligent-capture-designer) when using the Services Capture form.
- Listed in the Services column of the [Request List](/servicemanager-user-guide/request-list/overview).
- Shown on each request raised for the service.

Consider name length and how it displays in different areas. Service names are not required to be unique; different services can use the same name.

If you support multiple languages, provide translations for the name and description. Users see the translation that matches their profile language.

## Description

Add a brief description to explain the service purpose. Customers see this description on the Employee and Customer portals. Support staff see it in the Services Intelligent Capture form.

## Type

Service types: *business* and *technical*.

- **Business services** - Support business users (for example IT, accounting, marketing, HR) to improve efficiency and productivity.
- **Technical services** - Provide technical support such as troubleshooting, repair, installation, and maintenance to keep systems running.

:::tip
The service type can be used with the workflow [Services Automation](/servicemanager-config/customize/workflows/services-automation) to automatically update the status of related services based on the type.
:::

## Category

Group services by selecting a category from the predefined list.

:::tip
Modify the [list of categories](/servicemanager-config/setup/service-manager-simple-lists#service-manager-simple-lists) in Service Manager configuration. Categories are stored in the `serviceCategories` Simple List.
:::

### Portfolio status

Portfolio statuses show a service's lifecycle: Pipeline, Catalog, and Retired.

- **Pipeline** - Planning phase. The service is hidden from customers and support staff.
- **Catalog** - The service is live. Support staff and subscribers can select it when raising requests.
- **Retired** - The service is no longer active and is removed from view.

### Employee Portal

Settings to publish the service to the Employee Portal:

- **Service Domain** - Associate the service with a domain (for example IT, HR, Facilities).
- **Domain Category** - Select a category for services in this domain.

### Default mailbox

Choose the [mailbox](/esp-config/email/shared-mailboxes) used for manually sent emails on requests for this service.

- If no mailbox is selected, emails are sent from the shared mailbox used by the agent.
- Agents must have send rights for the default mailbox; otherwise, the system uses a mailbox they can send from.
- Agents with rights to multiple mailboxes can override the default when sending manually.

### Service icon

Select an icon to represent the service on the Employee and Customer portals.
