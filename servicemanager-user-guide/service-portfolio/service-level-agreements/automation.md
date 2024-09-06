# Service Level Workflow Automation

When configuring SLA response and resolution targets and expiry times on certain Workflow nodes you might find the target is set differently than expected. This is a because these timers need to be expressed in SLC (Service Level Calendar) times or working hours or business hours (which are usually X hours/day) rather than calendar time (which is 24 hrs/day).

When configuring a target time of N days, the value needed to be set is N working days instead of N calendar days. The value set will be obtained by multiplying N with the number of working or business hours/day.

Hornbill recommends that you configure hours rather than days as it is easier to calculate the values required to be configured for SLA targets or expiry times in Workflows nodes. However, in certain areas, for example SLA timers, depending on the target it might not be always possible to use hours exclusively. 

## Example of determining target values

Here is an example of how to find out which values needs to be configured depending on the intended target.

Imagine that you need to configure a resolution time, or an expiry time), of 5 days. You need the target to be set in 5 days from now. Also imagine that the working hours are 7.5 hours a day.

Calculate the number of working hours equal to the 5 days we need to set: 5 days * 7.5 hrs/day = 37.5 hours. 

Here, you need to configure round values. If you don't have a round number of hours you also need minutes (seconds, etc.). But in this example, the 37.5 hours equates to 37 hrs and 30 min. 

So for your 5 day target, the configuration must be 37 hrs and 30 min. Again, for simplicity always use hours where possible. If you need to configure this value as days/hours/min then the 37.5 hours need to be divided by 24 (which is the number of calendar hours in a day) resulting in 37.5 / 24 = 1.56 days. The 1.56 days equates to 1 day and 13.50 hours. This further equates to 1 day 13 hours and 30 min. 

To summarize our example:

A 5 day target in the context of 7.5 working hours/day is set as: 37 hours and 30 minutes or 1 day 13 hours and 30 min.

IMPORTANT: The rules described here only apply when configuring expiry times on Service Manager Workflow nodes. Non-application nodes, such as human tasks or external authorisations, do not account for Working Time Calendar, and as such the above setup does not apply in this scenario.

<!-- https://community.hornbill.com/topic/13775-setup-and-configure-timers-in-service-manager/ -->
<!-- 
To help you perform time calculations, you can use this Excel sheet to find out what values you need to configure. Type in the desired target time and the number of working hours per day. The values you need to configure are in red: Hornbill_Timer_Targets.xlsx -->
