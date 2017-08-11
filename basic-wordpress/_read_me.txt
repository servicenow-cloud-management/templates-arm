These templates are derived from the Wordpress catalog option and represent
simplifications to reduce the number of parameters exposed to ServiceNow.
This is done to reduce the number of variables that need to be handled by
the design as well as simplifying the user experience.

./wordpress-plus-new-network.json
Changes a few parameters into variables for convenience:
  - Added validation for the "vmDnsName" parameter
  - Added drop-down list with valid sizing
  - Created more dynamic variables to prevent duplicate naming issues

./wordpress-existing-network.json
Simplifies the process more. Make note of "variables" section to make sure
there are no conflicts or inconsistencies.
  - Before using, change to reflect the existing network in "variables"
    "virtualNetworkName" and "subnetName" 

./wordpress-chosen-network.json
  - Evolution of statically assigned networks in variables to reflect chosen
    variables as parameters. Use Dynamic Forms, Pools, and Filters to select
    from available Azure networks.
