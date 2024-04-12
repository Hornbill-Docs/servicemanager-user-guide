# Service Bulletins
Service Manager provides the ability to create and publish Bulletins to the subscribers of Services.

* Bulletins are created and managed from the Service records in the Service Portfolio
* Each Service can have it's own Bulletins which are relevant to it's purpose
* Bulletins can be viewed by the subscribers of a service via both the Customer, Service, and Employee Portals
* Bulletins will be visible on the My Services Landing Page of the Portals, and on the Service Specific Pages on the Portal
* Where more than one Bulletin exists either on the Same Service or Across Multiple Services, the Bulletins will be displayed in a Carousel, transitioning automatically between each Bulletin every 5 seconds, unless paused or manually progressed.

## Creating a Bulletin
From the Service form, navigate to the Bulletin Tab, and select +Add Bulletin Item.

* **Specify a title for the Bulletin**<br>This acts as a heading on the bulletin.
* **Add a Description**<br>This will be displayed immediately beneath the title. The text editor can be used to format the text and create hyperlinks to other resources or more detailed content. The description cannot exceed 400 Characters.
* **Upload a background image**<br>The recommended image dimensions are 1000px x 300px.
* **Configuration Options**
    * Display Bulletins Text - This allows you to hide the bulletin title and description text. This is desirable if your background image contains the message you wish to display meaning additional text is not necessary. This configuration option is "ON" by default.
    * Display Bulletins Text Shadow - This option determines whether the title and description text have a shadow. The shadow may affect how the text can be seen against your chosen background image and so the state of this setting will depend on that.
* **Bulletin Visibility**<br>This feature allows you to control the date and time that a Bulletin becomes visible or hidden on the Bulletin Slideshow component.
    * If the Start is left blank, the Bulletin will be immediately visible when the Bulletin is published
    * If the End is left blank, the Bulletin will remain visible until the Bulletin has been retired
* **Employee Portal Link**<br>Adding a link here will make the entire bulletin a clickable hyperlink when displayed in the Employee Portal.
* **Create the Bulletin in multiple Languages**<br>If your subscribed users work in multiple languages, define the Bulletin in the required languages. The users will see the appropriate language Bulletin on the Customer, Service, and Employee Portals based on the language set in their regional settings (by default an English version is created).
* **Status**<br>A bulletin can be in one of three states:
    * Draft - The Bulletin will not be visible on the Customer, Service, and Employee Portals
    * Published - The Bulletin will be visible on the Customer, Service, and Employee Portals
    * Retired - When retired, the Bulletin will not be visible on the Customer, Service, or Employee Portals.

## Viewing Bulletins
When Bulletins are marked as published, any subscribed user of the Service against which the Bulletin has been published will be able to view the Bulletin on the Customer and Service Portals in two locations:

* **My Services View**<br>If multiple Bulletins have been published from either the same or different Services a User is subscribed to, they will view the Bulletins in a carousel at the top of the My Services view.
    * Click on the Bulletin details, or the Service Name to be taken to the Service View which the Bulletin relates too.
    * Clicking on any hyper-link in the Bulletin text will open the link in a new browser tab.
* **Service Specific Details View**<br>If one or multiple bulletins have been published from the same Service, they will appear in Service Specific View. Again if there are multiple Bulletins these will appear in a carousel.
* Clicking on any hyper-link in the Bulletin text will open the link in a new browser tab.

If multiple Bulletins are published they will automatically transition every 5 seconds, if not manually progressed using the Arrow controls on the Carousel.

Bulletins are displayed in the Employee Portal using the corresponding Bulletins Widget, and are also shown in the specific service view.

## Managing Bulletins
Bulletin's can be created and viewed from the Bulletins tab on each service record.

* The list shows each Bulletin with various attributes including:
    * Status
    * Title
* Filter the List by Active or Retired Bulletins's
* Reorder the sequence in which the Bulletins will appear on the self service portals by dragging and dropping the Bulletins into the required order in the list.
* Edit or change the status of an Bulletin by clicking through into the Bulletins details from the Cog Icon
* Delete the Bulletin by clicking on the Trash Can Icon.
* Bulletin text will not display on the Bulletin in the list, if the bulletin has the Display Bulletin Text set to off