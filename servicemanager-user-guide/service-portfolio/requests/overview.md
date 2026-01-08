# Request Form Overview
This document covers the main sections of the different types of requests.  

![Request Form](/_books/servicemanager-user-guide/images/request-form.png)

## Title Bar
The title bar extends across the top of a request form, containing several different elements.

![Request Title Bar](/_books/servicemanager-user-guide/images/request-title-bar.png)

#### Request ID
The request ID is an automatically generated, unique identifier for the request.  The default format for this identifier is a two-letter abbreviation of the type of request followed by eight digits.
* IN - Incident record
* SR - Service request
* CH - Change request
* PR - Problem record
* KE - Known error
* RM - Release managment record

:::tip
Custom request IDs can be constructed using [**Auto Values**](/esp-config/advanced-tools-and-settings/auto-values) which can provide a different format from the default.
:::

#### Subtitle
The subtitle, located directly below the request ID, is taken from the summary field on the request.  Providing a short but descriptive summary can add value throughout Service Manager as this is used in a wide variety of places to help identify the request.

#### Custom Buttons
The [custom buttons](/servicemanager-user-guide/service-portfolio/requests/request-custom-buttons) are a series of actions that can be defined by a Service Manager administrator.  These custom buttons can open a URL, display a pop-up with an embedded URL, or run an automated workflow known as an [Auto Task](/servicemanager-config/customize/service-manager-auto-tasks).

The display of the custom buttons will vary depending on the size of the browser window.  Smaller windows will place all the custom buttons under a single drop-down option.

#### Raise New
The raise new button provides two main paths for raising a request.  The main button can be clicked on to start the process of raising a request when the request type hasn't been decided on yet. Alternatively, by clicking on the drop-down arrow, a request type can be selected.

![Raise New](/_books/servicemanager-user-guide/images/request-raise-new-button.png)

:::note
The options available on the Raise New button may vary depending on how this has been configured in the [application settings](/servicemanager-config/advanced-tools-and-settings/application-settings#raise-new-button).
:::

#### Options Menu
* **Copy Request**.
The copy request will create a copy of the request
    * Customer
    * Link Request
    * Copy Attachments
    
* **Print Request**.
The [print option](/servicemanager-user-guide/service-portfolio/requests/print-action) will take you through a number of options to select which information to print.  

## Workflow Tracker
The workflow tracker highlights the stages and checkpoints that the request will work through.

## Request Actions
The [request actions](/servicemanager-user-guide/service-portfolio/requests/request-actions) are a series of updates or actions that can be applied to a request.  The available actions are defined by the service under which the request was raised.

![Request Actions](/_books/servicemanager-user-guide/service-portfolio/requests/images/action-bar.png)


## Information panel
The title and color at the top of the panel help identify the request type.
### Team and Owner
This displays the team and owner who currently have responsbility of managing the request. 
### Key information 
* Logged On
* Status
* Priority
* Impact
* Urgency
* Category

### Service information
The name of the service that this request was raised under.

### Service Level
The name of the service level that has been assigned to this request.

### Substatus and On-hold
##### On-hold

When a request does not have any substatuses defined, there will be an option to simply place the request on-hold.  When a request is placed on-hold, any service level timers are paused until the request is taken off-hold.

![On-hold button](/_books/servicemanager-user-guide/images/request-on-hold-button.png)

After clicking on the `Place On-Hold` button, options include
* The Pause Until Date/Time when the request will automatically come off-hold.
* The reason for placing the request on-hold.
* The timeline visibility (Team or Customer).

![On-hold Options](/_books/servicemanager-user-guide/images/on-hold-options.png)

:::tip
When the timeline visibility is set to **Customer**, an **Email Customer** option becomes available.  Selecting this option will send a **[predefined email notification that is based on a set email template](/servicemanager-config/advanced-tools-and-settings/application-settings#email-request-on-hold-update-to-customer)**.
:::

##### Substatuses
When substatuses are available, there will be a choice between active and on-hold statuses.  This ensures that a request can only be placed on-hold under certain conditions.  In some cases, a request may not have any on-hold substatuses, forcing the service level timers to always be running.

## Customer information
This section of the request contains information about the customer for whom the request was created.  The customer section is only available on incidents, service requests, and changes (when enabled).

## Details
The details section contains the two key fields for the summary and description of the request.  More fields can be added and managed using the form designer.

## Activities
The activities panel consists of tasks and authorizations that have been created for the request.  Tasks can be either manually added or created automatically from the workflow.  Authorizations can only be created using the workflow.

## Members
There may be times when you need to bring in some expertise from outside of the team to help with a request.  The Members feature can be used to add other Service Manager users and provide them with full access to the request.  

## Email Contacts
[Email Contacts](/servicemanager-user-guide/service-portfolio/requests/request-email-contacts) contains a list of recipients that are associated with a request. They are designed to improve speed and consistency when sending emails from a request by ensuring that relevant recipients are automatically included in communications.

![Email Contacts](/_books/servicemanager-user-guide/images/request-email-contacts.png)

## Timeline
The Timeline is an interactive timeline of events and discussions about the request.  
