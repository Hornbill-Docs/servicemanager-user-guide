# Service levels
You can define one or more service levels (SLs) for each SLA. Each service level contains configurable service level targets and their associated automated escalations. Service levels are required if you need to automate and track targets such as response and resolution targets.

* **Name.** The name of the service level is displayed along with the SLA on a request that it is associated to. This is used to help a support person understand the service level that they need to adhere to. An example of a common naming convention for service levels is *Bronze*, *Silver*, and *Gold*.
* **Description.** Define the purpose of the SL and what it covers. This can be useful for service desk staff when changing an applied service level against a request.

## Service Level Targets
Service level targets allow you to define the timing for your response and resolution targets. Providing these targets is optional, however using them is an important part of keeping track of the performance provided by the service desk. Both the response and resolution targets are calculated against the selected Working Hours Calendar. By selecting any of the existing SLs, you will be able to manage the associated targets for that service level.

### Target types
* **Response Target.** The time in which a response to a new request needs to be made.
* **Resolution Target.** The time in which a suitable resolution to a request has been completed and a normal level of service provided.

#### Calculating service level targets
The service level targets that you add to Hornbill relate to the working hours defined in the Working Time Calendar (WTC) specified against the SLA. This means that some calculation is required to ensure the targets you set represent the correct number of calendar days that you are advertising to your customers.

#### Example
If you have a target that you advertise as 5 calendar days, you need to determine what this equates to in days, hours, and minutes in relation to the hours defined in your WTC.

**To calculate the number of calendar days:**
1. Begin by multiplying your target (in calendar days) by the working hours set in your WTC (your working day), i.e. 5 x 9.5.
1. Divide the result of that by 24 (i.e. (47.5)/24), which gives your Hornbill target in days (i.e. = 1.98 days).
1. Enter *1* in the field representing "days".
1. Now work out what .98 of a day is in hours. In this case, it would be 24 x 0.98 = 23.52 hours.
1. Enter *23* in the field representing "hours".
1. Finally, get the minutes from the answer of 23.52. 0.52 of an hour is 31.2 minutes (i.e. 60 x 0.52 = 31.2 minutes).
1. Enter *31* in the field representing "minutes".

Therefore the target of 5 calendar days based on a 9.5 hour working day equates to 1 day, 23 hours, and 31 minutes.

More details of this can be found in [Service Level Workflow Automation](/servicemanager-user-guide/service-portfolio/service-level-agreements/automation).

## Escalation actions
Against each service level target, you can configure escalation actions that will get automatically invoked should the service level still be active at defined time intervals before and/or after the specific target of the service level.

### Timers
Against each service level target, you can configure timers that will get automatically invoked should the service level still be active at defined time intervals before and/or after the specific target of the service level.
* **Before the Target.** Specify in days/hours/minutes how long before the target has been reached that an event will take place.
* **After the Target.** Specify in days/hours/minutes how long after the target has passed that an event will take place.

### Actions
You can specify one or more actions that you want to be invoked against each escalation event. Configure the required actions by clicking on the icons to expose the configuration options for each action type.

* **Send Notification.** This will send a Hornbill notification to the following (if this has been specified):
    * Owner
    * Owner's Manager
    * Team (which the request is assigned to)
    * Specified Recipients
* **Post to Timeline.** Tick if you want the notification text to be posted on the timeline of the impacted request.
* **Notification Text.** Specify the text that will appear in the Hornbill notification.
* **Send Reminder.** This will send an email to the following(if this has been specified):
    * Owner
    * Owner's Manager
    * Team (which the request is assigned to)
    * External Email Addresses (multiple - comma-separated)
    * Mailbox. Name of mailbox where the email will originate.
    * To. The recipient.
    * Email Template. The predefined email template that will be sent.
    * Subject. The email's subject line.
    * Escalation Text. The text that will appear inside the predefined email template specified above.
* **Assign.** This option will reassign the request to a specified team and/or individual analyst.
* **Increase Priority by 1.** Whatever the priority is currently at, this will increase the priority by one level.
* **Add to Board.** If you have boards configured, this option will add the request to a specified board, with the option to specify a particular list within the chosen board. If no list is specified, then the request will be added to the first (left-most) list on the board. Typically, this can be used to create a breach board, with lists representing the time left before the service level target will be missed.

<!-- https://wiki.hornbill.com/index.php?title=Escalation_Actions -->