# Domotz-Silent-Installer
This installer was originally designed to be run through the SyncroRMM Script deployment/automation.

The current Powershell script gets several of the variables from Syncro Variables that are selected when the script is run. In order to add the script manually to the RMM, you will need to add runtime variables for: $$checkversion $apiendpoint $activationkey $agentname 

I will continue working on improving the script, and releasing it as a standalone powershell script, as well as a silent or minimalist exe.
