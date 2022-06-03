# Phocas Report Solution
Legacy Microsoft SQL Reporting Services (SSRS) reports were exported from the Phocas server to initiate this solution.

### Contents

[About this solution](#about-this-solution)<br/>
[Before you begin](#before-you-begin)<br/>
[Run this solution](#run-this-solution)<br/>
[Solution deployment](#solution-deployment)<br/>
[Disclaimers](#disclaimers)<br/>
[Related links](#related-links)<br/>


<a name=about-this-solution></a>

## About this solution

- **Applies to:** SQL Server 2016 (or higher) 
- **Key features:** Reporting Services
- **Authors:** Doug Dekker

<a name=before-you-begin></a>

## Before you begin

To run this solution, you need the following prerequisites.

**Software prerequisites:**

1. A Server with SQL Server Reporting Services 2016 (or higher) configured (https://docs.microsoft.com/en-us/sql/reporting-services/install-windows/install-reporting-services?view=sql-server-ver16)
2. Visual Studio 2019 (or higher) [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)
3. Microsoft Reporting Services Projects extension (for version of Visual Studio installed) [Microsoft Reporting Services Projects 2022](https://marketplace.visualstudio.com/items?itemName=ProBITools.MicrosoftReportProjectsforVisualStudio2022)

<a name=run-this-solution></a>

## Run this solution

<!-- Step by step instructions. Here's a few examples -->

1. Clone this repository locally.
2. Open the PhocasReportSolution.sln file at the root with Visual Studio (configured as above).
3. Select the subfolder project to maintain or add reports.

Note: Shared Data Sources and Datasets are duplicated within different projects, but will all deploy to the common /Reports/Pages/Folder.aspx?ItemPath=%2fData+Sources base (hidden) folder.

<a name=solution-deployment></a>

## Solution deployment

First open properties for the project/folder to publish. Make sure the SQL Server version matches the production server.  Finally, right-click the RDLC file to update and select Deploy. Wee [Publishing Reports to a Report Server](https://docs.microsoft.com/en-us/sql/reporting-services/reports/publishing-reports-to-a-report-server?view=sql-server-ver16) for more details.

## Related Links
<!-- Links to more articles. Remember to delete "en-us" from the link path. -->

For more information, see these articles:

-[SSRS in Visual Studio](https://www.sqlservercentral.com/articles/ssrs-in-visual-studio)
-[User Tools Option](https://docs.microsoft.com/en-us/sql/reporting-services/tools/design-reporting-services-paginated-reports-with-report-designer-ssrs?view=sql-server-ver16)