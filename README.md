# VCenter Sever Appliance Installation Notes

### Pre-Req
1. DNS must be configured and all host VWMare Cluster members need a FQDN
2.


### Installation Steps
1. Download and Mount VCSA ISO
2. Copy ova from mounted ISO to EXSI datastore
    - The VCenter OVA file is found under the /vsca folder.  The name will be something like VMWare-VCenter-Server-Appliance-6.7.0.xxxxxx.ova
3. On the EXSi console, chose to Create/Register a VM.  Follow the VM creation wizard steps.  Chose the default settings until you get to step 6 in the VM wizard.  Note: you will point to a local copy of the OVA file and upload also via the wizard.
4. Follow the following example screen shots to complete step 6 Network Configuration settings in the VM wizard.

![GitHub Logo](/images/NetworkConfiguration01.png)


5. Add SSO Configuration Password

![GitHub Logo](/images/SSOConfigPassword01.png)


6. Add System Configuration Password

![GitHub Logo](/images/SystemConfigurationPassword03.png)


7. Add Networking Properties

![GitHub Logo](/images/NNetworkingProperties04.png)


8. Start up VM
    - The VM is ready for the Set up steps when the started VM displays setup URL which point to the VCenter URL you specified in step 4 with a port address of 5480 -> vsca01.example.com:5480

## Setup Steps

SystemConfigurationPassword03.png	
NetworkingProperties04.png	
SSOConfigPassword01.png
