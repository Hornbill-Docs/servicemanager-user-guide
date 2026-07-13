# Request snippets

Snippets are pre-defined responses that you can include in request updates, outgoing emails, or resolutions. Use snippets to save time and ensure your team provides consistent information to customers.

- Snippets can include plain text and request variables.
- You can share snippets with specific teams and services.

## Manage snippets

You can access the snippet manager from the **Update**, **Email**, or **Resolution** actions on any request.

1. Open a request.
2. Select the **Snippet** dropdown menu.
3. Select **Manage** to create, update, share, or delete snippets.

### Add a new snippet

To create a new snippet, select **Add New** from the **Manage** menu. You must complete the following attributes:

- **Title**: Enter a name for the snippet. This title helps you and other analysts identify the snippet in the list. It does not appear in the final message.
- **Content**: Enter the text that the system inserts into the email or update body.
- **Available On**: Select whether the snippet appears in the **Update** action, **Email** action, **Resolution** action, or all three.
- **Available For**: Define who can use the snippet.
  - **Myself**: The snippet is only visible to you.
  - **Teams**: Choose one or more teams to share the snippet with their members.
  - **Services**: Choose one or more services. The snippet becomes available to all teams that support those services.

Select **Save** to create the snippet.

Snippet lists

The manager organizes snippets into three lists:

- **All**: Visible only to users with the **Service Desk Admin** role. This list contains every snippet in the system.
- **Shared**: Contains snippets that other users have shared with you.
- **My Snippets**: Contains snippets that you created.

### Bulk actions

Use the checkboxes next to snippets in the list to perform bulk actions:

- **Change Owner**: Available only to Service Desk Admins. Use this to transfer snippet ownership to another user.
- **Make Me Owner**: Available only to Service Desk Admins. Use this to quickly take ownership of the selected snippets.
- **Delete**: Permanently removes the selected snippets from the system.

### Edit a snippet

To modify an existing snippet, select the name of the snippet in the list. This opens the **Snippet Editor**. After making your changes, select **Update** to save.

## Use request variables

Variables allow you to pull specific data from a request automatically. This prevents the need to type details like reference numbers or names manually.

To insert a variable, select the variable from the dropdown menu while editing the **Content** field. The system inserts the variable at your current cursor position.

Available variables:

- Customer First Name
- Customer Last Name
- Reference
- Summary
- Description
- Owner Name
- Service Name
- Priority
- Response Target
- Resolve Target
- Current Time
- Current Date
- Current Date / Time

## Use HAi with snippets

![HAi logo](/_books/servicemanager-user-guide/images/hai-logo-22x22.png) You can combine snippets with request variables and the **Ask HAi** feature of [**Text Assist**](/servicemanager-user-guide/hai/text-assist) to generate custom AI prompts.

For example, you can create a snippet to generate clarifying questions based on the request details:

```text
{{summary}}
{{description}}
Write 4 clarifying questions to solve this issue.
```

![Snippet Tip](/_books/servicemanager-user-guide/images/hai-snippet.png)

To use a snippet with HAi Text Assist:

1. Go to the **Update** action on a request.
2. Select the **Snippets** dropdown and choose the snippet containing your HAi prompt.
3. Select **Ask HAi** from the **HAi Text Assist** dropdown menu.
4. Select **Update** to add the snippet content to the request.

![Snippet Response](/_books/servicemanager-user-guide/images/hai-snippet-2.png)

## Apply a snippet to a request

When you are ready to use a snippet in a ticket:

1. Open the **Email**, **Resolution**, or **Update** action.
2. Select the **Snippets** button.
3. Choose a snippet from one of the following categories:
    - **Myself**: Snippets you created.
    - **Teams**: Snippets shared with your teams.
    - **Services**: Snippets associated with the service assigned to the ticket.

The categories only appear if there are snippets available for you to use.
