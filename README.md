# About
This script sets up an integeration between Googlesheet and Stitch so data can be directly imported from a spreadsheet to the warehouse. 

# Set up instruction
1. Check your Client ID
	1. Log into your Stitch account
	1. Check your URL, it should look like: https://app.stitchdata.com/client/103773/pipeline/connections
	1. The six digit number between client/ and /pipeline is your Clinet ID (103773 in the above example)
1. Set up integration on Stitch
	1. Create a new integration
	1. Choose Import API
	1. Give it a name
	1. Generate API token and write it down
1. Set up script in Googlesheet
	1. Open the sheet you want to set up the integration
	1. Click on the menu **tools** > **script editor**
	1. Delete default contents in the project
	1. Paste script.gs to the project
	1. Save the project
	1. Close the window
1. Set up sync in the sheet
	1. Close and reopen the sheet
	1. Wait for the script run and the dropdown menu **Stitch Import** to appear (usually takes a few seconds)
	1. Click **Stitch Import** > **Setup Spreadsheet for Push** for first time use
	1. Enter your API token, client ID and primary key
	1. By default, first row is read as headers
	1. Click **Stitch Import** > **Sync with Stitch** to sync table
1. We are done!

# Reference
Original article: https://blog.stitchdata.com/google-sheets-stitch-an-easy-way-sync-your-small-data-to-redshift-32a32ece8e0a