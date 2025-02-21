# Service levels
A service level is a measurable performance indicator used to assess the quality or efficiency of a service provided to customers. It’s a metric that helps organizations evaluate how well they are meeting predefined goals and commitments.

You can define one or more service levels for each SLA. Each service level contains configurable service level targets and their associated automated escalations. Service levels are required if you need to automate and track targets such as response and resolution targets.

* **Name.** The name of the service level is displayed along with the SLA on a request that it is associated with. This is used to help a support person understand the service level that they need to adhere to. An example of a common naming convention for service levels is *Bronze*, *Silver*, and *Gold*.
* **Description.** Define the purpose of the service level and what it covers. This can be useful for service desk staff when changing an applied service level against a request.

![Service Levels](/_books/servicemanager-user-guide/images/sla-service-levels.png)

## Service level targets
Service level targets allow you to define the timing for your response and resolution targets for each service level. These targets can be an important part of keeping track of the performance provided by the service desk.

![SLA Service Level Targets](/_books/servicemanager-user-guide/images/sla-service-level-targets.png)

### Target types
* **Response Target.** The time in which a response to a new request needs to be made. 
* **Resolution Target.** The time in which a suitable resolution needs to be provided and an acceptable level of service has been restored.

:::info
The starting, pausing, and marking of the service level targets are managed within a workflow using the [Timer Hornbill Automation](/servicemanager-config/customize/workflows/timer-automation).
:::

### Calculating service level targets
Each service level target allows you to set the number of days, hours, and minutes that will be used to determine the target time.  The service level targets are calculated using the working hours defined in the [Working Time Calendar (WTC)](/servicemanager-user-guide/service-portfolio/service-level-agreements/overview#details) set against the SLA. Any time outside of working hours is not included in the calculation. 

![SLA New Resolution Target](/_books/servicemanager-user-guide/images/sla-new-resolution-target.png)

#### Calculate days, hours, minutes from calendar days
Use this calculation to work out the values for days, hours, and minutes when working from a desired number of calendar days. This example is based on having an 8.5 hour work day set in the WTC.

:::important
The `Days` field represents 24 hours for each day specified. If the associated [WTC](/esp-config/customize/working-time-calendars) has each working day set to 8 hours, a value of 1 Day would equate to 3 working days (24/8).   
:::

1. Calculate the number of days.
    1. Multiply the number of calendar days by the working hours for one day (5 calendar days x 8.5 working hours = 42.5).
    1. Divide the result by 24 hours (42.5 working hours/24 hours = 1.77 days).
    1. Enter `1` in the "days" field.
1. Calculate the number of hours.
    1. Multiply 24 hours by the remainder of the days calculation. (24 hours x 0.77 of a day = 18.48 hours).
    1. Enter `18` in the "hours" field.
1. Calculate the number of minutes.
    1. Multiply 60 minutes by the remainder of the hours calculation (60 x 0.48 = 28.8 minutes).
    1. Enter `30` in the "minutes" field (Minutes can only be entered in 5 minute increments).
 
    ![SLA Target Time](/_books/servicemanager-user-guide/images/sla-target-time.png)

## Escalation events
Against each service level target, you can configure escalation events that will get automatically invoked should the service level still be active at defined time intervals before and/or after the specific target of the service level.

![Escalation Events](/_books/servicemanager-user-guide/images/sla-escalation-events.png)

### Timing
Against each service level target, you can set the time that an escalation event will get automatically invoked should the service level still be active.
* **Before the Target.** Specify in days/hours/minutes how long before the target has been reached that an event will take place.
* **After the Target.** Specify in days/hours/minutes how long after the target has passed that an event will take place.

:::important
The `Days` field for escalation events works the same as the service level targets.  Please see the section for [calculating service level targets](/servicemanager-user-guide/service-portfolio/service-level-agreements/service-levels#calculating-service-level-targets) 
:::

### Actions
You can specify one or more actions that you want to be invoked against each escalation event. Configure the required actions by clicking on the icons to expose the configuration options for each action type.

* **Send Notification.** This will send a Hornbill notification to the following (if this has been specified):
    * Owner
    * Owner's Manager
    * Team (which the request is assigned to)
    * Specified recipients
    * Post to timeline.
    * Notification text.
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