# Configuration Item Explorer
The Configuration Item Explorer provides a graphical representation of associated or linked CIs. The explorer can be launched from within the Configuration Manager app, or from other views where the Configuration App plug in is available. Typically this would be from Configuration Item views such as:
* Service records
* Request records
* Asset records

The Explorer can be used to view and define relationships between Configuration Items.

## Features
When opening the Explorer view, it's root will default to the Configuration item which it was launched from.

## Explorer View
If the Configuration item has existing defined relationships to other Configuration Items , then the first level of these relationships will be visible.

* If further levels exists, click on the + icon of a Configuration Item in the explorer the next level
* To hide or contract an explorer level, click on the - icon of a Configuration Item
* By Default the explorer is set to expand to a maximum of 3 levels, but this can be configured in the admin tool under Home > Configuration Manager > Applications Settings and the app.cm.explorer.diagram.level.max system setting

### In Policy
Each Configuration Item will either be flagged as being In Policy or not, denoted on the explorer by a Tick or Cross icon.

Configuration Items can be moved in or out of Policy by clicking on the icon and switching it from a Tick or a Cross
Configuration Items which do not have a Tick or Cross can't be marked as in or out of Policy, typically this will be Users etc

### Viewing Relationship Links
Inherited relationships between Configuration Items will be shown in the explorer. These could be based on Assets being linked to other Assets or Services in Service Manager, or where Assets have been linked to a Request, or where a Request has an Owner, or a document has been linked to an Asset.

If no Dependency Relationships exist between two Configuration Items then the link with say Not Set
If an existing Dependency and Impact Relationship exists between two Configuration Items then the link will show the Dependency relationship and the color will indicate the impact level
Clicking on a link will allow the Dependency and Impact to be viewed and edited.

## Explorer View Filters
The displayed Configuration items in the explorer can be filtered on various criteria, this is detailed below.

### In Policy
Show all Configuration Items, just those marked as in policy, or those out of Policy

### Impact Relationship Visibility
Filter the displayed Configuration Items by level of impact. By default All will be visible, but filter this to only show Configuration Items where the Relationships are marked as High, Medium or Low Impact

### CI Visibility
Choose which Configuration Item Types are displayed on the Explorer CI Types list.png by enabling or disabling the Types from the menu control.

By Default all Configuration Types will be displayed
Configuration Item Types are:
* Assets
* Requests
* Documents
* Users
* Services

### Set Current Configuration Item Node as Root
Having clicked on and viewed the Details of a Configuration Item, use the CI Root.png icon from the menu to set that Current Node as Root in the Explorer

This will reset the explorer view using this Configuration Item as the Root.
This option will not be enabled if the Configuration Item in focus is the current Root on the Explorer

### Show Legend
Use the CI Legend.png icon to open the Explorer Legend and for an explanation of the Explorer content

* red background - an entity has high impact on the other
* orange background - an entity has medium impact on the other
* green background - an entity has low impact on the other
* dark border - selected item
* green tick - item in policy
* red cross - item not in policy

### Details
Click on the name of a Configuration Item in the explorer to see it's information displayed in the Details section on the explorer.

Select the Title of the Configuration Item from the Details section to open the Configuration Item in a new tab
Hide the Details section on the explorer view to create more space by selecting the Hide details action item.
If the Details section is hidden select Show Details to show it again on the explorer

## Defining Dependency and Impact Relationships
### Relationship Definitions
Define bi-directional relationships between Configuration Items by setting the Dependency type and level of impact by selecting form the defined dependency types and impact levels.
* **Dependency on the Parent**<br>Click on the Explorer and the arrow facing the Parent Configuration Item, choose the relevant Dependency from the drop down and the Impact level and select Save to create the relationship
* **Dependency from the Parent**<br>Click on the Explorer and the arrow facing away from the Parent Configuration Item, choose the relevant Dependency from the drop down and the Impact level and select Save to create the relationship

Edit or remove the relationships by clicking on either relationship link and changing the Dependency or Impact and selecting Save to apply the change

The available relationship types can be set differently depending on the direction of the relationships, and be different depending on the type of Configuration Items being connected.

These options can be configured in the admin tool under Home > Configuration Manager > Application Settings and the app.cm.explorer.items.dependencies system setting.