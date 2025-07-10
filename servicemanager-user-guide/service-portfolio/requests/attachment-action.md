# Attachment Action
One or more attachments can be added to a request through either dragging and dropping the files onto the attachment box or using the `Select Attachment` option to browse the local file systme and then select the files you wish to attach. 

![Attachment Action](/_books/servicemanager-user-guide/service-portfolio/requests/images/attachment-action.png)

### Before you begin
* **Is the attachment action enabled on the service?**  The attachment action can be enabled or disabled for each request type under the [Service Configuration](/servicemanager-user-guide/service-portfolio/request-configuration#request-actions). If you can't see the attachment action, this might be because the service owner has disabled this feature.
* **Do you know the maximum file size that you can attach?**  The default maximum size is 10 MB. This can be increased or decreased by the Hornbill administrator. If you attach a file larger than the maximum size, an error message will be displayed along with the maximum file size that is allowed.

### Add a comment
The **Add a comment** field can be used to provide additional information about the attachments and why they are being added to the request.  The comment will be added to the request's timeline.  

### Select Attachment
There is an option to either browse the local computer or drag and drop one or more files onto the Attachment Action.  

:::tip
When browsing the local computer, multiple files can be added at the same time by holding down the `Shift` key while clicking on each file.
:::

#### Add a description
Once your files have been added to the attachment action, you can provide a short description of each attachment. This can be used to describe the content of each attachment. The description will be visible within the [Attachment section](/servicemanager-user-guide/service-portfolio/requests/attachment-action#attachment-section) of the request.

#### Select visibility
For each attachment, a visibility can be set to either **Customer** or **Team**. When this is set to **Customer** the customer of the request will be able to see and download the attachment when viewing the request in the Employee or Customer Portals. 

### Lock/Unlock
A user who has a [Full Access role](/servicemanager-config/setup/service-manager-roles#system-roles) to the request type can lock this action.  Locking this action will prevent other users from being able to upload an attachment. The locking and unlocking of this action can also be controlled by using [Access Control in a workflow](/servicemanager-config/customize/workflows/service-manager-workflows#access-control).  

### Visibility
Once you have selected your files and added any supporting comments and descriptions, you can choose the visibility level of the attachments. If this is set to Customer, it will allow the customer to view the attachments on the request via the customer or employee portal. If the setting is changed to Team or Owner then the customer will not see these attachments when viewing the request.

## Attachment section
Any attachment that has been added to a request can be accessed from the Attachments section.  The Attachments section is only visible when one or more attachments have been added.

![Attachments Section](/_books/servicemanager-user-guide/service-portfolio/requests/images/attachments-section.png)

### Downloading
By clicking on the name of the attachment, it will be downloaded to your local computer. Browsers generally have settings to control the location and behavior of downloads.
### Image preview
If an attachment is recognized as an image, an image icon appears next to the attachment's name.  Clicking on this icon will display a thumbnail of the image without having to download it. Clicking on the thumbnail will then open a larger preview of the image.  

### Actions
Each attachment has an Actions menu where the following can be done.
* Edit Description.
* Edit Visibility.
* Remove (Permanently delete the attachment).

## System settings
Restrictions can be applied to both the type of files that you want to allow to be uploaded and the maximum size of any individual attachments that are being added. These can be managed by your administrator through configuration.
|Name|Description|Default Setting
|-|-|-|
|communications.maxfileUploadSize|Sets the maximum size (in bytes) of a file upload|10000000
|security.fileUploadRestriction.webdav.types|This is a semicolon(;) separated list of the restricted file extensions (without the dots(.)) for file upload|exe;bat;cmd;js;vbs|

## Application settings
|Name|Description|Default Setting
|-|-|-|
|guest.ui.app.com.hornbill.servicemanager.operation.defaultVisibility.attachFile|Default Timeline visibility value when attaching a file to a request|Customer|