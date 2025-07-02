# Request Catalog
The Request Catalog provides a structured way of promoting the available types of requests for a particular Service. Requests in the catalog are available to subscribed users of a service on the Hornbill Portals and can also be accessed by support staff to provide a standard way of raising a particular type of request. 

## Before You Begin
To create and manage the Request Catalogs the following user roles are needed to perform the different actions

|Role|Description|
|-|-|
|Services Manager Role|Required to View and Access the Services forms where the Request Catalogs are created|
|Progressive Capture Manager Role|Required to create and modify Capture Scripts that will be used with a catalog request model|
|Business Process Manager Role|Required to create and modify any workflow to be used with a catalog request model.|

:::tip
By default Change Requests can't be raised from the Customer or Employee Portal. Enabling the system setting: ***guest.servicemanager.portal.additionalRequestTypes.change*** will allow Changes marked with the visibility to `Portal` or `Both` to be visible on the portals. At least one request catalog item must exist for customers to raise a change.

Please beware that enabling this setting will also allow customers to see any historical changes that have been raised and they have been set as the customer of the Changes (even if no Change Catalog Items were used on the Change records).
:::

## How to Access
A request catalog can be created and managed for Incidents, Service Requests and Changes under the Request Configuration section of a Service.

1. From the Service Manager application icon on the left-hand menu bar, select `Service Portfolio`.
1. From the list of services, select a service to view the details of that service.
1. On the Service form select the Request Configuration tab.
1. Select either incident, service request, or change from the available request types.
1. Locate the section titled Request Catalog.

## Features
* **Title**<br>The name for the request, that will be displayed on the portals for customers, and to support staff in Intelligent Capture.
* **Description**<br>Provide information that describes the purpose of the request. This will be displayed on the portals for customers and to support staff in Intelligent Capture.
* **Intelligent Capture**<br>Select from defined scripts that can ask the customer or support agent pertinent questions when raising a request using this model.
* **Workflow**<br>Select which workflow will be invoked and followed when a request is raised.
* **Icon**<br>Select an icon that will represent the request in portals and in intelligent capture.
* **Visibility**<br>Decide if the request will be available on just the portals, or just to support staff, or to both.
* **Language**<br>Select the language that it is being written in. This will default to the language that is currently being used in the user's session.
* **Statuses**<br>
    ***Draft***<br>Is not visible on the portals or in intelligent capture.<br>
    ***Published***<br>Is visible on the portals or in intelligent capture.

## Managing
The available Catalog Items are displayed in a list under the Request Catalog section. From this list, there are three options available:

### Ordering Catalog Items
It is possible to influence the order in which the Catalog Items will appear on the portals (under the Service) by dragging and dropping to reorder the Catalog Items.
Managing Catalog Visibility - it is possible to configure which service subscribers can view each catalog item.

### Update and Delete
* **Update**<br>It is possible to edit the details or status or to add additional languages to the Catalog Item by selecting the update Cog icon
* **Delete**<br>It is possible to permanently delete the Catalog Item by selecting the Delete Bin icon
Information If this list is empty, subscribed users for this Service will not have an option to raise a request from the portals for this request type.

## Intelligent Capture
The Request Catalog Items have been created in a way to allow each Catalog Item to be published to either Portal Users, Support Staff, or both. Publishing a Catalog Item to both of these groups enables a member of the support team to raise a request on behalf of a user while following the same steps that the user would experience in the portals. This ensures that the same information is captured no matter what the source is.

### Service Details Form
The Service Details Form is required to give a support person the ability to select a Catalog Item when raising an Incident or Service Request. Selecting a service on the Service Details form will expose any available Catalog Items for that service.
* If no Catalog Items have been defined, the Service can be selected and the current progressive capture will continue to run
* If one or more Catalog Items have been defined, either the Service can be selected to continue with the current progressive capture or one of the individual Catalog Items can be selected which will run a new progressive capture that is specific to that item.

### Portal Only Catalog Items
The creation of a Capture Script that is only going to be available to users of the portals is as straightforward as going to Administration and creating a collection of forms and questions that the user will be stepped through to raise the appropriate request.

When building a Progressive Capture Script for this purpose there is only one thing to keep in mind. There are particular progressive capture forms that are not designed for use by portal users. If these forms are added to these progressive capture scripts they will simply be skipped and not visible to the user on the portals. These include the following forms:

* Customer Search
* Co-worker Search
* Contact Search
* Service Details
* Request Type
* Customer Request Type
* Analyst Assignment

### Support Staff Only Catalog Items
When a support person begins the steps of raising a request, they will start by clicking on the `Raise New` option or selecting a particular type of request, such as an incident, or service request. Each of these will run its own capture script. Within any of these capture scripts, the Service Details form may be included. It is this Service Details form that displays the Request Catalog for each Service. If one of these Catalog Items is selected, a new Progressive Capture Script will be launched.

Some of the information collected in the initial Capture Script may be relevant to the Catalog Model's specific Capture Script. In order to maintain this information between the two Capture Scripts, the same Capture forms must be included in both scripts. For example, if you use the Customer Search form in the initial Progressive Capture, and you want to retain the selected customer in the next script, the next script must also include the Customer Search form. If the information collected in the initial script is no longer relevant to the Catalog Item, simply leave that form out of the Catalog Item script.

### Shared Catalog Items
In some cases, you may be able to use the same Catalog Item in both the Portal and for the Support Staff. Using the considerations mentioned in the previous two sections, you can build a progressive capture script that lets you include support-specific forms that are skipped and not visible in the portals, but they can be added to retain information that the support person needs.

## Language
If you are working in a multilingual environment you can publish each catalog model in several different languages. Any user that has a matching language set against their profile will see this in their preferred language.

### Add a Translation
The Language option provides a list of all of the different languages that this has been translated into. A new catalog model will only show the language that was selected at the time of creation. To add a new translation click on the `Add Translation` button which will expose the options for publishing this in another language.
* **Language**<br>Select the new language that you wish to add.
* **Translate**<br>Clicking this button will take the original title and description from the default language and automatically translate these fields using Google Translate. The title and description fields will be automatically populated with this translation. These fields can also be manually edited to either add your translation or to correct any mistakes made by the automatic translation.
Clicking on the `Translate` button will overwrite any information that is already held in the title and description fields.

### Update a Translation
* **Delete Translation**<br>Clicking on this button will delete the language translation that is currently selected in the language pick list. The default language translation cannot be deleted, therefore this button is not available when the default language is selected. The default language is a fallback and is displayed to a user who is using a language that does not have an associated translation available.
* **Update**<br>If a manual change has been made to either the title or description fields, save these changes by clicking on the `Update` button
* **Preview Google Translate**<br>This is a sub-action of the Update button which is accessed by clicking on the arrow next to Update. This will translate the title and description fields using the default translation without saving it. This preview can then be saved using the main Update button.
* **Update with Google Translate**<br>This is a sub-action of the `Update` button which is accessed by clicking on the arrow next to `Update`. This will automatically translate and save the title and description fields.

## Request Catalog Visibility
Manage which service subscribers will have visibility of individual catalog items, by default all catalog items are visible to all service subscribers. Visibility applies to both the Service and Customer Portals as well as which catalog items are visible for the user in the user app when agents are raising requests via progressive capture.

### Configuring Visibility
Against each catalog item select the Manage Catalog Visibility icon. This will present a list of all the subscribed users of the service.
> By default, all subscribed users will have visibility of all catalog items

To remove a user's or group's visibility to a catalog item, simply toggle their visibility setting from Included to Excluded

* **Exclude All**<br>Choose this option to exclude all subscribed users of the service from viewing a catalog item.
* **Include All**<br>Choose this option to include all subscribed users of the service to view a catalog item.

#### Use Case Example
If you have a requirement to exclude one or multiple users from viewing a catalog item, but they are not directly subscribed to the service, but are subscribed via a group subscription, then you will first need to subscribe them to the service as an individual and then include or exclude them individually from within the Subscribers' List for the relevant catalog item.

### List Filters
* **Filter**<br>Search for a specific user or grouping
* **Subscribers**<br>Filter the list of subscribers by All Subscribers, Included Subscribers, and Excluded Subscribers.
* **Groupings**<br>Filter the list of subscribers by all groupings, or specific subscriber groupings.

Combine any of the above filters and search options to manage the displayed list of service subscribers.