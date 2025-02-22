# Link request action
The Link Action within a request enables two main functions. Firstly, the searching for and linking of existing requests, and secondly the raising of new linked requests.

![Request Link Action](/_books/servicemanager-user-guide/images/request-link-action.png)

### Linking requests
Use the search bar to find related requests and link them to the request.
* **Filters**<br>Use the supplied filters to narrow the returned results. Options include Status, Type, Customer, Owner, Service.
* **Link**<br>From the Returned Results, use the Link button next to each request, to link it to the request.
    * *Relationships*<br>If Service Manager Relationship Links have been configured, choose from one of the available Link types, to create not only a link but a defined relationship between the requests. If Relationship Links have not been configured, no drop-down will appear, and requests will use the generic Link option.

### Raising linked requests
As well as linking the request to other existing requests, you can use the `Raise New Linked Request` option to create a new request, which will automatically be linked to the request.
* The request types available will depend on your rights to raise the different request types.
* Choosing the Request Type for the linked request will initiate the Intelligent Capture for that request type.
    * The summary and description from the original request will be populated into the Request Details Intelligent Capture form fields if selected in the capture flow.

### Linked requests
As soon as the request is either linked to other existing requests or a new request is created from the request, a new collapsable section will appear on the request view.
* All linked requests will be added to this section.
* Options to unlink or edit the relationship link (If Relationship Links have been configured and used) will be presented.
* The request that is linked will also have a request section created when a link to it is added.

![Linked Requests Section](/_books/servicemanager-user-guide/images/request-link-section.png)

:::tip
After a linked request has been added, an addition option on the [Update Action](/servicemanager-user-guide/service-portfolio/requests/update-action#update-linked-requests) becomes available where you can provide an update to all the linked requests.
:::

<!-- https://wiki.hornbill.com/index.php?title=Link_Action_Item -->