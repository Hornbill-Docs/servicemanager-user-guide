# Update Action
The update action is used for posting information into the timeline which can be used for collaborating with your team members and the customer.

![Update-Action](/_books/servicemanager-user-guide/service-portfolio/requests/images/update-action.png)

This action can be enabled or disabled from within the [Service Configuration](/servicemanager-user-guide/service-portfolio/request-configuration#request-actions)

## Links and Embedded Content
The update supports text, images, and embedded multimedia/hyperlinks. Simply cut and paste the content, or link you wish to share in the update box. Examples include:
* Sharing a youtube video, which can be viewed in the update from the timeline of the request.
* Links (URL) to another request, workspace post, or document in Hornbill.

## Wiki Mark-Up
For easy formatting of content, a sub-set of Wiki Markup can be used for decorating text, with italics and bold, creating bulleted or numbered lists etc. Use Ctrl+I or Ctrl+B keyboard shortcuts to enable/disable italic and bold text as you type.

## Mentions
It is possible to @mention a co-worker in an update. The mentioned co-worker will receive a Hornbill notification that includes a link to the request.

## Customer Email Notifications
Email notifications can be sent to the customer of the request each time an Update is added with the visibility level of Customer. These emails can contain links back to originating request to allow the customer to read and respond to the updates. Subsequent comments that are made below a customer visible update will also provide an email notification to the customer This is a great way to keep the customer up to date.

:::note
It is important that the following has been set up in order for the customer to receive the updates by email.
* **Service Mailbox**<br>Set a default mailbox on the service and/or on the Request Types for the service
* **Shared Mailbox Access**<br>Make sure that all the analysts that will be updating the request have access to the mailbox set on the service.
* **Default Email Template**<br>A default Email Template called CustomerTimelineUpdateNotification has been provide for you. Emails sent to customers will be based on this template. You can modify this email template to suite your needs.
* **Email Template Setting**<br>If you want to create a new email template for this purpose, update the system setting guest.app.requests.notification.emailTemplate.customerTimelineUpdate with the name of the new email template.
* **Email Notification Setting**<br>This setting guest.app.requests.notification.emailMailbox defaults to helpdesk on installation. This needs to be changed to the name of the mailbox that you wish to use for notifications from Service Manager.
* **Notify Customer**
Enable the Notify Customer option on the Request Action configuration.
:::

## Update Linked Requests
If there are linked requests associated to the request that you are working on, you are able to send an update to the Timeline of these linked requests

### Setting
This feature is turned off by default and can be enabled in Service Manager Application Settings.
* **app.request.update.enableLinkedRequestAction**<br>Enable the option to update linked requests against a request through the Update tab.

### Using
If there are requests linked to the request you are working on, the Update button within the Update Action will include an arrow that exposes the option to update the linked requests. Selecting the option to Update this and linked requests... will display a dialog box that lists the linked requests.

* **Select All**<br>Use this to select or deselect all of the requests in the list
* **Check Boxes**<br>Use the individual check boxes to select individual requests to include in the update
* **Request Type Filter**<br>Filter the list of linked requests to only show the selected type
* **Update**<br>Click to apply the update text to all of the selected requests
:::tip
Updating linked requests is a one way update. If comments are made on the update in the linked requests, the originating request will not have visibility of these comments.
:::
<!--https://wiki.hornbill.com/index.php?title=Update_Action_Item -->