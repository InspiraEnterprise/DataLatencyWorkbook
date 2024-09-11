# Data-Latency-Workbook-
Building a custom Sentinel Workbook to get an overview of data latency in log sources 

# Description
The Latency Details workbook offers a comprehensive view of latency across data connectors and log sources. It shows the timestamp of the last data received and calculates the time elapsed since the last ingestion for each data source, covering both Windows and Linux machines, enabling efficient monitoring and troubleshooting of data flow.
 
# Business Requirements
•  Timely Detection of Data Ingestion Issues: The workbook provides real-time insights into latency across data connectors and log sources, enabling prompt identification of any delays or failures in log ingestion to prevent potential security risks.
•  Comprehensive Monitoring Across Environments: It offers detailed visibility into both Windows and Linux environments, showing the last received logs and time differences for each data source, ensuring complete monitoring across diverse platforms.
•  Actionable Reporting and Alerts: The workbook generates clear, actionable reports, allowing security teams to quickly address latency issues. Automated alerts can be configured based on latency thresholds, supporting proactive incident response.
 
# Prerequisites
•	An active Azure subscription
•	Contributor RBAC role assigned to a development resource group
•	An active Sentinel workspace
•	A Log Analytics workspace linked to Sentinel
•	Basic Required Tables (Syslog, Events, Security Events, Azure Activity) 
 
# Setup Guide
The following provides step-by-step instructions to deploy the Workbook:
 
**Step 1: Access Microsoft Sentinel**
 
• Sign in to the Azure portal: https://portal.azure.com.
• In the search bar, type Microsoft Sentinel and click on it from the results.
• Select the appropriate Sentinel workspace where you want to deploy the custom workbook.
**Step 2: Navigate to the Workbooks Section**
 
• Once in the Sentinel workspace, on the left-hand panel, scroll down and click on Workbooks under the Threat Management section.
**Step 3: Create a New Workbook**
 
• At the top of the Workbooks page, click on the + New button to start creating a custom workbook.
• You’ll now see the workbook editor interface, where you can start designing your custom workbook.
**Step 4: Import a Custom Workbook Template**
 
• If you already have a custom workbook template in JSON format, click on the "Advanced Settings" gear icon (⚙️) in the top right corner of the workbook editor.
• In the menu, choose "Edit as Code".
• Copy your custom workbook JSON code and paste it into the code editor.
• Click Apply to load the template into the workbook.
**Step 5: Save the Workbook**
 
• Once your custom workbook is ready, click Save at the top of the page.
• Provide a name and description for your workbook.
• Select Save to Microsoft Sentinel or My Workbooks to choose the visibility of the workbook. Saving it to Sentinel will make it available to all users in the workspace.
 
# Solution Insights: Workbook Visuals

![image](https://github.com/user-attachments/assets/694983a4-a899-4552-afee-4f0e4b592715)
