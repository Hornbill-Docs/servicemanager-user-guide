# Request Configuration
## Enabled / Disabled
When this setting is set to *Enabled*, the request type is available for use when raising requests against this service. When set to *Disabled*, this request type is not available in Intelligent Capture or when raising linked requests for this service.

## Workflow
The Workflow field, an optional setting, allows you to associate a workflow that will be used as the default workflow for all incidents associated to this service. If left blank, the workflows that are specified in the `app.requests.defaultBPMProcess` application settings will be used (**Configuration > Service Manager > Advanced Tools & Settings > Application Settings**). 

If a request catalog item is used, the workflow in the catalog item will supersede both these settings.

## Email Configuration
The Email Configuration popup provides two options to set how email templates can be used on the email action of a request: **Groupings** and **Email Templates**.

Here you can select an email template group, then from the shorter list that subsequently appears in the Email Template dropdown, select the template you want to use for the request's email action.

Hornbill admins can create [grouping levels](/servicemanager-config/customize/email-templates#grouping) to organize the various email templates available for selection into more manageable groups.

The email template you select will be used by default when sending emails from within a request using the email action item. If left blank, the email template specified in the `app.email.template.request.sendMessage` Service Manager application setting will be used. If both the Email Template option and the Service Manager application setting are not set, a blank plain text email will be sent without a template.

## View Details Form
Using this popup, you can define custom fields to use against each request type per service. You can edit which default fields are displayed in the Details section of each request form, as well as add new fields, set field validation, configure mandatory options, and use drag and drop to re-order how the required fields are displayed.

## Portal HUD
When a workflow is being used to support either Service Requests or Incidents, you can define the level of visibility you wish to give to your customers using this process tracker (heads-up display).
* **Off.** The process tracker is hidden from customers.
* **Stages Only.** Only the top level of the process tracker that shows the stages is displayed.
* **Stages and Checkpoints.** Both the stages and the checkpoints are displayed.

## Request Actions
Define which actions are available on the Request Action toolbar when working on requests raised against the service.

![Request Action Tool bar](/_books/servicemanager-user-guide/service-portfolio/services/images/request-action-toolbar.png)

Not all actions on a request are available by default, and in some cases there are actions that are visible but not needed for a particular type of request. 

Enable or disable an action by clicking the **Enable Action** button next to each action. See the [Request Actions overview](/servicemanager-user-guide/service-portfolio/requests/request-actions) for more information about each individual action.

![Request Actions](/_books/servicemanager-user-guide/service-portfolio/services/images/request-actions.png)

:::tip
Actions that are available when a request is on hold are managed separately through the [On Hold Settings](/servicemanager-config/administration/request-settings#on-hold-settings).
:::

## Request Categories
Define which logging and resolution categories are available per request type per service. You can configure which level of the category tree will be the starting level (exposed) when choosing a category on a request, either using Intelligent Capture or on the Request Details form. If a category level is not selected, the root of the category tree will be used.

**Note:** If the category level is filtered to the last level on a branch, no categories will be visible for selection.