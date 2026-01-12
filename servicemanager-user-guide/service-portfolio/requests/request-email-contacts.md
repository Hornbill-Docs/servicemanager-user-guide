# Email Contacts
The Email Contacts feature is like an email address book for a request. It contains a list of contacts that can be used with email communications.  This feature is designed to improve speed and consistency when sending emails from a request by ensuring that the relevant contacts are automatically included in communications.

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
* **Green envelope**. Email contacts showing a green envelope will be included in the relevant `To`, `Cc`, or `Bcc` field of the outgoing email.
* **Grey envelope**. Email contacts showing a gray envelope will not be included.

![Excluding Contacts](/_books/servicemanager-user-guide/images/request-contact-exclude.png)

Clicking on the envelope icon will toggle the setting between being included or excluded.  Any changes to these are saved and will still apply when the request is next viewed.

:::note
Inclusion is enabled by default when a contact is added.
:::

## Editing or removing email contacts
For each email contact, the following actions are available:

#### Edit
Allows a user to:
* Update the Display Name.
* Change whether the contact appears in the `To`, `Cc`, or `Bcc` field of new emails.
#### Delete
* Removes the email contact from the request.

