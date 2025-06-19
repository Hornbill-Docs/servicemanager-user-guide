# Schedule
The Schedule Action Item lets you define a start and end date for when this request will be implemented. This feature is only available for Change Requests and Releases.

## Adding and removing a schedule
The Schedule Action can be used for both adding and removing a schedule. 

### Schedule Change
Both a From and a To date are required when scheduling a change or release. Once the dates are entered you can click on the Schedule Change button to add the schedule and have it display on the Calendar.

### Change Freeze Periods
When attempting to schedule a change, if a change freeze exist and the dates collide, the user will automatically be notified.
* The Change Freeze icon will remain clear if no collision is detected, but it will turn red if the dates are during a change freeze. Users can click on the freeze icon at any time to manually view any clashes or upcoming change freeze periods.
* If a user attempts to schedule a change during a change freeze period, the Add Schedule button will remain inactive. 
    > The exception to this rule is for any user who has either the Full Change Management Access or the Full Release Management Access roles, and they will be prompted and warned about the collision with any change freeze periods, but will have the rights to proceed with the scheduled dates.
    > Change Freeze periods can be added and managed via the forward schedule of change calendar view by users whom have the above roles.
* Schedule Action Icon
Once a request has been scheduled, the icon for the Schedule Action on a request will turn Green to provide an indicator when viewing the request that a schedule has been set.

## Workflow automation
The adding and removing of a Change Schedule can also be automated within the workflow. For more information please see the [Change Request Automation](/servicemanager-config/customize/workflows/change-request-automation) documentation.

### Add to Change Calendar
The From and To dates are set by selecting the number of days from the point that this step in the process is reached. For example Start this change 5 days from now and finish in 6 days from now. The corresponding dates will be automatically added.

### Remove from Change Calendar
This will remove both the From and To dates from a change request. This can be useful for when a change or release has been rejected after it has been scheduled or you may want to remove the change from the Change Calendar once the change / release has been completed.