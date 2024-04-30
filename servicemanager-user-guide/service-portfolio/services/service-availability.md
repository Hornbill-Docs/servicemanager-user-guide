# Service Availability
Analyze Service Availability in Hornbill. As the Status changes on a Service from one state to another, information is automatically collected to provide availability metrics.

## Managing Service Status
The default position is 'No Status', this will result in no status or message being displayed, this is important when Service Status is not relevant to a Service.

The Three Status options are
* Available - Indicated by a green icon
* Impacted - indicated by an amber icon
* Unavailable - indicated by a red icon

When any of the above status's are chosen a default message will be displayed, and can be edited. Once saved the status and message will be visible to the subscribers of the service on the Service and or Customer Portals, and analysts who support the Service through the user app in the following places:
* Services List
* Request List
* Request Details
* Progressive Capture - Services Form

Supporting Messages can be seen by Hovering over the Service Status Icon.
* To Change the Status of the Service, simple select a different option from the drop down list and save.
* To remove any Status, simply select the 'No Status' option from the drop down list and save.

In the user app and the Request Details view, the Service Name will take you through to see more information about the service. The Level of information visible to you will depend on your rights to view the Service, including:
* If the Service is Open or Private these rights will be respected
* If you are the Owner, or a member of a team which supports the Service
* If you do not have Services Manager right, you will still be able to see very basic Service Details but no edit rights.

## Automatically Changing the Status of a Service
Through the business process designer it is possible to automate the changing of the status of a service using the Automated Task node and the Request > Request Service > Update Service Status option from within business processes.

## Availability Metrics
* **Mean time between failures (MTBF)**<br>The average time between instances of service unavailability
* **Mean time to repair (MTTR)**<br>The average time to restore service availability
* **Percentage Availability**<br>The percentage of time the service is available

The availability metrics can be accessed using the chart icon next to the service status. At least one change in the status is required in order to view the metrics, and two status changes are needed to show the MTBF metric.

## Data
To compliment the availability metrics a full list of all changes in the Services Status (Availability) are recorded and displayed under the Data option.

* **Status**<br>The status the Service was sat in (Available, Unavailable, Impacted)
* **From**<br>The date and time the Service was in this status
* **To**<br>The date and time the Service changed from this status
* **Duration**<br>The total time the service was in this status
* **Action**<br>Use this option to manually exclude a Status change from the overall Availability Metrics. If a status change was made in error, or testing you may wish to exclude this from the Services overall Availability Metrics.

Filter the Data list to show:
* All Records
* Included Records
* Excluded Records

## Date Range
By Default the Availability Metrics will be set to look at the previous 3 months.
* Manually alter the date range to view the Availability Metrics for any given time period.
* Use the refresh icon to return the date range to the default previous 3 month period

## SLA
By default the Availability Metrics will be based on a 247 clock, however it is possible to display the Availability Metrics based on the working days / hours of the working time calendar which underpins any SLA which is available on the Service.

Change the SLA to view the Availability Metrics for the Service based on the working hours of the SLA.

:::tip
Whilst it is possible to add custom service statuses via the servicestatus simple list, the availability metrics are only calculated on changes to the default statuses (Available, Unavailable and Impacted)
:::
<!-- https://wiki.hornbill.com/index.php?title=Service_Availability-->
<!-- https://wiki.hornbill.com/index.php?title=Service_Status -->