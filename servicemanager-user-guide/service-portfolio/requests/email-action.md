# Email Action
The Email Action within a request enables the sending of emails directly from the request to any recipient that you wish to communicate with regarding that particular request. Email communication sent from a request is captured in the Timeline to help track and view all outbound emails sent about that request.

![Request Email Action](/_books/servicemanager-user-guide/images/request-email-action.png)

## Before you begin

* **Has a shared mailbox been set up**? Emails sent from a request use a [Shared Mailbox](/esp-config/email/shared-mailboxes) rather than an individual user's mailbox. This ensures a single point of email communication from the Service Desk.
* **Do you have rights to a shared mailbox**? To use a shared mailbox, each user must be assigned [a role that provides access to a shared mailbox](/esp-config/email/shared-mailboxes#associated-roles).
* **Who is the email sent from**? Emails sent from a request use the [default email address](/esp-config/email/shared-mailboxes#addresses) set on a shared mailbox as the sender.  

    :::tip
    If the user sending the email from the request has access to more than one shared mailbox, a drop-down list will be available for them to manually change which mailbox the email will be sent from.
    :::

## Recipients
The recipients of an email can include [Hornbill users](/esp-user-guide/co-workers) and Hornbill contacts, or if the recipient does not exist within Hornbill, you can simply type their email address.
* **To**<br>Add one or more recipients who will receive the email. The customer of the request is automatically added as a recipient as they are seen as the most common recipient, however, there is no restriction on who the email is sent to.
* **CC/BCC**<br>Clicking on the CC/BCC option, these two fields will be exposed to allow additional recipients to be added as either a carbon copy or as a blind carbon copy.
* **Connections**<br>For ease of communication with people who are connected to a request, you can quickly include connections as recipients of your email.

## Attachments
For any outgoing email, a user can include attachments as part of the email. By Clicking on the Paper Clip button the file upload is displayed.
* **File Upload**<br>Click on the File Upload button to browse your local file system or you can drag and drop a file into the designated area. The attached files are displayed and each file can be removed if it was added in error.
* **Associated Files**<br>You can include files that are already attached to the request. After selecting the paper clip button, if there are existing files already associated with the request, an option titled Show Associated files is displayed. Clicking on this link will show a list of the attachments associated with the request. You can select one or more of these attachments to include with your email.

## Email body
Depending on the settings configured in Service Manager there are two options for the editor that is used when writing the main body of the email. 

### Message Text
The Message Text is a simple text editor that doesn't include any formatting options. The text that is typed by the user gets inserted into an email template when the email is sent. This can assure that the email formats and content are consistant. There are no options to view the email template or select an alternative email template.
* Simple, quick, and easy to use.
* No concerns about formatting or consistancy.  Just write and send.

### Template Editor
The Template Editor loads the email template into view so the user can see exactly what will be sent to the recipient.  The editor includes a tool bar with a number of formating options. 
* Format the font by applying different font types and colors.
* Include links.
* Add images, either by pasting or providing a URL to an image source.
* Add bullets, numbering, subscript and superscript text.
* Automatically loads the associated email template into view.

## Email Templates
When an email is composed from within a request, a template is used to pre-populate the subject and body of the email. This is a great way to provide a standard format for all of the outgoing emails.
* **Default Template**<br>The default email template used can be based on the request type, and service against which the request has been logged. The selected template name is displayed, and the email template content is made available. If a template is not set against a serivce, the RequestMessage template is used.
* **Variables**<br>A template can contain variables that are automatically populated from information contained within the request. For , an email may start with Dear John where John is the first name of the customer on the request and the variable {{Customer Coworker.H_first_name}} was used. If a variable that is displayed within curly braces is visible as {{variable name}} this means that the variable has failed to populate. If this happens, the text representing the variable can be manually removed or replaced before sending, or the information required can be updated on the request and then the template reloaded into the email action. Alternatively, the template itself needs updating to either remove or change to the correct variable.
* **Selecting a Template**<br>In some cases, the use of multiple templates may be required. The application setting app.email.request.operation.templateSelectable is available which can be enabled to allow a user to select from a list of available templates. This setting is enabled within Administration under Service Manager > Settings. This is a global setting and will apply to all request types and all services, and will return a list of all email templates.

## Snippets
Snippets provide the ability to define common responses that you want to include in outgoing email content. The use of Snippets ensures that the same response does not need to be typed manually each time and ensures a consistent level of response is given by all analysts who use the snippets rather than manually entering responses each time.

* Create and use personal Snippets that only you have access to
* Create and use team Snippets that can be used by all your team members
* Create and use service Snippets that can be used by all teams that support a service

## Settings
These settings provide the default behavior for the Email Action. These settings can be accessed by a Hornbill Administrator in the [Service Manager Application Settings](/servicemanager-config/advanced-tools-and-settings/application-settings).
|Setting|Description|
|-|-|
|app.email.request.operation.composerType|This setting has a choice of Template Editior, Message Text, and Analyst Setting that determines which email editor is used. <br><br>**Template Editor** sets the Email Action to use the Email Template Editor and Preview. <br><br>**Message Text** sets the Email Action to use the basic Text field editor. It is mandatory that the email templates that are used when this setting is selected contain the variable {{message}} is positioned where the text is to be included on the email. <br><br>**Analyst Setting** allows each user to select and switch between both editors. It is mandatory that the email templates that are used when this setting is selected contain the variable {{message}} is positioned where the text is to be included on the email. In the case where the user uses the Template Editor, if the {{message}} variable is included in the template, it will be automatically removed for the user.
|app.email.request.operation.templateEditor|If set to On, it will default to the Email Template Editor, false shows the old message text. This setting is used when the app.email.request.operation.composerType is set to Analyst Setting|
|app.email.request.operation.templateSelectable|When the Email Template Editor is enabled, this setting will allow a user to select from a list of available Email Templates.|
|guest.app.requests.notification.emailMailbox|The default shared mailbox to use when sending emails. This can be superceded by the [default mailbox set on a service](/servicemanager-user-guide/service-portfolio/services/service-details#default-mailbox).|

## Timeline
When an email has been sent, a record of the email is posted to the request timeline. To view the content of the sent email, select View Email from the more menu option on the timeline post.