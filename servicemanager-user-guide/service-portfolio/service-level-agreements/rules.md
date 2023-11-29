# Rules
Once you have created a service level agreement, you may have a requirement for more than one service level and its associated targets to be available. When more than one service sevel has been defined within your service level agreement, the Manage Rules tab will become enabled. This will allow you to configure your rules for when each of the available Service Levels should be invoked.

## Managing Rules
### Adding Rules
* **Name**<br>The Name of the Rule
* **Service Level**<br>The Service level which you would like to be invoked should the conditions of this rule be met
* **All**<br>Configure one or multiple conditions which All must match in order for the rule to be met and the defined Service Level to be invoked.
* **Any**<br>Configure one or multiple conditions where Any of the the conditions can match, in addition too any All must match conditions in order for the rule to be met and the defined Service Level to be invoked.

### Configuring Rule Conditions
1. Click on the `Add Condition` button
1. Choose one of the available Condition parameters
1. Choose if the Condition for the parameter is looking for a match on Is or Is not
1. Add one or more values against the Condition parameter

Repeat the above for any additional Conditions you wish to set against the Rule, and click on Create when finished configuring the conditions for the Rule.

### Managing the Order Rules are Evaluated
It is possible to define multiple rules per Service Level Agreement. When a request is raised using the Service Level Agreement the system logic will start by evaluating the first rule in the list looking for a match, if no match is found with the first rule, it will evaluate the remaining rules in list order until the first rules match is found.

Reorder the rules in the list by using the up and down arrows which will be visible once more than one Rule has been configured against the Service Level Agreement.
If no rules are matched, then No Service Level will be used or invoked on the request
Editing and Deleting Rules
Click on the Rule in the list you wish to edit or delete.
Add, Amend or Remove Conditions of the Rule and Click Save to apply the edit
Click Delete to Delete the Rule from the Service Level Agreement

## When are the Rules Evaluated?
Once you have created your rules that will determine when a particular Service Level Agreement (SLA) and Service Levels will be invoked, it is useful to understand when the service manager application will evaluate your rules, and how this takes place.

The trigger which invokes a service level agreement and thus sets a service level against a request is performed via Hornbill business process. Without a business process, Service Level Management will not be applied to the request. More specifically, the trigger occurs when the BPM reaches a node involved with the starting of a timer, either the "start response" or "start resolution" timer node.

The high level steps are as follows:
1. The request is logged and a BPM is successfully initiated.
1. The BPM reaches either the "start response" or "start resolution" timer node (This is an automated operation and will be represented by a blue node in your business process workflow).

The application logic then takes over and performs the following:
1. Checks the service against which the request is logged
1. If there are multiple Service Level Agreements (SLAs) associated to the Service, the application will first evaluate the SLA rules and determine which SLA should be invoked. If there is only one SLA associated to the Service, this will be chosen.
1. The application logic will then focus on the SLA that has been identified, and work through the Service Level rules. Upon finding a rule which contains matching conditions, Service Level targets will be set against the request.

## Troubleshooting Service Level Management
If you've configured your SLA's and service levels, but continue to find some or all of your requests fail to have targets initiated, there are a few things you can check:

Does the request have an active business process? (usually indicated by the presence of the green heads up display at the top of a request).
* Does the Service have an SLA associated to it?
* If there is more than one SLA associated, have rules be created to determine which SLA should be used.
* If an SLA is being associated, but no targets are being set, check that you have configured rules against each Service Level within your SLA.
* Check that you have appropriate conditions defined for each rule.
* If you have rules configured, but still the SLA and/or Service Level targets fail to be set, ensure that the criteria being used to set the appropriate SLA, and also service level, is present on the request before the BPM reaches the node responsible for triggering the evaluation of the rules. i.e. if the triggering of an SLA is depended on the priority being established, ensure the request has a priority set before triggering the evaluation of the service level rules. This may mean the location of the node(s) has to be considered in the BPM or perhaps utilizing a relevant "suspend" node.

What happens if I change something in a request, will the SLA and Service Level targets be updated?

By default, the changing of the service level following a change in any of the criteria governing the response or fix targets is a manual action. E.g. if your service levels are based on the priority, if the priority is changed, the service level must also be changed in a separate action. A service level can be amended by clicking on the name of the service level located in the request information area on the right hand side of the request. In order to amend a Service Level, a user must posses one of the following roles: "Service Request Full Access", "Incident Management Full Access", "Problem Management Full Access", or "Change Management Full Access". Possessing the "Service Desk Admin" role will also allow the user to amend the service level.

### Automated Service Level Changes
If you prefer that Service Levels are automatically updated, enabling the application setting guest.app.view.ITSM.serviceDesk.slm.enableAutomatedSLChanges will provide this. When any of the following is changed on a request, the Service Level Rules will be re-assessed automatically.
* Customer
* Company
* Team
* Site
* Priority
* Category

<!-- https://wiki.hornbill.com/index.php?title=Service_Level_Rules_Builder -->