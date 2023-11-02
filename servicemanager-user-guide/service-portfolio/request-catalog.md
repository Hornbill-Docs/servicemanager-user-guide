# Request Catalog
The Request Catalogs provide a structured way of promoting the available types of requests for a particular Service. Items in the Request Catalog are available to subscribed users of a Service on the Hornbill Portals and can also be accessed by Support Staff to provide a standard way of raising a particular type of request. Each item in the Request Catalog can be configured to run its own unique Capture Script allowing you to prompt for information required for that request and it can run its own Business Process Workflow to define how that request will be fulfilled.


## Before You Begin
In order to create and manage the Request Catalogs the following user roles are needed to perform the different actions

|Role|Description|
|-|-|
|Service Manager Role|Required to View and Access the Services forms where the Request Catalogs are created|
|Progressive Capture Manager Role|Required to create and modify and Progressive Capture Scripts to be used with a Catalog Item|
|Business Process Manager Role|Required to create and modify any Workflow to be used with a Catalog Item
Catalog items can be created to support Incident Management, Change Management and Request Fulfilment|


:::tip
By default Change Catalog Items can't be raised from the Customer or Service Portal. Enabling the system setting: guest.servicemanager.portal.additionalRequestTypes.change will allow Change Catalog items marked as Portal or Both visibility to be visible on the Portals.

Please beware that enabling this setting will also allow customers to see any historical changes which have been raised and they have been set as the customer of the Changes (even if no Change Catalog Items were used on the Change records).
:::


## Creation
Catalog Items can be created for Incidents, Service Requests and Changes under the Request Configuration section of a Service.

1. On the Service form select the Request Configuration tab
1. Locate the section titled Catalog Items
1. Click on the Add Catalog Item button

## Features

* **Title**<br>The name for the Catalog Item, which will be displayed on the portals for customers, and to support staff in Progressive Capture
* **Description**<br>Provide information which describes the purpose of the Catalog Item. This will be displayed on the portals for customers and to support staff in progressive Capture
* **Intelligent Capture**<br>Select from defined scripts which can ask the customer or support agent pertinent questions when raising a request for this Catalog Item
* **Workflow**<br>Select which workflow will be invoked and followed when a request is raised for this Catalog Item.
* **Icon**<br>Select an Icon which will represent the Catalog Item in portals and in progressive capture
* **Visibility**<br>Decide if the Catalog Item will be available on just the portals, or just to support staff, or to both.
* **Language**<br>Select the language that this Catalog Item is being written in. This will default to the language that is currently being used in the user's session
* **Statuses**<br>
    *Draft*<br>Is not visible on the portals or in progressive capture.
    *Published*<br>Is visible on the portals or in progressive capture.

## Managing
The available Catalog Items are displayed in a list under the Catalog Items section. From this list there are three options available

Ordering Catalog Items – It is possible to influence the order in which the Catalog Items will appear on the portals (under the Service) by dragging and dropping to reorder the Catalog Items.
Managing Catalog Visibility - it is possible to configure which service subscribers can view each catalog item
Update – It is possible to edit the details or status or to add additional languages to the Catalog Item by selecting the update Cog icon
Delete – It is possible to permanently delete the Catalog Item by selecting the Delete Bin icon
Information If this list is empty, subscribed users for this Service will not have an option to raise a request from the portals for this request type.

Intelligent Capture
The Request Catalog Items have been created in a way to allow each Catalog Item to be published to either Portal Users, Support Staff, or both. Publishing a Catalog Item to both of these groups enables a member of the support team to raise a request on behalf of a user while following the same steps that the user would experience in the portals. This ensures that the same information is captured no matter what the source is.

Capture Service Form
Service Details Form
The Service Details Form is required to give a support person the ability to select a Catalog Item when raising an Incident or Service Request. Selecting a service on the Service Details form will expose any available Catalog Items for that service.

If no Catalog Items have been defined, the Service can be selected and the current progressive capture will continue to run
If one or more Catalog Items have been defined, either the Service can be selected to continue with the current progressive capture or one of the individual Catalog Items can be selected which will run a new progressive capture that is specific to that item.
Portal Only Catalog Items
The creation of a Progressive Capture Script that is only going to be available to users of the portals is as straight forward as going to Administration and creating collection of forms and questions that the user will be stepped through to raise the appropriate request.

When building a Progressive Capture Script for this purpose there is only one thing to keep in mind. There are particular progressive capture forms that are not designed for use by portal users. If these forms are added to these progressive capture scripts they will simply be skipped and not visible to the user on the portals. These include the following forms:

Customer Search
Co-worker Search
Contact Search
Service Details
Request Type
Customer Request Type
Analyst Assignment
Support Staff Only Catalog Items
When a support person begins the steps of raising a request, they will start by clicking on the Raise New option or select a particular type of request, such as an Incident, or Service Request. Each of these will run its own Progressive Capture Script. Within any of these Progressive Capture Scripts the Service Details form may be included. It is this Service Details form that displays the list of available Catalog Items for each Service. If one of these Catalog Items is selected, a new Progressive Capture Script will be launched.

It is possible that some of the information collected in the initial Progressive Capture Script will be relevant to the Catalog Item specific Progressive Capture Script. In order to maintain this information between the two Progressive Capture Scripts, the same Progressive Capture forms must be included in both Scripts. For example if you use the Customer Search form in the initial Progressive Capture, and you want retain the selected customer in the next script, the next script must also include the Customer Search form. If information collected in the initial script is no longer relevant to the Catalog Item, simple leave that form out of the Catalog Item script.

Shared Catalog Items
In some cases you may be able to use the same Catalog Item in both the Portal and the for the Support Staff. Using the considerations mentioned in the previous two sections, you can build a progressive capture script that lets you include Support specific forms which are skipped and not visible in the portals, but they can be added to retain information that the support person needs.

Language
If you are working in a multilingual environment you can publish each Catalog Item in a number of different languages. Any user that has a matching language set against their profile will see this Catalog in their preferred language.

Add a Translation
The Language option provides a list of all of the different languages that this Catalog Item has been translated into. A newly created Catalog Item will only show the language that was selected at the time of creation. To add a new translation click on the Add Translation button which will expose the options for publishing this in another language

Language - Select the new language that you wish to add
Translate - Clicking this button will take the original title and description from the default language and automatically translate these fields using Google Translate. The Title and Description fields will be automatically populated with this translation. These fields can also be manually edited to either add your own translation or used to correct any mistakes made by the automatic translation
Information Clicking on the Translate button will overwrite any information that is already held in the Title and Description fields.
Update a Translation
Delete Translation - Clicking on this button will delete the language translation that is currently selected in the Language pick list.
Information The default language translation cannot be deleted, therefore this button in not available when the default language is selected. The default language is a fallback and is displayed to a user who is using a language that does not have an associated translation available.
Update - If a manual change has been made to either the Title or Description fields, to save these changes by clicking on the Update button
Preview Google Translate - This is a sub-action of the Update button which is accessed by clicking on the arrow next to Update. This will translate the Title and Description fields using the default translation without saving it. This Preview can then be saved using the main Update button.
Update with Google Translate - This is a sub-action of the Update button which is accessed by clicking on the arrow next to Update. This will automatically translate and save the Title and Description fields.