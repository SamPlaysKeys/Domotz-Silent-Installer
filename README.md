# Domotz-Silent-Installer
This installer was originally designed to be run through the SyncroRMM Script deployment/automation.

The current Powershell script gets several of the variables from Syncro Variables that are selected when the script is run. In order to add the script manually to the RMM, you will need to add runtime variables for:

$checkversion - whether or not you want to automatically check for Windows Version compatibility
$apiendpoint - this is explained in the domotz installation guide
$activationkey - this is also from the domotz installation guide
$agentname - what you would like the name of the agent location to be, i.e. "Main Office"

NOTE: $checkversion is specifically looking for "yes" or "no" and was used with a dropdown. This could be amended to a checkbox for easier use.

I will continue working on improving the script, and releasing it as a standalone powershell script, as well as a silent or minimalist exe.
