# Questions section

The Questions section contains the questions and the responses to those questions that are asked when a request is being raised.  These questions are defined as part of an **Intelligent Capture**

![Questions section on a request(/_books/servicemanager-user-guide/images/request-questions-section.png)]

The questions can be used to capture additional information about the request that may be required to fulfill the request, or to route the request to the appropriate team for fulfillment.

You can delete a question from the questions section of a request in Hornbill Service Manager, but doing so requires specific user roles or the use of automated workflows.

## Manual Deletion

To manually remove questions, a user must be assigned a specific application role that grants this permission. This is typically restricted to help remove sensitive information or correct errors.

Required Role: You must have a role that specifically includes the right to "delete questions from a Request".
Standard User Limitations: Regular users or those with standard "Service Request User" roles generally cannot delete these questions to ensure the integrity of the audit trail.

Automated Deletion (BPM)
You can also automate the removal of questions using the Business Process Tool.

Automation Node: Use the "Delete Questions" task within a Hornbill Automation Node in your workflow.
Common Use Cases:
Security/Governance: Automatically clearing sensitive data once it is no longer needed.
Service Re-allocation: Removing questions that are no longer applicable if a request is moved to a different service.
