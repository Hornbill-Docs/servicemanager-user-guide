# Request details

The **Details** section provides an overview of the request, including the summary and a description of the request. This section also includes the source of the request and an external reference field for tracking purposes. You can also add custom fields to capture additional information specific to your organization's needs.

![Request details section showing the summary and description fields](/_books/servicemanager-user-guide/images/request-details-section.png)

## Standard fields

- **Summary**: The summary provides a brief overview of the request, highlighting the key points and objectives of the request. The summary should be clear and specific to ensure that stakeholders can quickly grasp the essence of the request without needing to read through the entire description. This is a mandatory field that must be filled out when creating a request.

- **Description**: The description provides a more detailed explanation of the request, including the background, rationale, and any relevant information that stakeholders need to know. It should be comprehensive and well-structured, allowing stakeholders to fully understand the context and implications of the request.

- **Source**: The source section identifies the origin of the request, such as Self Service using one of the portals, email, or by another system. This is a read-only field that is automatically populated based on how the request was created.

- **External Reference**: The external reference section provides an option to store an ID that is external to the this request. This is useful for tracking the request in other systems or for referencing related information that is not stored within the request itself.

## Custom fields

In addition to the default fields, you can also add custom fields to the request details section using the [Form Designer](/servicemanager-user-guide/service-portfolio/requests/request-details-form-designer). Custom fields allow you to capture additional information that is specific to your organization's needs. You can create custom fields for various types of data, such as text, numbers, dates, or dropdown selections. This flexibility enables you to tailor the request details to better suit your processes and requirements.

## Saving Changes

When you make changes to the request details, it is important to save your changes to ensure that they are not lost. To save your changes, click on the "Save" button located at the bottom of the request details section. This will update the request with the new information you have entered.

### Timeline

Each time the updated details of a request are saved, a timeline post is automatically created. Each entry in the timeline includes a timestamp and a description of the action taken. This allows you to track the history of changes made to the request over time, providing a clear record of how the request has evolved.

### View changes to the details

The **View Changes** feature allows you to see exactly what was modified when request details are updated. Whenever a user manually updates the request details in the UI, the system automatically creates a timeline post with a **View Changes** option.

![Request timeline showing a post with the View Changes button highlighted](/_books/servicemanager-user-guide/images/request-timeline-view-changes.png)

When you open **View Changes**, you'll see:

- The total number of fields that were changed.
- The name of the person who updated the request.
- The date and time the update was made.
- The fields that were changed.

![The View Changes window showing the summary, user name, and timestamp](/_books/servicemanager-user-guide/images/request-details-view-changes-summary.png)

#### Side-by-side view

This is the default view. it displays the old and new values next to each other:

- **Was**: The original value before the update (highlighted in red).
- **Now**: The new value after the update (highlighted in green).

#### Diff view

This view shows an inline comparison. It highlights the specific characters or words added or removed. This is helpful for reviewing small changes within long blocks of text.

### Redact sensitive data

If sensitive data had been removed from the details of a request, this data can still exist within the **View Changes** logs.  Authorized administrators can redact this data from these logs for privacy compliance (such as GDPR), security, or policy reasons.

![The View Changes window showing the redaction options for a specific field](/_books/servicemanager-user-guide/images/request-details-view-changes-redact.png)

#### Permissions

Only users with **Service Desk Admin** permissions can redact content. Redaction permanently removes the information from the record.

#### Redaction options for individual fields

When viewing changes for a specific field, admins can choose to redact:

- **Both the old and new values**: This removes all content for that field.
- **Only the old value**: This removes what the field contained before the change.
- **Only the new value**: This removes the updated information.

#### Redaction options for all fields

Admins can redact multiple fields at once by selecting one of these options:

- **Redact all content**: Removes both old and new values for every changed field in the record.
- **Redact all old content**: Removes all original values across all fields.
- **Redact all new content**: Removes all updated values across all fields.

#### The redaction process

Redaction is permanent and cannot be undone. To prevent accidental data loss, the system requires the following steps:

1. **Review the summary**: A warning screen appears showing exactly which fields the system will redact and how many fields are affected.
2. **Provide a reason**: You must enter a reason for the redaction (for example: "GDPR erasure request #12345"). The **Confirm** button remains inactive until you provide a reason.
3. **Confirm**: Click **Confirm** to permanently remove the data. Click **Cancel** if you want to close the warning without making changes.

#### After redaction

Once you confirm the redaction, the system updates the record:

- **Data removal**: The system replaces the sensitive values with the text ***[REDACTED]***.
- **Audit trail**: The change record remains visible so users can see that an update occurred, even though the specific values are hidden.
- **Redaction details**: The system displays the following information below the field:
  - Who performed the redaction.
  - The date and time of the redaction.
  - The reason provided for the redaction.

![The View Changes window showing the result after redaction with the [REDACTED] text and redaction details](/_books/servicemanager-user-guide/images/request-details-view-changes-redacted.png)
