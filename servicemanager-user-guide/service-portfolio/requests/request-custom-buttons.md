# Request custom buttons
[Custom Buttons](/esp-config/customize/custom-buttons) provide a way to add your own buttons to a request to perform a particular action or set of actions.   Custom Buttons can be configured to do one of the following:

* Open a URL
* Create a pop-up that contains an embeddable URL.
* Run an Auto Task Process

Custom Buttons can be personalized with descriptions, icons, tooltips, and optionally be set to only show if a set of rules is met.

## Before you begin
* Know how to configure [custom buttons](/esp-config/customize/custom-buttons).

The following roles are needed to create and manage custom buttons. 
* **Form Designer**<br>A user will need this role to be able to configure and manage custom buttons.
* **Business Process Manager**<br>A user will need this role to be able to link an Auto Task Process to a Custom Button

## Using custom buttons
The custom buttons on a request are located on the right side of the request title bar.

![Request custom buttons](/_books/servicemanager-user-guide/images/request-custom-button.png)

The available custom buttons might be displayed as individual buttons, a single drop-down option, or a collection of drop-down options. This display can dynamically change, based on the size of the browser window.

## Adding a custom button
Custom buttons are unique to each request type.  For example, when adding a custom button to an incident record, that custom button will be available to all incident records.

Anyone with the [form designer role](/esp-config/organizational-data/roles#system-roles) will see the cog icon on the right side of the request title bar.

Click on the `Cog` icon to add a new custom button
* **Label**<br>Provide a label for the new custom button.
* **Icon**<br>Optionally choose an icon to represent and sit alongside the custom button label on the entity form.
* **Color**<br>Choose a background color for the custom button.
* **Tooltip**<br>Optionally provide a more detailed explanation of the custom button. This will be displayed when a user hovers over the custom button.

### Show button if...
Rules can be used to determine when the button is visible. When adding a rule, you can select from a variety of fields that are available on the request record. 

Three session variables can be used to control visibility. These are particularly useful when you want a button to only be available to an individual or specific group.
* User
* Role
* Group

When there is more than one rule, all rules must be met for the custom button to be displayed. 

:::tip
* Request status values need to entered in the following format: status.new, status.open, status.status.recolved, status.closed.
:::

### Actions
Each custom button can be configured to be one of the following:

#### Open URL
* Add a URL which you want to launch from the custom button.
* Include variables from the entity in the URL.

When adding the URL, you can construct parts of the URL using information in the request.

![Request Custom Button user a URL](/_books/servicemanager-user-guide/images/request-custom-button-url.png)

### Auto Task
Auto tasks is a very powerful tool that can utilize most of the automation that is available in a regular workflow.

The Business Process Manager role will be needed to be able to link an [Auto Task Process](/servicemanager-config/customize/service-manager-auto-tasks) to a Custom Button.
* Select the Auto Task Process that you wish to be invoked and executed when the custom button is selected.

#### Response
* Display Autotask progress in timeline - tick this option if you want a post to be added to the entity timeline to audit the running of the Auto Task process and its progress and success.
* Open pop-up with Autotask progress - tick this option if you want a pop-up to display when the custom buttons is selected, and to show the user the progress of the executed Auto Task.

## Manage Custom Buttons
* Click on the edit option next to a custom button to edit its attributes.
* Click on the Trash Can icon next to a custom button to delete it.

## Using Custom Buttons
Once a custom button has been configured, users will be able to use the custom button from the entity view it has been configured against. Visibility of the custom button will also depend on any conditions that may have been set when configuring the button.