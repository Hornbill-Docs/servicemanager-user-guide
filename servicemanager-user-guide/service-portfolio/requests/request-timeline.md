# Request Timeline
The Timeline is an interactive timeline of events and discussions about the request.

## Email-Related Posts
Email-related timeline posts provide users with quick access to common email actions directly from the request timeline. These actions are available for timeline entries relating to sent or received emails and allow users to view, respond to, or navigate to the original email without leaving the request context.

#### Options
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

#### Deleted Emails
The email-related timeline actions rely on the original email still existing in the mailbox.
If the email has been permanently deleted (for example, removed from Deleted Items):
* The ellipses menu options will still be visible
* The email can no longer be opened, as it no longer exists in the mailbox
