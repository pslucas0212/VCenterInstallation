# VCenter Sever Appliance Installation Notes

### Pre-Req
1. DNS must be configured and all host VWMare Cluster members need a FQDN
2.


### Installation Steps
1. Download and Mount VCSA ISO
2. Copy ova from mounted ISO to EXSI datastore
  - The VCenter OVA file is found under the /vsca folder.  The name will be something like VMWare-VCenter-Server-Appliance-6.7.0.xxxxxx.ova
3. On the EXSi console, chose to Create/Register a VM.  Follow the VM creation wizard steps.  Chose the default settings until you get to step 6 in the wizard.  Note: you will point to a local copy of the OVA file and upload also via the wizard.
