# Request Timeline
The Timeline is an interactive timeline of events and discussions about the request.

## Email Posts
Email posts are created when an email is sent from a request using the [Email Action](/servicemanager-user-guide/service-portfolio/requests/email-action) or if the request has been automatically updated from an [incoming email](/esp-config/email/using-email-routing-rules).  

#### Email options
When viewing an email-related post in the timeline, additional options are available via the ellipses (⋯) icon that allow you to view or reply to the email.

![Request timeline email options](/_books/servicemanager-user-guide/images/request-timeline-email-options.png)

* **View**. Opens a pop-up from the request displaying the full email, including images and formatting. Reply, Reply All, and Forward options are also available.
* **Go To**. Opens the associated email directly in its mailbox in a new browser tab. This option loses the context of the request, and therefore, some of the features mentioned below are not available.
* **Reply**. Opens a pop-up from the request in Reply mode, with the original sender pre-populated in the `To` field.
* **Reply All**. Opens a pop-up from the request in Reply All mode, with the following:
    * The original sender is pre-populated in the To field
    * Any additional recipients from the original email are included in the appropriate `To` or `Cc` fields
* **Reply to Contacts**. Opens a pop-up from the request in Compose mode, with the `To`, `Cc`, and `Bcc` fields populated using the contacts listed in the [Email Contacts](/servicemanager-user-guide/service-portfolio/requests/request-email-contacts).

#### Timeline updates
When an email is sent using View, Reply, Reply All, and Reply to Contacts, the sent email is automatically added as a new post in the timeline of the request.

#### Request ID handling
When an email is sent using View, Reply, Reply All, and Reply to Contacts, and the subject line does not already contain the request ID, the request ID will be automatically appended to the end of the subject line.

This ensures:
* Subsequent replies can be correctly associated with the request.
* [Inbound Routing Rules](/esp-config/email/using-email-routing-rules) can process the incoming email responses accurately.

#### Including the email trail
A setting is available to allow the original message text (including the email trail) to be included automatically in replies that are sent using the View, Reply, Reply All, and Reply to Contacts options.

##### Enabling the setting
1. Navigate to [Platform Configuration → Core Settings](/esp-config/advanced-tools-and-settings/core-settings).
1. Search for: `app.view.email.reply.includeOriginalMessageText`.
1. Set the value to `ON`

#### Deleted emails
The email-related timeline actions rely on the original email still existing within a [folder of a mailbox](/esp-user-guide/email-folders). If the email has been permanently deleted:
* The ellipses menu options will still be visible.
* The email can no longer be opened, as it no longer exists in the mailbox. When trying to access a deleted email, a warning message will be displayed to inform the user that it can no longer be accessed.
