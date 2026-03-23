---
layout: article-toc
---
# Reports
You can run in-app reports in Hornbill Service Manager to gather and review operational data from the system in order to understand service performance and activity. In-app report categories include *Performance*, *Productivity*, *Satisfaction*, and *Analytics*. Example in-app reports include *Open Requests by Age*, *Average Rating by Service*, and many others.

You access in-app reports in **Service Management > Reports**. From here, you can find default reports and run them. You can create custom versions of the default reports, focusing on system entities you choose and applying filters to extract the relevant data.

You can download, schedule, and print reports.

For information about configuring reports in Hornbill, Hornbill admins should read [the configuration documentation](/esp-config/reporting/reports).

## Access
To access in-app reports in Service Manager, your user account must have one of the following roles associated.

|Role|Description|
|-|-|
|Service Manager In-App Reporting |This role provides access to the Reports feature in Service Manager.|
|Reporting User|This Platform role grants the ability to view reporting, as well as preview and run reports.|

## Create in-app reports

The in-app reports within Service Manager are pre-made standard industry reports defined by Service Desk Institute. In addition to creating reports [from a view](/servicemanager-user-guide/request-list/views), you can build reports from the in-app reports page.

1.	Go to **Service Management > Reports**.
2.	Above the reports list, select one of the in-app report categories, for example, **Performance**.
3.	In the reports list for your selected category, find an in-app report to view, for example, **Average Incident Resolution time by Service Level**.
    ::: note
    If an in-app report has been customized previously, you can select a customized version of that report from the Custom Reports column.
    :::
4.	Select the **Run** button to execute the report.
5.	(Optional) To download the report, select the **Download PDF** button.
6.	(Optional) To print the report, select **Print**.
7.	(Optional) To add the report to your favorites, select the heart icon.

## Customize in-app reports

1. Go to **Service Management > Reports**.
1. Above the reports list, select an in-app report category.
1. In the reports list, select an in-app report.
1. Next to **Custom Reports**, select **Create Customized Report** (the plus sign).
1. Give the custom report a name.
1. (Optional) If you want to base the custom report on a view of data that has already been created in your system, you can select the view in the **Load Criteria from View** dropdown.
1. Configure the ordering and grouping of results.
    1. In the Columns tab (if it exists for this report type), select the columns you want to report on.
    1. In the Criteria tab, specify the filtering conditions to filter your data as needed:
        1. Select **+ Add Condition**.
        1. Set the condition, then repeat to add more conditions as necessary.
1. (Optional) To run the report once, select **Run Once**. 
    ::: note
    If you choose this option, the report is not saved to the reports lists in the Reports page (**Recent Reports** and **My Saved Reports**).
1. Select **Create**. After creating, the report runs automatically and is listed in its in-app reports group for future reuse.

For an example of customizing an in-app report for trend analysis of common request types, see [this how-to guide](/hornbill-how-to-guides/create-custom-report-trend-analysis-common-request-types).
