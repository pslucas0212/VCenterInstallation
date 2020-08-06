# VCenter Sever Appliance Installation Notes

### Pre-Req
1. DNS must be configured and all host VWMare Cluster members need a FQDN
2.


### Installation Steps
1. Download and Mount VCSA ISO
2. Copy the VCenter OVA file from the mounted ISO to EXSI datastore
    - The VCenter OVA file is found under the /vsca folder.  The name will be something like VMWare-VCenter-Server-Appliance-6.7.0.xxxxxx.ova
3. On the EXSi console, chose to Create/Register a VM.  
4. Chose "Deploy a virtual machind from a OVF or OVA file" option during Step 1. Selectation Creation TYpe in the New Virtual Machine dialog box.

![](/images/SelectCreationType.png)

5. Follow the VM creation wizard steps.  Chose the default settings until you get to step 6 in the VM wizard.  Note: you will point to a local copy of the OVA file and upload also via the wizard.  The exclamation to the right of each text field provides help for completing the information in the text field.
6. Follow the following example screen shots to complete step 6 Network Configuration settings in the VM wizard.

![GitHub Logo](/images/NetworkConfiguration01.png)


7. Add SSO Configuration Password

![GitHub Logo](/images/SSOConfigPassword01.png)


8. Add System Configuration Password

![GitHub Logo](/images/SystemConfigurationPassword03.png)


9. Add Networking Properties

![GitHub Logo](/images/NetworkingProperties04.png)


10. Start up VM
    - The VM is ready for the Set up steps when the started VM displays setup URL which point to the VCenter URL you specified in step 4 with a port address of 5480 -> https://vsca01.example.com:5480  Note: In Firefox you seem to need to add the https:// to the url.


## Setup Steps

1. Click the Setup Wizard and read the introduction.
2. Review step 2 Appliance Configuration settings. Click Next.

![GitHub Logo](/images/ApplianceConfiguration05.png)

3. Configure the SSO Configuration page.

![GitHub Logo](/images/SSOConfiguration06.png)


4. Chose your option to particpate in the CEIP on the Configure CEIP screen and click next.
5. Review the Ready to complete page and click the Finish button.

![GitHub Logo](/images/ReadyToComplete07.png)
