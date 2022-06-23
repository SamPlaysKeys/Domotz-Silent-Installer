# Domotz-Silent-Installer

This will install the Domotz agent on an endpoint without any popups or notifications. 

Important: There is a 5 minute wait as the install runs, in order to give as much time as possible in the case of slow computers. This was the shortest time I could use that still worked for the many machines we tested on. However, this can be adjusted in the script,  by adjusting the "Start-Sleep" value in line 53.

The $apiendpoint and $activationkey variables should be filled with the relevant data from your Domotz install page. If you do not know where this information is, you can reach out to Domotz technical support for assistance.


This installer was originally designed to be run through the SyncroRMM Script deployment/automation.
The current Powershell script gets several of the variables from Syncro Variables that are selected when the script is run. In order to add the script manually to the RMM, you will need to add runtime variables for:

$checkversion - whether or not you want to automatically check for Windows Version compatibility
$apiendpoint - this is explained in the domotz installation guide
$activationkey - this is also from the domotz installation guide
$agentname - what you would like the name of the agent location to be, i.e. "Main Office"

NOTE: $checkversion is specifically looking for "yes" or "no" and was used with a dropdown. This could be amended to a checkbox for easier use.


I will continue working on improving the script, and releasing it as a standalone powershell script, as well as a silent or minimalist exe.
