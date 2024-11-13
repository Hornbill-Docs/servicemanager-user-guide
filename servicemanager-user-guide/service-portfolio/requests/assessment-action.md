# Assessment Action
The assessment action is for determining the importance of a request. Multiple assessment types can be used to make an assessment; these include priority, impact, urgency, and risk.

![Assessment Action](/_books/servicemanager-user-guide/service-portfolio/requests/images/assessment-action.png)

::: important
The only assessment type available by default is priority. Administrators must configure all the other assessment types. Administrators can navigate to Configuration > Administration and configure assessment types in [Levels](/servicemanager-config/administration/assessment-levels) and [Questionnaires](/servicemanager-config/administration/assessment-questionnaires).
:::

## Priority
Priority is the default option and is available to all requests that use the assessment action. Users choose from a drop-down list of [priority levels](/servicemanager-config/administration/assessment-levels#default-levels). Once a priority has been selected and applied to the request, it is displayed in the information panel.

![Request Priority](/_books/servicemanager-user-guide/service-portfolio/requests/images/request-info-priority.png)

### Benefits of using the Priority assessment
Setting the priority of a request allows users to focus on the most important requests. Users can:
* View color-coded priority levels in the request list.
* Sort the request list by priority to put the most important requests at the top.
* Determine the service-level targets that will be used for the request.
* Drive workflow automation based on the selected priority.
* Contribute to statistics and reports based on the priority levels.

## Impact
You can use the Impact assessment option to determine the effect a request may have on your business. Impact could be based on the number of users affected by the issue, or it could be based on something else, such as the issue's potential financial cost.

Impact is not available on the request's assessment action by default. Administrators have two options for configuring the use of impact:

* [Impact level drop-down list](/servicemanager-config/administration/assessment-levels#impact)
* [Impact questionnaire](/servicemanager-config/administration/assessment-questionnaires)

## Urgency
Urgency refers to how quickly the request must be resolved or closed. While an incident may not be causing too much trouble at the time it was raised, it might cause significant problems if it isn't resolved quickly.

Urgency is not available on the request's assessment action by default. Administrators have two options for configuring the use of urgency:

* [Urgency level drop-down list](/servicemanager-config/administration/assessment-levels#urgency)
* [Urgency questionnaire](/servicemanager-config/administration/assessment-questionnaires)

## Risk

Risk refers to the probability and or impact of this change being completed successfully.

Risk is not available on the request's assessment action by default. Administrators have two options for configuring the use of risk:

* [Risk level drop-down list](/servicemanager-config/administration/assessment-levels#risk)
* [Risk questionnaire](/servicemanager-config/administration/assessment-questionnaires)

## Request timeline
Each time an assessment is added or changed on a request, a record is added to the timeline.
