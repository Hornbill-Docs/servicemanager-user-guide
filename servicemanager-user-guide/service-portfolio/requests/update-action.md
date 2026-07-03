# Update Action

Use the Update action to post information to the request timeline. This feature helps you collaborate with team members and customers.

![Update action screenshot](/_books/servicemanager-user-guide/service-portfolio/requests/images/update-action.png)

Administrators can enable or disable this action in the [service configuration](/servicemanager-user-guide/service-portfolio/request-configuration#request-actions).

## Add a comment

You can include text, images, and embedded multimedia or hyperlinks in your updates.

### Links and embedded content

To share content or links, paste them directly into the Update box. Examples of supported content include:

* YouTube videos that users can view directly from the timeline.
* Hyperlinks to other Hornbill requests, workspace posts, or documents.

### Wiki markup

Use wiki markup to format your text. You can apply formatting like italics and bold, or create bulleted and numbered lists.

* Use the **CTRL+B** keyboard shortcut for bold text.
* Use the **CTRL+I** keyboard shortcut for italic text.

Select the **Preview wiki markup** button ![wiki preview button](/_books/servicemanager-user-guide/service-portfolio/requests/images/wiki-preview-button.png) to see how your content will appear before you post it to the timeline.

### Mentions

To notify a coworker about an update, use an @mention. Type the **@** symbol followed by the first few letters of the coworker's name. Select the correct person from the list that appears. The coworker will receive a notification that includes a link to the request.

## HAi Text Assist

![HAi Assist logo](/_books/servicemanager-user-guide/images/hai-logo-22x22.png) [HAi Text Assist](/servicemanager-user-guide/hai/text-assist) is an AI tool that helps you write request updates. Clear and concise updates improve communication with your team and customers. These updates also provide data for request summarization and knowledge article generation.

* **Ask HAi**: Enter an open-ended prompt to find solutions for common issues. For example, type "How to set up an email signature in Outlook in Office 365."
* **Change Tone**: Adjust the tone of your text to suit your audience. Options include Apologetic, Professional, Friendly, and Technical.
* **Improve Text**: Correct spelling and grammar mistakes to improve readability.
* **Shorten Text**: Remove unnecessary words from your update.
* **Listify**: Convert blocks of text into a list format.

## Customer email notifications

Email notifications can be automatically sent to customers when you add an update with the visibility level set to *Customer*. These emails include links to the original request so the customer can read and respond. Any subsequent comments on a customer-visible update also trigger a notification.

To ensure customers receive these emails, verify the following configurations:

* **Default Email Template**: Use the provided **CustomerTimelineUpdateNotification** template or a custom version.
* **Email Template Setting**: If you use a custom template, update the **guest.app.requests.notification.emailTemplate.customerTimelineUpdate** system setting with the new template name.
* **Email Notification Setting**: Change the **guest.app.requests.notification.emailMailbox** setting to the name of the mailbox you want to use for Service Manager notifications. This defaults to "helpdesk" upon installation.
* **Notify Customer**: Enable the **Notify Customer** option in the Request Action configuration.

## Update linked requests

If a request has linked records, you can send updates to the timelines of those linked requests simultaneously.

### Settings

This feature is disabled by default. You can enable it in the [Service Manager Application Settings](/servicemanager-config/advanced-tools-and-settings/application-settings) by changing the following system setting:

* **app.request.update.enableLinkedRequestAction**: Set this to enabled to allow updates to linked requests from the Update tab.

### Usage

When linked requests exist, the **Update** button includes an arrow. Select **Update this and linked requests...** to open a dialog box.

* **Select All**: Select or deselect all requests in the list.
* **Check boxes**: Select specific requests to include in the update.
* **Request Type Filter**: Filter the list to show only specific request types.
* **Update**: Apply the text to all selected requests.

:::tip
Updates to linked requests are one-way. If a user comments on the update within a linked request, that comment does not appear in the original request.
:::
