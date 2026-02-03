# Attachment action

Add one or more attachments to a request by dragging files onto the attachment box or by selecting **Select Attachment** to browse your computer.

![Attachment Action](/_books/servicemanager-user-guide/service-portfolio/requests/images/attachment-action.png)

## Before you begin

- **Is the attachment action enabled on the service?** The attachment action is enabled or disabled per request type under [Service Configuration](/servicemanager-user-guide/service-portfolio/request-configuration#request-actions). If you don't see the attachment action, the service owner may have disabled it.
- **What is the maximum file size?** The default maximum file size is 10 MB. An administrator can change this. If you upload a file that exceeds the limit, an error shows the allowed size.

## Add a comment

Use the **Add a comment** field to explain the attachment or why you added it. The comment appears in the request timeline.

## Select attachment

You can browse your computer or drag and drop one or more files onto the attachment area.

:::tip
Hold Shift while selecting files to add multiple items at once.
:::

### Add a description

After you add files, enter a short description for each attachment. The description appears in the [Attachments section](/servicemanager-user-guide/service-portfolio/requests/attachment-action#attachment-section) of the request.

### Select visibility

For each attachment, set visibility to **Customer** or **Team**. When visibility is **Customer**, the customer can view and download the attachment in the Employee or Customer portals. When visibility is **Team** or **Owner**, the customer cannot see the attachment.

## Lock and unlock

Users with a [Full Access role](/servicemanager-config/setup/service-manager-roles#system-roles) for the request type can lock this action. Locking prevents other users from uploading attachments. You can also control locking through [Access Control in a workflow](/servicemanager-config/customize/workflows/service-manager-workflows#access-control).

## Attachment section

Open the Attachments section to access attachments added to the request. The section is visible only when one or more attachments exist.

![Attachments Section](/_books/servicemanager-user-guide/service-portfolio/requests/images/attachments-section.png)

### Downloading

Click an attachment name to download it. Browser settings control download location and behavior.

### Image preview

If the attachment is an image, an image icon appears next to its name. Click the icon to open a thumbnail, and click the thumbnail for a larger preview.

### Actions

Use the Actions menu for each attachment to:

- Edit description
- Edit visibility
- Remove (permanently delete)

## System settings

Administrators can restrict allowed file types and set the maximum upload size.

|Name|Description|Default setting|
|-|-|-|
|communications.maxfileUploadSize|Maximum size (in bytes) for a file upload|10000000|
|security.fileUploadRestriction.webdav.types|Semicolon-separated list of restricted file extensions (no leading dots)|exe;bat;cmd;js;vbs|

## Application settings

|Name|Description|Default setting|
|-|-|-|
|guest.ui.app.com.hornbill.servicemanager.operation.defaultVisibility.attachFile|Default timeline visibility when attaching a file to a request|Customer|
