# Server Reports for SQL Operations Studio

Welcome to **Server Reports** for SQL Operations Studio! Server Reports give useful insights about the server related to performance. These can be used to see current activity as well as historical activity. Here is a list of some of the available reports.

* DB Space Usage
* DB Buffer Usage
* CPU Utilization
* Backup Growth Trend
* Wait counts

<img src="https://github.com/Microsoft/sqlopsstudio/raw/master/samples/serverReports/images/server_reports.png" alt="Server Reports" style="width:480px;"/>

This extension is inspired by SQL Server Management Studio (SSMS)'s reports. We will continually add more useful server insights and tasks.

## Building your own reports
This extension is also useful as a sample dashboard extension. It demonstrates building a dedicated dashboard extension with a set of insights built in. You can get started building your own reports by following the [extension authoring guide].

See the [Server Reports Extension Project] in the SQL Operations Studio repository on Github for the extension source code.

[Server Reports Extension Project]:https://github.com/Microsoft/sqlopsstudio/tree/master/samples/serverReports
[extension authoring guide]:https://github.com/Microsoft/sqlopsstudio/wiki/Getting-started-with-Extensibility


## Contributions and "thank you"
Special thanks to our Microsoft MVPs for providing useful queries.
*	Paul Randal:
https://www.sqlskills.com/blogs/paul/wait-statistics-or-please-tell-me-where-it-hurts/

See [Paul Randal's wait types library] for more information about each wait type in the Wait Counts widget.

[Paul Randal's wait types library]:https://www.sqlskills.com/help/waits

*	Glenn Berry: https://gallery.technet.microsoft.com/scriptcenter/All-Databases-Data-log-a36da95d

*	Aaron Bertrand: https://www.mssqltips.com/sqlservertip/2393/determine-sql-server-memory-use-by-database-and-object/


We would like to thank all our users who raised issues, and in particular the following users who helped contribute fixes:
*	flyfishingdba for Add square brackets for ms_foreachdb call (#1023)

## What's new in Server Reports v1.1?
* Fixed DB Space Usage where it threw an error when database names contain special characters
* Changed DB Space Usage and DB Buffer Usage to show only top 10 data