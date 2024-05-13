# Request Snippets
Snippets provide the ability to define common responses that can be included in an update, outgoing email, or as part of a resolution. The use of Snippets ensures that the same response does not need to be typed manually each time, and to ensure a consistent level of response is given by all analysts who use the snippets rather than manually entering responses each time.
* Snippets can include text and variables
* Snippets can be shared with other Teams and Services

## Manage Snippets
From the Update, Email, or Resolution actions on a request you will be able to access Snippets. From the Snippet drop down you can select Manager to create, update, share, or delete a Snippet.

### Add New
From the Manage option you can then choose Add New.

#### Snippet Attributes
* **Title**<br>This is used to define or name the Snippet and any text entered here will not be inserted, this will simply be used to describe the Snippet for you or other analysts to select.
* **Content**<br>This is the text which will be inserted into the body of the email, when the Snippet is chosen.
* **Available On**<br>Select if the snippet will be available on the Update, Email Action, Resolution Action, or all three.
* **Available For**<br>This will allow you to either create the Snippet for yourself, or to choose to share and make the Snippet available to analysts in other teams, or for those analysts whose team's support specific services.
    * Myself: Choose this option to only make the Snippet Available to yourself
    * Teams: Choose one or multiple teams to make this Snippet available to
    * Services: Choose one or multiple Services to make the Snippet available to the teams which are supporting these Services.
Once the Mandatory selections have been made, select Save to create and make the Snippet available.

### Snippet Lists
* **All**<br>This list is only available to users with the Service Desk Admin role. From here all Snippets belonging to any user can be managed.
* **Shared**<br>This list shows all the Snippets that have been shared with you, and you are not the owner.
* **My Snippets**<br>This list shows all of the Snippets that you own.

#### Select Box Options
On each of the lists, a select box is available to select one or more Snippets to perform one of the following options.
* **Change Owner**<br>This option is only available if you have the Service Desk Admin role. This will allow you to change the Owner of the selected Snippets.
* **Make Me Owner**<br>This option is only available if you have the Service Desk Admin role. This is a quick option to set you as the owner of all the selected Snippets.
* **Delete**<br>This will permanently delete the Snippet.

### Edit
You can edit or alter a Snippet by clicking on the Snippet's name within the lists. This will open the Snippet Editor where you can make your changes and select Update to save your changes.

### Using Request Variables
When creating Snippets it can be useful to include Variable content from the request, this could include inserting the Reference Number, Customer Name, or other variables into the Snippet to remove the need to manual add these each time you wish to send an email from the request.

Available Variables:
* Customer First Name
* Customer Last Name
* Reference
* Summary
* Description
* Owner Name
* Service Name
* Priority
* Response Target
* Resolve Target
* Current Time
* Current Date
* Current Date / Time

Insert variables into the Content text box by selecting the appropriate variable from the drop down list at the required points in the sentences and paragraphs of the Snippet text.

## Using Snippets
Once Snippets have been created and shared, they will be available to use from the Snippets button on the Email, Resolution and Update actions on a request. To insert a Snippet simply choose the snippet from the list of Snippets which are available to you. The Snippets will be available from one of three options:

* **Myself**<br>Snippets you have created.
* **Teams**<br>Any Snippets which have been shared with teams you are a member of
* **Services**<br>Any Snippet that has been shared and is available to the Service which the ticket is raised against.

The above options will only appear if Snippets exist and have been shared with you, or you have created Snippets yourself.