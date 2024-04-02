# Custom Buttons
Custom Buttons provide a way to add your own buttons to a request to perform a particular action or set of actions.   can be added to requests and configured to allow one of three options

* Open a URL
* Create a popup contains an embeddable URL.
* Run an Auto Task Process

Custom Buttons can be personalized with descriptions, icons, tooltips, and optionally be set to only display on views if configurable conditions are met.

## Before you begin
The following roles are need to create and manage custom buttons. 
* **Form Designer**<br>A user will need this role to be able to configure and manage custom buttons.
* **Business Process Manager**<br>A user will need this role to be able to link an Auto Task Process to a Custom Button

## Configuring Custom Buttons

### Creating a Custom Button
Click on the `Cog` icon to add a new custom button
* **Label**<br>Provide a label for the new custom button.
* **Icon**<br>Optionally choose an icon to represent and sit alongside the custom button label on the entity form.
* **Color**<br>Choose a background color for the custom button.
* **Tooltip**<br>Optionally provide a more detailed explanation for the purpose of the custom button. This will be displayed when a user hovers over the custom button.

### Conditions
By default a custom button will appear on all requests of the same type. Conditions can be used to determine when the button is visisble. 
* The available conditions will be relevant to the request type which you are adding the custom button.
* Having multiple conditions will be treated as AND conditions, so all conditions will need to be met for the custom button to be displayed.

:::tip
* Request status values need to entered in the following format: status.new, status.open, status.status.recolved, status.closed.
* Request type values need to be entered in lower case.
:::

### Actions
Each custom button can be configured to be one of the following:

* Open URL.
* Open a popup that contains an embeddable URL.
* Run an Auto Task process.

#### Open URL
* Add a URL which you wish to launch from the custom button.
* Include variables from the entity in the URL.

### Auto Task
The Business Process Manager role will be needed to be able to link an Auto Task Process to a Custom Button.
* Select the Auto Task Process which you wish to be invoked and executed when the custom button is selected

#### Response
* Display Autotask progress in timeline - tick this option if you want a post to be added to the entity timeline to audit the running of the Auto Task process and it's progress and success
* Open popup with Autotask progress - tick this option if you want a pop up to display when the custom buttons is selected, and to show the user the progress of the executed Auto Task process

## Manage Custom Buttons
* Click on the edit option next to a custom button in order to edit it's attributes
* Click on the Trash Can icon next to a custom button in order to delete it

## Using Custom Buttons
Once a custom button has been configured, users will be able to use the custom button from the entity view it has been configured against. Visibility of the custom button will also depend on any conditions which may have been set when configuring the button.