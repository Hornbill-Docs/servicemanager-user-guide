# Request Actions
The action bar located at the top of each request contains the majority of actions that you can apply to a request. 

![Request Actions](_books/servicemanager-user-guide/service-portfolio/requests/images/action-bar.png)

* The actions available on a request can be configured within the service they are associated with.
* The supporting workflow that sits behind the request can control the focus of an action when that action is required to be completed.
* Use the [Access Control automation](/servicemanager-config/customize/workflows/service-manager-workflows#access-control) to lock or unlock individual actions at any point within a workflow.
* [Request Settings](/servicemanager-config/administration/request-settings#on-hold-settings) control which of these options are enabled when an incident is on hold.

## Update
----
The update action is used for posting information into the timeline which can be used for collaborating with your team members.

### Links and Embedded Content
The update supports text, images, and embedded multimedia/hyperlinks. Simply cut and paste the content, or link you wish to share in the update box. Examples include:
* Sharing a youtube video, which can be viewed in the update from the timeline of the request.
* Links (URL) to another request, workspace post, or document in Hornbill.

### Wiki Mark-Up
For easy formatting of content, a sub-set of Wiki Markup can be used for decorating text, with italics and bold, creating bulleted or numbered lists etc. Use Ctrl+I or Ctrl+B keyboard shortcuts to enable/disable italic and bold text as you type.

### Mentions
It is possible to @mention a co-worker in an update. The mentioned co-worker will receive a Hornbill notification that includes a link to the request.
<!--https://wiki.hornbill.com/index.php?title=Update_Action_Item -->
## Phone Call
----
Capture information taken from a phone call with a customer. If there is no answer, schedule a callback.

### Customer Information
By default when you view the Phone Call Action it will show the name of the customer associated with the request and their phone number. This provides you with quick access to phone them without having to look up their details.
* Use the `Search` option to look up other user's contact details.
* Initiate a phone call using a linked app by clicking on the customer's phone number.

### Conversation Notes
Use this to capture information about the phone call. These are added to the timeline under the category of **Phone** and will reference the call as being incoming or outgoing depending on the option chosen.

### Schedule a Callback
Built into this action item is a callback feature that lets you schedule an activity to phone the customer back at another time. This callback is added to the activities section of the request and onto your personal Activities View.
<!--https://wiki.hornbill.com/index.php?title=Phone_Call_Action_Item -->

## Attachment
----
One or multiple attachments can be added to a request through either dragging and dropping the files into the file box, or using the Select Files option to browse to find and then select the files you wish to attach.

### Comments and Descriptions
Once your files have been added to the attach action, you can provide an optional comment which will be visible on the timeline of the request, which can be used to help explain why the attachments have been added. You also have the option to add a short description to each of the files you are adding which may help describe each file.

### Visibility and Uploading
Once you selected your files and added any supporting comments and descriptions, you can choose the visibility level of the attachments. If this is left as the default Customer, this will allow the customer to view the attachments on the request via their customer or employee portal. If the setting is changed to say team, or owner then the customer will not see these attachments when viewing the request.

### System Settings
Restrictions can be applied to both the type of files which you want to allow to be uploaded and the maximum size of any individual attachments which are being added. These can be managed by your administrator through configuration.
|Name|Description|Default Setting
|-|-|-|
|communications.maxfileUploadSize|Sets the maximum size (in bytes) of a file upload|1000000
|security.fileUploadRestriction.webdav.types|This is a semicolon(;) separated list of the restricted file extensions (without the dots(.)) for file upload|exe;bat;cmd;js;vbs|
<!-- https://wiki.hornbill.com/index.php?title=Attachment_Action_Item -->

## Link
----
The Link Action within a request enables two main functions. Firstly, the searching for and linking of existing requests, and secondly the raising of new linked requests.

### Linking Requests
Use the Search bar to find related requests and link them to the request.
* Filters - Use the supplied filters to narrow the returned results, options include Status, Type, Customer, Owner, Service
* **Link** - From the Returned Results, use the Link button next to each request, to link it to the request
    * Relationships - If Service Manager Relationship Links have been configured, choose from one of the available Link types, to create not only a link but a defined relationship between the requests. If Relationship Links have not been configured, no drop-down will appear, and requests will use the generic Link option.

### Raising Linked Requests
As well as linking the request to other existing requests, you can use the Raise New Linked Request option to create a new request, which will automatically be linked to the request.
* The Request Types available will depend on your rights to raise the different request types.
* Choosing the Request Type for the Linked Request, will initiate the Progressive Capture for that Request Type
    * The Summary and Description from the original request will be populated into the Request Details Progressive Capture form fields, if selected in the Progressive Capture flow.

### Linked Requests
As soon as the request is either linked to other existing requests or a new request is created from the request, a new collapsable section will appear on the request view.
* Linked Requests will be displayed.
* Options to Unlink or edit the Relationship Link (If Relationship Links have been configured and used) will be presented.
----
<!--
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