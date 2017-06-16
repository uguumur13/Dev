# Azure-Firewall-into-existing-environment

[<img src="http://azuredeploy.net/deploybutton.png"/>](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fkblackstone%2FDev%2Fmaster%2FAzure-1FW-3-interfaces-existing-environment-NoAS%2FAzureDeploy.json)

This template was created to support the deployment of a 4 interface Palo Alto Networks firewall into an existing Microsoft Azure environment that has the following items already deployed:

                    -VNET - with subnets
                    -Storage Account for the firewall VHD
                    -Resource Group for Firewall
            

FEATURES:
- The firewall deploys with 4 interfaces.  1 MGMT and 3 data plane into an existing environment.
- It is possible to choose the version of software the firewall is running. 7.1 or 8.0 (Latest)
- The deployment SKU can also be choosen during deployment.  BYOL, Bundle1 or Bundle2 are the available options.
- Static IP addresses assignment is used for all the firewall interfaces.


The following Storage Account types are supported:

                    -Standard_LRS
                    -Standard_GRS
                    -Standard_RAGRS
                    -Premium_LRS
                    
The following VMs are supported:

                    -Standard_DS3_v2
          			-Standard_DS4_v2
         	 		-Standard_DS5_v2
          			-Standard_D3_v2
          			-Standard_D4_v2
          			-Standard_D5_v2
          			-Standard_GS1
          			-Standard_F8s
          			-Standard_F16s
        
NOTE: Make sure the VMs are supported in the specific Storage Account Type and Azure Region.
