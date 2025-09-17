# Service Level Rules
Once you have created an SLA, you may have a requirement for more than one service level and its associated targets to be available.

## Topics covered
* [Manage Rules tab](/servicemanager-user-guide/service-portfolio/service-level-agreements/rules#manage-rules-tab)
* [Managing rules](/servicemanager-user-guide/service-portfolio/service-level-agreements/rules#managing-rules)
* [When are the rules evaluated?](/servicemanager-user-guide/service-portfolio/service-level-agreements/rules#when-are-the-rules-evaluated)
* [Automating service-level changes](/servicemanager-user-guide/service-portfolio/service-level-agreements/rules#automating-service-level-changes)
* [Troubleshooting service level management](/servicemanager-user-guide/service-portfolio/service-level-agreements/rules#troubleshooting-service-level-management)

## Manage Rules tab
When more than one service level has been defined within your SLA, the **Manage Rules** tab is enabled. In this tab, you can configure your rules for when each of the available service levels should be invoked.

## Managing rules
### Adding rules
**To add a rule:**
1. In the [**Manage Rules** tab](/servicemanager-user-guide/service-portfolio/service-level-agreements/rules#manage-rules-tab), click **+New Rule**.
1. Give the rule a name and fill in the following fields:
    * **Name.** The name of the rule.
    * **Service Level.** The service level to to be invoked should the conditions of this rule be met.
    * **All.** Configure one or more conditions, all of which must match in order for the rule to be met and the defined service level to be invoked.
    * **Any.** Configure one or more conditions where any of the the conditions can match, in addition to any "All must match" conditions, in order for the rule to be met and the defined service level to be invoked.

### Configuring rule conditions
**To configure rule conditions:**
1. In the [**Manage Rules** tab](/servicemanager-user-guide/service-portfolio/service-level-agreements/rules#manage-rules-tab), in your list of rules, click the rule you want to add conditions to.
1. In the Create/Edit Rule dialog, click **+Add Condition**.
1. Choose one of the available condition parameters.
1. Choose whether the condition for the parameter is looking for a match on *Is* or *Is not*.
1. Add one or more values against the condition parameter.
1. Repeat the above for any additional conditions you wish to set against the rule.
1. Click **Create** when finished configuring the conditions for the rule.

### Managing the order in which rules are evaluated
You can define multiple rules per SLA. When a request is raised using the SLA, the system logic will start by evaluating the first rule in the list looking for a match. If no match is found with the first rule, it will evaluate the remaining rules in list order until the first rules match is found.

If no rules are matched, then no service level will be used or invoked on the request.

You can change the order of the rules in your rules list.

**To reorder the rules in the list:**
1. Click the up and down arrows at the end of each rule's row in the list.
    ::: note 
    The up and down arrows are visible only when more than one rule has been configured against the SLA.
    :::

### Editing and deleting rules
1. In the rules list, click the row of the rule you wish to edit or delete.
1. In the Edit Rule dialog, make changes and click **Save**, or click **Delete**.

## When are the rules evaluated?
Once you have created your rules that will determine when a particular SLA and service levels will be invoked, it is useful to understand when the Service Manager application will evaluate your rules, and how this takes place.

The trigger that invokes a SLA and thus sets a service level against a request is performed via a Hornbill workflow. Without a workflow, service level management cannot be applied to the request. More specifically, the trigger occurs when the Business Process Manager reaches a node involved with the starting of a timer --- either the *Start response* or *Start resolution* timer node.

The high-level steps are as follows:
1. The request is logged and a BPM is successfully initiated.
1. The BPM reaches either the *Start response* or *Start resolution* timer node. (This is an automated operation and is represented by a blue node in your workflow).

The application logic then takes over and performs the following:
1. Checks the service against which the request is logged.
1. If there are multiple SLAs associated to the service, the application first evaluates the SLA rules and determine which SLA should be invoked. If there is only one SLA associated to the service, this one will be chosen.
1. The application logic then focuses on the SLA that has been identified, and works through the service-level rules. Once a rule that contains matching conditions is found, service level targets are set against the request.

### Update via workflow request
As part of your BPM workflow, you can request an update to the SLA at set points. This is done as part of the *Update Request* operation when you select a service level.

### Manual evaluation on a request
On a request, you can select the listed SLA and view the available SLAs for this request.

## Automating service-level changes
If you prefer that service levels are automatically updated, then enable the application setting `guest.app.view.ITSM.serviceDesk.slm.enableAutomatedSLChanges`.

When any of the following is changed on a request, the service level rules will be re-assessed automatically.
* Customer
* Company
* Team
* Site
* Priority
* Category

## Troubleshooting service level management

**Why has my request failed to have targets initiated?**

If you've configured your SLAs and service levels, but continue to find some or all of your requests fail to have targets initiated, there are a few things you can check:

* Does the request have an active workflow? (This is usually indicated by the presence of the green heads-up display at the top of a request.)
* Does the service have an SLA associated to it?
* If there is more than one SLA associated, have rules been created to determine which SLA should be used?
* If an SLA is associated to the request, but no targets are set, check that you have configured rules against each service level within your SLA.
* Check that you have appropriate conditions defined for each rule.
* If you have rules configured, but still the SLA and/or service-level targets fail to be set, ensure that the criteria being used to set the appropriate SLA, and also the service level, is present on the request before the BPM reaches the node responsible for triggering the evaluation of the rules. For example, if the triggering of an SLA is dependent on the priority being established, ensure the request has a priority set before triggering the evaluation of the service-level rules. This may mean the location of the node(s) has to be considered in the BPM, or perhaps you need to use a relevant *Suspend* node.

**What happens if I change something in a request? Will the SLA and service level targets be updated?**

By default, the changing of the service level following a change in any of the criteria governing the response or fix targets is a manual action. For example, if your service levels are based on the priority, and the priority is changed, the service level must also be changed in a separate action. A service level can be amended by clicking on the name of the service level located in the request information area on the right-hand side of the request.

::: note 
In order to amend a service level, a user must have one of the following roles: [Service Request Full Access](/servicemanager-config/setup/service-manager-roles#service-request-roles), [Incident Management Full Access](/servicemanager-config/setup/service-manager-roles#incident-management-roles), [Problem Management Full Access](/servicemanager-config/setup/service-manager-roles#problem-management-roles), or [Change Management Full Access](/servicemanager-config/setup/service-manager-roles#change-management-roles).

Having the [Service Desk Admin](/servicemanager-config/setup/service-manager-roles#administration-roles) role also allows the user to amend the service level.
:::

<!-- https://wiki.hornbill.com/index.php?title=Service_Level_Rules_Builder -->