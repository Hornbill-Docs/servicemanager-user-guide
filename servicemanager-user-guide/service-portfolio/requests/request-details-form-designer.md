# Request Details Form Designer

The **Details** section of the requests can be customized using the Request Details Form Designer, allowing you to modify the standard fields and expose custom fields.

![The Request Details Form Designer showing the default Summary field and a custom field called "Custom Text"](/_books/servicemanager-user-guide/images/request-details-form-designer.png)

## Before you begin

To access the form designer, the logged in user needs one of the following roles associated to their account:

* Form Designer
* Admin Role

:::important
Changes made to the request details form will impact all requests of that type (Incident, Problem, Change, Service Request, Release) that come under the same service.
:::

## How to Access the Request Details Form Designer

The request details form designer can be accessed from any request or from the [service configuration form](/servicemanager-user-guide/service-portfolio/request-configuration#view-details-form).

## Tool Bar Options

Across the top of the Editor there are some options to manage your design session.

* **Cancel**: Cancels your current editing and returns you to the previous screen without saving any changes.
* **Revert Back**: Reverts all changes made during the current edit to its previous state, and you remain within the editor.
* **Restore Defaults**: Restores all the fields and settings back to the original or default state that was provided at the time of your Service Manager installation
* **Apply Changes**: Any changes made during your edit will be saved and available for use.
* **+ (Add Custom Fields)**: By clicking on the + button you can add Custom Fields to your form

## Standard Fields

* **Summary**: The Summary field is used as a short description of the request.
* **Description**: The Description provides a long text field for detailing the request
* **Source**: This contains the source of the request. These include Email, Analyst, Posts, and Self Service. These are automatically populated based on how a request is raised.
* **Location**: Used to capture the location at where the request has occurred
* **External Reference**: Record a reference number of an item that is used in another application or tool that relates to this request

## Custom Fields

If you would like to store some information within the Request Details and there is not an existing Default Field available, you can add a Custom Field to the form. This is done by clicking on the + button in the tool bar and choosing the custom field type which you wish to use.

* **Available Fields**: There are 30 available custom fields which you can choose from per request type per service.
  * Fields Custom A-M are of type varchar and limited to 255 characters - any values entered into these fields will be truncated after 255 characters
  * Fields Custom P-T are of type text with no character limit
  * Fields Custom 21-25 are of type datetime
  * Fields Custom 26-30 are of type Integer
  * Fields Custom 31-40 are of type text with no character limit

Once you have used a custom field it will not be visible in the list of available fields.

To repurpose a custom field that has already been used, you will need to remove the custom field from the form and it will then appear again in the list of available fields.

* **Display Label**: Add a Display Label which will be visible to the users when viewing or editing this form.  To add different language translations for the Display Label on custom fields switch the UI into the required language and provide the values for that specific language, this can be repeated for any subsequently required languages.
* **Control Type**: A number of Control Types can be used. These include Single Line Text Field, Multi-line Text Area, Drop Down List Box, Radio Option List, Check List Box, 5 Star Rating, Single Check Box, Date Selector, Date Time Selector

:::tip
The list of available Control Type you can use will depend on the field type of the custom field you have chosen to use.

Information Some Control Types will provide additional Field Properties that will allow the defining of the options that accompany the Control Type.
:::

## Field Properties

Both Default and Custom Fields include a properties option. This is accessed by clicking on the Cog button displayed on each field. The available properties will vary on each field, depending on the type and the information held in that field.

* **Show the field in the form**: This will make this field available when in Edit mode on the form. This can also be enabled/disabled using the Eye icon located on the field.
* **The field value cannot be blank when saving**: Checking this option will make this field mandatory. As long as the field is blank, you will not be able to save any updates to the form.
* **The field cannot be edited**: When a field is contains a value that you don't want changes, use this option to prevent this.
* **Show the field in view mode even if the value is blank**: In order to keep a clean and uncluttered details section, if a field is empty the label is not displayed. Once a field is populated the Label and the content of the field are displayed. If you would like the label to be displayed even when the field is empty, tick this box.
* **Field Label**: This is the label that is displayed on the form. The label can be changed to suite the terminology that you prefer to use. In parentheses the current language code is displayed. You are able to provide a translation for the language that you are currently using in your session.
* **Validate Input with RegEx Expression**: Including a RegEx Expression you can control how the user is to input the information into the field. Use the ? button to open the RegEx Selector to help with building your Expression.
* **Test Regex Expression With Value**: This field lets you take your RegEx Expression for a test run to make sure that it works as expected.
* **Message to display to user when validation fails**: If a user enters a value that does not match the provided RegEx Expression you can present them with a message. This can be used to guide them with the correct format that needs to be used.

:::tip
Some Control Types which are configured with Custom Fields will provide additional Field Properties that will allow the defining of the options that accompany the Control Type.
:::
