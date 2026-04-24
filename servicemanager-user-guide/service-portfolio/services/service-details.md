---
layout: article-toc
---
# Service details

Service details define the settings and values that make a service function. You can set the name, description, status, and other options when you create a new service.

![Service Details](/_books/servicemanager-user-guide/images/service-details-tab.png)

## Name

The service name identifies your service. This is a required field. The name appears in the following locations:

- Visible to [subscribed customers](/servicemanager-user-guide/service-portfolio/services/overview#subscribers) on the Employee and Customer portals.
- Visible to support staff in [Intelligent Capture](/esp-config/automation/intelligent-capture-designer) when using the Services Capture form.
- Listed in the Services column of the [Request List](/servicemanager-user-guide/request-list/overview).
- Shown on each request raised for the service.

Service names do not need to be unique. The same name can be used for different services. However, a unique name should be considered so the service can be easily identified.

## Description

Use the description to explain the purpose of the service. This information helps your users and support staff understand what the service offers. The description appears in the following locations:

- The Employee and Customer portals.
- The [Services Intelligent Capture](/servicemanager-config/customize/service-manager-capture-forms#services) form used by support staff.

## Configuration

### Type

The service type helps you organize your portfolio. You can choose from two types:

- **Business services**: These support business users in departments such as IT, accounting, marketing, and HR to improve productivity.
- **Technical services**: These provide technical support such as troubleshooting, repair, installation, and maintenance to keep systems running.

:::tip
The service type can be used with the workflow [Services Automation](/servicemanager-config/customize/workflows/services-automation) to automatically update the status of related services based on the type.
:::

### Category

Group services by selecting a category from the predefined list.

:::tip
Modify the [list of categories](/servicemanager-config/setup/service-manager-simple-lists#service-manager-simple-lists) in Service Manager configuration. Categories are stored in the `serviceCategory` Simple List.
:::

### Portfolio status

The portfolio status tracks the lifecycle of your service. Choose the status that matches the current stage of the service:

- **Pipeline**: Use this for the planning phase. The system hides the service from customers and support staff.
- **Catalog**: Use this when the service is live. Support staff and subscribers can select the service when they raise requests.
- **Retired**: Use this when the service is no longer active. The system removes the service from view.

### Service icon

Choose an icon to represent the service. This icon helps users visually identify the service on the Employee and Customer portals.

### Default mailbox

Select the [mailbox](/esp-config/email/shared-mailboxes) the system uses for emails sent manually from requests.

- If you do not select a mailbox, the system sends emails from the shared mailbox used by the agent.
- Agents must have permission to send from the default mailbox. If they do not have permission, the system uses a mailbox they are authorized to use.
- Agents with permissions for multiple mailboxes can change the default mailbox when they send an email manually.

## Employee Portal

Settings to publish the service to the Employee Portal:

- **Service Domain** - Associate the service with a domain (for example IT, HR, Facilities).
- **Domain Category** - Select a category for services in this domain.
