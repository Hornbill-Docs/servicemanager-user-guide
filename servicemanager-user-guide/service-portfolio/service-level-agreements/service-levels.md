# Service Levels
One or more Service Levels can be defined for each Service Level Agreement. Each Service Level contains configurable Service Level Targets and their associated automated escalations. Service Levels are required if you need to automate and track targets such as response and resolution targets.

* **Name**<br>The name of the Service Level will be displayed along with the SLA on a request that it is assocaited to. This is used to help a support person understand the Service Level that they need to adhear to. An example of a common naming convention for Service Levels is Bronze, Silver, and Gold.
* **Description**<br>Define the purpose of the SL and what it covers. This can be used by Service Desk Staff when changing an applied Service Level against a request.

## Service Level Targets
Service Level Targets allow you to define the timing for your response and resolution targets. Providing these targets is optional, however using these is an important part of keeping track of the performance provided by the service desk. Both the response and resolution targets are calculated against the selected Working Hours Calendar. By selecting any of the existing Service Levels you will be able to manage the associated targets for that Service Level.

### Target Types
* **Response Target**<br>The time in which a response to a new request needs to be made.
* **Resolution Target**<br>The time in which a suitable resolution to a request has been completed and a normal level of service provided.

#### Service Level Target Calculation
The service level targets that you add to Hornbill relate to the working hours defined in the working time calendar specified against the SLA. This means that some calculation is required to ensure the targets you set represent the correct number of calendar days that you are advertising to your customers.

#### Example
If you have a target that you advertise as 5 calendar days, you need to determine what this equates to in days, hours, and minutes in relation to the hours defined in your Working time calendar.

1) Begin by multiplying your target (in calendar days) by the working hours set in your working time calendar (your working day) i.e. 5 x 9.5. Now divide the result of that by 24 (i.e. (47.5)/24) which gives your Hornbill target in days (i.e. = 1.98 days).
2) You place "1" in the field representing "days".
3) It's then a case of working out what .98 of a day is in hours – which in this case would be 24 x 0.98 = 23.52 hours.
4) You place "23" in the field representing "hours".
5) Finally, we then need to get the minutes from our answer of 23.52. Therefore, 0.52 of an hour is 31.2 minutes (i.e. 60 x 0.52 = 31.2 minutes).
6) You place "31" in the field representing "minutes".

Therefore the target of 5 calendar days based on a 9.5 hour working day equates to 1 day, 23 hours, 31 minutes.

More details of this can be found in the [Service Level Workflow Automation](/servicemanager-user-guide/service-portfolio/service-level-agreements/automation) document.

## Escalation Actions
Against each Service Level Target you can configure escalation actions which will get automatically invoked should the Service Level still be active at defined time intervals before and or after the specific Target of the Service Level.

### Timers
Against each Service Level Target you can configure escalation actions which will get automatically invoked should the Service Level still be active at defined time intervals before and or after the specific Target of the Service Level.
* **Before the Target**<br>Specify this in Days / Hours / Minutes how long before the Target has been reached that an event will take place
* **After the Target**<br>Specify this in Days / Hours / Minutes how long after the Target has passed that an event will take place

### Actions
You can specific one or more Actions which you want to be invoked against each Escalation Event. Configure the required Actions by clicking on the icons to expose the configuration options for each action type.

* **Send Notification**<br>This will send a Hornbill notification to the following (If this has been specified).
    * Owner
    * Owners Manager
    * Team (Which the request is assigned to)
    * Specified Recipients
* **Post to Timeline**<br>Tick if you want the notification text to be posted on the timeline of the impacted request.
* **Notification Text**<br>Specify the text which will appear in the Hornbill Notification
* **Send Reminder**<br>This will send an email to the following(if this has been specified).
    * Owner
    * Owners Manager
    * Team (Which the request is assigned to)
    * External Email Addresses (multiple - Comma separated)
    Mailbox**<br>Name of Mailbox where the email will originate
    To - The Recipient
    Email Template - The Predefined Email Template which will be sent
    Subject - The Email Subject
    Escalation Text - The text which will appear inside the predefined email template specified above
* **Assign**<br>This option will reassign the request to a specified team, and or individual analyst.
* **Increase Priority by 1**<br>What ever the priority is currently at, this will increase the priority by one level.
* **Add to Board**<br>If you have boards configured, this option will add the request to a specified board, with the option to specify a particular list within the chosen board. If no list is specified, then the request will be added to the first (left-most) list on the Board. Typically this can be used to create a Breach Board, with lists representing the time left before the Service Level Target will be missed. More information on Boards can be found on the My boards wiki page.

## Managing Service Level Rules
If you create more than one Service Level for any of your SLA's, you will enable the Manage Rules tab. This will allow you to configure rules to manage when the different Service Levels of your SLA should be used. Learn more about configuring rules for your Service Level Agreement here

<!-- https://wiki.hornbill.com/index.php?title=Escalation_Actions -->