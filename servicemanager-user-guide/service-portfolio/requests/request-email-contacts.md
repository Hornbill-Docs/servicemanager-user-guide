# Email Contacts
The Email Contacts feature is like an email address book for a request. It contains a list of contacts that can be used with email communications.  This feature is designed to improve speed and consistency when sending emails from a request by ensuring that the relevant recipients are automatically included in communications.

![Email Contacts](/_books/servicemanager-user-guide/images/request-email-contacts.png)

## How Email Contacts work
When a request is either manually or automatically raised from an email, if there are additional recipients in the `To` or `Cc` fields, they are saved to the Email Contacts list. These contacts can then be used in future email communications when using the [Email Action](/servicemanager-user-guide/service-portfolio/requests/email-action) or when replying to an email in the request's timeline.  The contacts will be automatically added to the `To`, `Cc`, or `Bcc` fields of these outgoing emails.

This feature is particularly useful in environments where support teams and end users rely heavily on email communications. 

## Access
* This feature is available to any user who has permission to view and work on a request.
* A user must have access to a [Shared Mailbox](/esp-config/email/shared-mailboxes#associated-roles).

## Adding contacts
Email contacts can be added in the following ways:
1. **When a request is automatically raised from an email**. If [Inbound Routing Rules](/esp-config/email/using-email-routing-rules) are configured to raise a request from an incoming email, any additional recipients included in the To or Cc fields (excluding the shared mailbox address) will be added to the Email Contacts.
2. **When a request is manually raised from an email**. When a user manually raises a request from an email stored in a [mailbox](/esp-user-guide/email-overview), any additional recipients included in the To or Cc fields will be added to the Email Contacts.
3. **Manually adding Email Contacts**. From an existing request, users can add contacts using the plus `+` icon.

## Exluding contacts
Each contact in the list displays an envelope icon that indicates whether they are automatically included or excluded from outgoing emails, based on the color. 
* **Green envelope**. Email contacts showing a green envelope will be included in the relevant `To`, `CC`, or `Bcc` field of the outgoing email.
* **Grey envelope**. Email contacts showing a gray envelop will not be included.

:::note
Inclution is enabled by default when a contact is added.
:::

Clicking on the envelope icon will toggle the setting between being included or excluded.  Any changes to these settings are stored and will apply to future email communications sent from this request.

## Editing or removing email contacts
For each email contact, the following actions are available:

#### Edit
Allows a user to:
* Update the Display Name
* Change whether the contact appears in the To, Cc, or Bcc field of new emails
#### Delete
* Removes the email contact from the request.

## Email-Related Timeline Posts
Email-related timeline posts provide users with quick access to common email actions directly from the request timeline. These actions are available for timeline entries relating to sent or received emails and allow users to view, respond to, or navigate to the original email without leaving the request context.

#### Ellipses Options
When viewing the timeline of a request, additional email-specific actions are available via the ellipses (⋯) icon on timeline posts related to sent or received emails.

The following options are available:
* Email – View - Opens a pop-up from the request displaying the full email, including images and formatting. Reply, Reply All, and Forward options are also available.
* Email – Go To - Opens the associated email directly in its mailbox in a new browser tab.
* Email – Reply - Opens a pop-up from the request in Reply mode, with the original sender pre-populated in the To field.
* Email – Reply All - Opens a pop-up from the request in Reply All mode, with:
    * The original sender is pre-populated in the To field
    * Any additional recipients from the original email are included in the appropriate To or Cc fields
* Email – Reply to Contacts - Opens a pop-up from the request in Compose mode, with the To and Cc fields populated using the contacts listed in the Email Contacts section of the request.

#### Timeline Updates
When an email is sent using any of the following options, the sent email is automatically added as a new post in the timeline of the originating request:
* Email – View
* Email – Reply
* Email – Reply All
* Email – Reply to Contacts

#### Call Reference Handling
If an email is sent using any of the options listed above and the subject line does not already contain the request’s Call Reference, the Call Reference will be automatically appended to the end of the subject line.
This ensures:
* Subsequent replies can be correctly associated with the request
* Auto-Responder Rules can process incoming responses accurately

This behavior applies to:
* Email – View
* Email – Reply
* Email – Reply All
* Email – Reply to Contacts

#### Including the Email Trail
A Core Setting is available to allow the original message text (including the email trail) to be included automatically in replies sent using the following options:
* Email – View
* Email – Reply
* Email – Reply All
* Email – Reply to Contacts

##### Enabling the Setting
1. Navigate to Platform Configuration → Core Settings
1. Search for: app.view.email.reply.includeOriginalMessageText
1. Set the value to ON

## Deleted Emails
The email-related timeline actions rely on the original email still existing in the mailbox.
If the email has been permanently deleted (for example, removed from Deleted Items):
* The ellipses menu options will still be visible
* The email can no longer be opened, as it no longer exists in the mailbox
