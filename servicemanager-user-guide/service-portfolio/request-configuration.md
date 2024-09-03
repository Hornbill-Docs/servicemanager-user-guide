# Request Configuration
## Enabled / Disabled
Setting this to Enabled will make this request type available for use when raising requests against this service. When set to Disabled, this request type will not be available in Progressive Capture or when raising linked requests for this service.

## Workflow
The Workflow is an optional setting that allows you to associate a workflow which will be used as the default Workflow for all Incidents associated to this service. If left blank, the workflows that are specified in the app.requests.defaultBPMProcess Service Manager Settings will be used. If a Request Catalog Item is used the workflow in the Catalog Item will supersede both these settings.

## Email Configuration
The Email Configuration provides two options to set how email templates can be used on a the Email Action of a request.  

### Grouping
By selecting the different [grouping levels](/servicemanager-config/customize/email-templates#grouping), the email templates availabe on the request's email action can be managed. 

### EMail Template
Select an email template that will be used by default when sending emails from within a request using the Email Action Item. If left blank, the email template specified in the app.email.template.request.sendMessage Service Manager Setting. If both the Email Template option and the Service Manager Setting are not set, a blank plain text email will be sent without a template.

## Form Designer
It is possible for you to define custom fields to use against each request type per service. Using the form designer you can edit which default fields will be displayed in the Details section of each request form, as well as add new fields, set field validation, configure mandatory options and using drag and drop to re-order how the required fields will be displayed.

## Portal Process Tracker
When a Business Process Workflow is being used to support either the Service Requests or Incidents, it is possible to define what level of visibility you wish to give to your customers of the Process Tracker.
Off - The Process Tracker is hidden from customers.
Stages Only - Only the top level of the Process Tracker that shows the stages will be displayed.
Stages and Checkpoints - This will show both the Stages and the checkpoints.

## Request Actions
Define which Actions are available on the Request Action toolbar when working on requests raised against the Service.

![Request Action Tool bar](_books/servicemanager-user-guide/service-portfolio/services/images/request-action-toolbar.png)

Not all actions on a request are available by default and in some cases there are actions that are visible but not needed for a particular type of request. 

Enable or Disable an Action by clicking on the Enable or Disable Action button next to each action. See the [Request Action Overview](/servicemanager-user-guide/service-portfolio/requests/request-actions) for more information about each individual action.

![Request Actions](_books/servicemanager-user-guide/service-portfolio/services/images/request-actions.png)

:::tip
Actions that are available when a request is on hold are managed seperately through the [On Hold Settings](/servicemanager-config/administration/request-settings#on-hold-settings)
:::

## Request Categories
Define which logging and resolution categories are available per request type per service. It is possible to configure which level of the category tree will be the starting level (exposed) when choosing a category on a request, either using Progressive Capture or on the Request Details from. If a Category Level is not selected, the root of the category tree will be used.
Note: If the Category Level is filtered to the last level on a branch, no Categories will be visible for selection.