# Attachment Action
One or more attachments can be added to a request through either dragging and dropping the files onto the attachment box, or using the `Select Attachment` option to browse to find and then select the files you wish to attach.

![Attachment Action](/_books/servicemanager-user-guide/service-portfolio/requests/images/attachment-action.png)

### Comments and Descriptions
Once your files have been added to the attach action, you can provide an optional comment which will be visible on the timeline of the request, which can be used to help explain why the attachments have been added. You also have the option to add a short description to each attachment.

### Lock/Unlock
A user that has a [Full Access role](/servicemanager-config/setup/service-manager-roles#system-roles) to the request type can lock this action.  Locking this action will prevent other users from being able to upload an attachment. The locking and unlocking of this action can also be controlled by using [Access Control in a workflow](/servicemanager-config/customize/workflows/service-manager-workflows#access-control).  

### Visibility
Once you have selected your files and added any supporting comments and descriptions, you can choose the visibility level of the attachments. If this is set to Customer, it will allow the customer to view the attachments on the request via the customer or employee portal. If the setting is changed to Team, or Owner then the customer will not see these attachments when viewing the request.

## Attachment Section
Any attachment that has been added to a request can be accessed from the Attachments section.  The Attachments section is only visible when one or more attachments have been added.

![Attachments Section](/_books/servicemanager-user-guide/service-portfolio/requests/images/attachments-section.png)

### Downloading
By clicking on the name of the attachment, it will be downloaded to your local computer. Browsers generally have settings to control the location and behavior of the downloads.
### Image Preview
If an attachment is recognized as an image, an image icon appears next to the attachment's name.  Clicking on this icon will display a preview of the image without having to download it.
### Actions
Each attachment has an Actions menu where the following can be done
* Edit Description
* Edit Visibility
* Remove (Permanently delete the attachment)

## System Settings
Restrictions can be applied to both the type of files that you want to allow to be uploaded and the maximum size of any individual attachments that are being added. These can be managed by your administrator through configuration.
|Name|Description|Default Setting
|-|-|-|
|communications.maxfileUploadSize|Sets the maximum size (in bytes) of a file upload|1000000
|security.fileUploadRestriction.webdav.types|This is a semicolon(;) separated list of the restricted file extensions (without the dots(.)) for file upload|exe;bat;cmd;js;vbs|
|guest.ui.app.com.hornbill.servicemanager.operation.defaultVisibility.attachFile|Default Timeline visibility value when attaching a file to a request|Customer|
<!-- https://wiki.hornbill.com/index.php?title=Attachment_Action_Item -->
