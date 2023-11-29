# Workflow automation

When configuring SLA response and resolution targets and expiry times on certain BP nodes you might find the target being set differently than possibly expected. This is because a common oversight as these timers needs to be expressed in SLC (Service Level Calendar) times or working hours or business hours (which are usually X hours/day) rather than calendar time (which is 24 hrs/day).

When configuring a target time of N days, the value needed to be set would be N working days rather than N calendar days. The value that needs to be set will be obtained by multiplying N with the number of working or business hours/day.

We advise to always configure hours (rather than days) as it is easier to figure out the values required to be configured for SLA targets or expiry times on business process nodes. However, in certain areas (e.g. SLA timers), depending on the target, it might not be always possible to use hours exclusively. Below is a quick example of how to find out which values needs to be configured depending on the intended target:

Let's say we need to configure a resolution time (or an expiry time) of 5 days. We need the target to be set in 5 days from now. Let's also say the working hours are 7.5 hours/day although this really depends on your SLC. 

Step 1 is to find out the number of working hours equal to the 5 days we need to set: 5 days * 7.5 hrs/day = 37.5 hours. You need to configure round values therefore if you don't have a round number of hours you also need minutes (seconds, etc.). The 37.5 hours equates to 37 hrs and 30 min. In conclusion, for a 5 day target, the configuration needs to be 37 hrs and 30 min. As mentioned above, for simplicity always use hours if possible. If you need to configure this value as days/hours/min then the 37.5 hours need to be divided by 24 (which is the number of calendar hours in a day) resulting in 37.5 / 24 = 1.56 days. The 1.56 days equates to 1 day and 13.50 hours. This further equates to 1 day 13 hours and 30 min. In conclusion:

5 day target in the context of 7.5 working hours/day is set as: 37 hours and 30 minutes or 1 day 13 hours and 30 min

If you don't want to be bothered with the mathematical calculation, you can use this Excel sheet to find out what values you need to configure. Type in the desired target time and the number of working hours per day. The values you need to configure are in red: Hornbill_Timer_Targets.xlsx


IMPORTANT: the above only applies when configuring expiry times on Service Manager workflow nodes. Non-application nodes, such as human tasks or external authorisations, do not account for Working Time Calendar, and as such the above setup does not apply in this scenario.

<!-- https://community.hornbill.com/topic/13775-setup-and-configure-timers-in-service-manager/ -->