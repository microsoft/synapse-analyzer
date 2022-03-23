# Using Power BI Template (.pbit) for Synapse Best Practice Report

You can install and use this tool in the following two ways.

1. If you have Power BI Service portal access, with a Power BI Pro license, you can search in the Power BI App marketplace and install it through a Power BI template app.

2. If you do not have access to Power BI service or do not use Power BI then you can download  Power BI template file (*.pbit) from this location. You can then use this pbit file through Power BI desktop (latest build) to install and run report.

Below explains steps to install and run this report using Power BI template file (.pbit) from this location.

## Prerequisite
1. Latest version of Power BI Desktop App from [Microsoft Store](https://aka.ms/pbidesktopstore "Microsoft Store") on your PC.
2. Sysadmin privileges are required to capture information from Synapse dedicated pool. The person setting up refresh, and the credentials used for refresh, should have admin rights on Synapse Dedicated pool and its databases.

## Installation
1. IF not already done, install latest version of Power BI Desktop (Feb-2022 or greater).

![Install Power BI Desktop](./img/Install-Power-BI-Desktop.png "Install Power BI Desktop")

2. Open Power BI Desktop on your PC,  
3. It will prompt you for Get Data screen. You can click on Open other reports link

![Open Other Reports](./img/Open-Other-Reports.png "Open Other Reports")

4. Change file type from pbix to pbit (1)
5. Select “Synapse Best Practice Report.pbit” template file provided (2)

![Browse select pbit file](./img/Browse-select-pbit-file.png "Browse select pbit file")

6. Click open (3)
7. Dialogue box for Synapse Best Practice report will open

![Provide connection parameters SQL endpoint database](./img/Provide-connection-parameters-SQLendpoint-database.png "Provide connection parameters SQL endpoint database")

8. Provide Synapse Dedicated Pool Endpoint (1) and Database Name (2) in the parameter text boxes
9. Click Load to open report (3)
10. If you are opening it for the first time it will pop up security warnings. This is because most of the data is collected using native database queries against DMVs. You need to allow each one permission to run by hitting 'Run' on the popup. Like an example below

![Native database query warning](./img/Native-database-query-warning.png "Native database query warning")

11. Click “Try Again” to allow it to connect to Synapse Endpoint through Native Query.
12. This should start the refresh process.

![Refresh starts](./img/Refresh-starts.png "Refresh starts")

13. Once refresh is complete click OK
