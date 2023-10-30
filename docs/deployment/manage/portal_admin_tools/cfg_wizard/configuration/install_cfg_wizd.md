# Installing or uninstalling the Configuration Wizard

The Configuration Wizard is installed by default when you install HCL Digital Experience. As an alternative to using the default installation, you can install the Configuration Wizard on another server that already has IBM WebSphere Application Server installed.

1.  Change to the AppServer_root/ConfigEngine directory.

2.  To install the Configuration Wizard, run the following command:

    -   AIX® and Linux™: `./ConfigEngine.sh deploy-wizard-war-standalone`
    -   Windows™: `ConfigEngine.bat deploy-wizard-war-standalone`
    
3.  To uninstall the Configuration Wizard, run the following command:

    -   AIX and Linux: `./ConfigEngine.sh remove-wizard-war-standalone`
    -   Windows: `ConfigEngine.bat remove-wizard-war-standalone`



