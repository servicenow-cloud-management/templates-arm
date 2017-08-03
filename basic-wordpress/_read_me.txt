These templates are derived from the Wordpress catalog option and represent
simplifications to reduce the number of parameters exposed to ServiceNow.
This is done to reduce the number of variables that need to be handled by
the design as well as simplifying the user experience.

./wordpress-plus-new-network.json
Changes a few parameters into variables for convenience:
  - Added validation for the "vmDnsName" parameter
  - Added drop-down list with valid sizing

./wordpress-existing-network.json
Simplifies the process more. Make note of "variables" section to make sure
there are no conflicts or inconsistencies.
  - Before using, change to reflect the existing network on lines 43 and 44:
    "virtualNetworkName" and "subnetName" 
