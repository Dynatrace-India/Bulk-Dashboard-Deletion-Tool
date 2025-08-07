## Dynatrace Dashboard Deletion Tool (v1 API)
This tool is designed to help Dynatrace admins and consultants delete dashboards in bulk based on the dashboard owner.

## Features
- Enter Dynatrace Tenant URL and API Token via GUI
- Displays real-time deletion logs in the UI
- Uses dashboard owner mapping from a local owners.txt file
- Shows progress bar
- Logs actions to logs.txt file in the root folder

## Pre-requisites
- A valid Dynatrace SaaS or Managed Tenant URL (e.g., https://abc123.live.dynatrace.com)
- A valid API Token with the following API scopes:
	- Read configuration
	- Write configuration
- owners.txt file must be present in the same folder as the tool

## owners.txt Format
Create a file named owners.txt in the tool's folder. Add one email per line for each dashboard owner whose dashboards you want to delete.

-  Example:
  - abc@gmail.com
  - bgfj@dt.com

## How to Use
- Double-click the gui_delete_dashboards.exe file to launch the tool.
- Enter your Tenant URL and API Token.
- Click “Delete Dashboards”.
- Dashboards owned by the users listed in owners.txt will be deleted.
- Progress and results will appear in the logs box and be saved to logs.txt.

## Important Notes
- Dashboards will be permanently deleted, so ensure you have a backup if needed.
- The tool skips dashboards whose owners are not listed in owners.txt.
- Avoid editing logs.txt while the tool is running.

## Developed By
Abhishek Satpathy (abhishek.satpathy@dynatrace.com)
