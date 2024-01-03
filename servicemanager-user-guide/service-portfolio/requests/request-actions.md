# Request Actions
The action bar located at the top of each request contains the majority of actions that you can apply to a request. 

![Request Actions](_books/servicemanager-user-guide/service-portfolio/requests/images/action-bar.png)

* The actions available on a request can be configured within the service they are associated with.
* The supporting workflow that sits behind the request can control the focus of an action when that action is required to be completed.
* Use the workflows to lock or unlock individual actions at any stage in a supporting workflow.
* Global Request Settings control which of these options are enabled when an Incident is on hold.

## Update
----
The update action is used for posting information into the timeline which can be used for collaborating with your team members.

### Links and Embedded Content
The update supports text, images, and embedded multimedia / hyperlinks. Simply cut and paste the content, or link you wish to share in the update box. Examples include:
* Sharing a youtube video, which can be viewed in the update from the timeline of the request.
* Links (URL) to another request, workspace post, or document in Hornbill.

### Wiki Mark-Up
For easy formatting of update content, a sub-set of Wiki Markup can be used for decorating text, with italics and bold, creating bulleted or numbered lists etc. Use Ctrl+I or Ctrl+B keyboard short cuts to enable/disable italic and bold text as you type.

### Mentions
It is possible to @mention a co-worker in an update. The mentioned co-worker will receive a Hornbill notification that includes a link to the request.
<!--https://wiki.hornbill.com/index.php?title=Update_Action_Item -->
## Phone Call
----
Capture information taken from a phone call with a customer. If there is no answer, schedule a call back.

### Customer Information
By default when you view the Phone Call Action it will show the name of the customer associated to the request and their phone number. This provides you with quick access to phone them without having to look up their details.
* Use the `Search` option to look up other user's contact details.
* Initiate a phone call using a linked app by clicking on the customer's phone number.

### Conversation Notes
Use this to capture information about the phone call. These are added to timeline under the category of **Phone** and will reference the call as being incoming or outgoing depending on the option chosen.

### Schedule a Call Back
Built into this action item is a Call Back feature that lets you schedule an activity to phone the customer back at another time. This Call Back is added into the activities section of the request and onto your personal Activities View
<!--https://wiki.hornbill.com/index.php?title=Phone_Call_Action_Item -->

## Attachment
----
One or multiple attachments can be added to a request through either dragging and dropping the files into the file box, or using the Select Files option to browse to find and then select the files you wish to attach.

### Comments and Descriptions
Once your files have been added to the attach action, you can provide an optional Comment which will be visible on the timeline of the request, which can be used to help explain why the attachments have been added. You also have the option to add a short Description to each of the files you are adding which may help describe each individual file.

### Visibility and Uploading
Once you selected your files and added any supporting comments and descriptions, you can choose the visibility level of the attachments. If this is left as the default Customer, this will allow the customer to view the attachments on the request via their customer or employee portal. If the setting is changed to say team, or owner then the customer will not see these attachments when viewing the request.

### System Settings
Restrictions can be applied to both the type of files which you want to allow to be uploaded, and the maximum size of any individual attachments which are being added. These can be managed by your administrator through configuration.
|Name|Description|Default Setting
|-|-|-|
|communications.maxfileUploadSize|Sets the maximum size (in bytes) of a file upload|1000000
|security.fileUploadRestriction.webdav.types|This is a semicolon(;) separated list of the restricted file extensions (without the dots(.)) for file upload|exe;bat;cmd;js;vbs|
<!-- https://wiki.hornbill.com/index.php?title=Attachment_Action_Item -->
<!--
## Link
Link this request to other requests
----
## Linked Services
Link other related Services to the request
## Authorisers
Add Authorisers to a Request
## Email
Send an email directly from the request
## Customer
Change the customer that is associated to this request
## Assign
Reassign the request to another team or user
## Connections
Add other users that might have an interested in this request and keep them updated by email
## Escalate
Reset the Priority for this request
## Category
Set the Request Category
## Assets
Associate One or more assets to this request
## Boards
See what Boards this request is on or add it to a Board
## Solutions
If linked to a Problem Record this will present possible solutions
## Resolve and Close
Capture resolution details
## Cancel
Raised by mistake? Use this option to cancel a request
## Print
Select and Print details of the request -->