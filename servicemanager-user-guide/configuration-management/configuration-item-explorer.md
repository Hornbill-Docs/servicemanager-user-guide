# Configuration Item Explorer
The Configuration Item Explorer provides a graphical representation of associated or linked CIs. The Explorer can be launched from within Configuration Management, or from other views where the Configuration Management plug-in is available. Typically, this would be from CI views such as:
* Service records
* Request records
* Asset records

The Explorer can be used to view and define relationships between CIs.

## Features
When you open the Explorer view, its root defaults to the CI from which it was launched.

## Explorer View
If the CI has existing defined relationships to other CIs , then the first level of these relationships will be visible.

* If further levels exist, click the + icon of a CI in the Explorer to get to the next level.
* To hide or contract an Explorer level, click the - icon of a CI.
* By default, the Explorer is set to expand to a maximum of three levels, but admins can configure this in Configuration Manager > Applications Settings using the `app.cm.explorer.diagram.level.max` system setting.

### In Policy
Each CI is either marked as being In Policy or not, denoted in the Explorer by a tick or cross icon.

You can move CIs in or out of policy by clicking on the icon and switching it from a tick to a cross or vice versa. Some CIs can't be marked as in or out of policy (e.g. users).

### Viewing Relationship Links
Inherited relationships between CIs are shown in the Explorer. Examples include the following:
* Assets linked to other assets or services in Service Manager
Assets linked to a request
Requests that have an owner
Attachments linked to an asset

If no dependency relationships exist between two CIs, then the link will say Not Set.

If an existing dependency and relationship exists between two CIs, then the link will show the dependency relationship and the color will indicate the impact level. You can click a link to view and edit the dependency and impact.

## Explorer View Filters
The CIs displayed in the Explorer can be filtered on various criteria, as follows:

### In Policy
Show all CIs, only those marked as In Policy, or those out of policy.

### Impact Relationship Visibility
Filter the displayed CIs by level of impact. By default, all are visible, but you can filter this to show only CIs for which the relationships are marked as High, Medium, or Low Impact.

### CI Visibility
Choose which CI types are displayed in the Explorer CI Types list by enabling or disabling the types from the menu control.

By default, all CI types are displayed. The Configuration Item types are:
* Assets
* Requests
* Attachments
* Users
* Services

### Set Current Configuration Item Node as Root
Having clicked on and viewed the details of a CI, click the CI Root icon from the menu to set that current node as root in the Explorer. This resets the Explorer view using this CI as the root. This option is not enabled if the CI in focus is the current root in the Explorer.

### Show Legend
Use the CI Legend icon to open the Explorer legend. The content of the Explorer can be explained as follows:

* **Red background.** An entity has high impact on the other.
* **Orange background.** An entity has medium impact on the other.
* **Green background.** An entity has low impact on the other.
* **Dark border.** The selected item.
* **Green tick.** An item in policy.
* **Red cross.** An item not in policy.

### Details
Click the name of a CI in the Explorer to see its information displayed in the Details section of the Explorer.

Select the title of the CI from the Details section to open the CI in a new tab.

To create more space, hide the Details section in the Explorer by clicking the **Hide Details** action item.

If the Details section is hidden, click **Show Details** to show it again in the Explorer.

## Defining Dependency and Impact Relationships
### Relationship Definitions
Define bi-directional relationships between CIs by setting the dependency type and level of impact. Select from the defined dependency types and impact levels.
* **Dependency on the Parent**<br>Click on the Explorer and the arrow facing the parent CI, then choose the relevant dependency from the dropdown and the impact level, then click **Save** to create the relationship.
* **Dependency from the Parent**<br>Click on the Explorer and the arrow facing away from the parent CI, then choose the relevant dependency from the dropdown and the impact level, then click **Save** to create the relationship.

Edit or remove the relationships by clicking on either relationship link and changing the dependency or impact. Click **Save** to apply the change.

The available relationship types can be set differently depending on the direction of the relationships, and be different depending on the type of CIs being connected.

Admins can configure these options in Configuration using the `app.cm.explorer.items.dependencies` system setting.