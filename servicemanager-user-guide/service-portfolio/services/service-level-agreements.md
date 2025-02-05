# Service Level Agreements
The use of Service Level Agreements can be a requirement to ensure an agreed level of support is provided to the customers that are subscribed to a service. Within each service, you can either define a unique service level agreement that is particular to the service or you can associate the service to a shared Service Level Agreement which can be shared across multiple Services. For each Service Level Agreement, you can configure Service Levels along with Service Level Targets and automated escalation actions.

## Configuration
Under the Configuration tab, you have the option of either linking to an existing Corporate Service Level Agreement or you can create a Service Level Agreement that is specific to this Service.

### Linking Corporate Service Level Agreements
A service can link to one or more existing Corporate Service Level Agreements. Corporate Service Level Agreements can be shared with multiple services. Linked Corporate Service Level Agreements can not be edited from within a Service as this may have consequences for other linked Services.
* **Search**<br>Type in the name of the Corporate Service Level Agreement that you wish to link with this service. Once located, click on the Link button to add the Corporate Service Level Agreement to the Service.

### New Service Level Agreement
A Service Level Agreement that is specific to this service can be created using the + New Service Level Agreement button.

* **Name**<br>The Name provides visibility of this Service Level Agreement and can be used from within the Service, BPM Operations, Reports, and other areas.
* **Description**<br>Provide a description to allow other users that have access to the Service to have an understanding of the use of the service. level agreement.
* **Working Time Calendar**<br>The Working Time Calendar will indicate the working periods that the team(s) that support the service are available. The selected calendar will be used to calculate target times for the Service Levels that come under this Service Level Agreement
* **Service Levels**<br>This option is only available once the Service Level Agreement has been created. Service Levels can be added which allows Service Level Targets and automated escalation actions to be defined.

## Manage Rules
Once you have created or associated more than one Service Level Agreement to a service, the selection of the SLA can be automated based on configurable rules. When more than one Service Level Agreement has been defined within your Service, the Manage Rules tab will become enabled.

* **Adding Rules**<br>Click on the New Rule button to create and add a new rule to invoke the correct SLA.
* **Name**<br>Add a name to the rule that will allow it to be easily identified in the list of rules.
* **Service Level Agreement**<br>Select the Service Level Agreement which you would like to be invoked should the conditions of this rule be met.
* **All** of these conditions must match<br>Configure one or multiple conditions which All must match for the rule to be met and the defined Service Level Agreement to be invoked.
* **Any** of these conditions must match<br>Configure one or multiple conditions where Any of the the conditions can match, in addition to any All must match conditions for the rule to be met and the defined Service Level Agreement to be invoked.

### Configuring Rule Conditions
An extensive condition builder is available to determine which SLA should be invoked under these conditions.

1. Click on the Add Condition button
1. Choose one of the available Condition parameters
1. Choose if the Condition for the parameter is looking for a match on Is or Is not
1. Add one or more values against the Condition parameter

Repeat the above for any additional Conditions you wish to set against the Rule, and click on Create when finished configuring the conditions for the Rule.

### Managing the Order Rules are Evaluated
It is possible to define multiple rules per Service. When a request is raised using the Service the system logic will start by evaluating the first rule in the list looking for a match, if no match is found with the first rule, it will evaluate the remaining rules in list order until the a rule match is found.
* Reorder the rules in the list by using the up and down arrows which will be visible once more than one Rule has been configured against the Service.
* If no rules are matched, then No Service Level Agreement will be used or invoked on the request.
* If no rules have been configured, the first Service Level Agreement in the list of Service Level Agreements linked to the Service will be used.

### Editing and Deleting Rules
* Click on the Rule in the list you wish to edit or delete.
* Add, Amend or Remove Conditions of the Rule and Click Save to apply the edit
* Click Delete to Delete the Rule from the Service