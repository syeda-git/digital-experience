# Removing UXFM dialog definitions

Remove the UX Screen Flow Manager (UXFM) dialog definitions before uninstalling UXFM. This is a required step before you uninstall UXFM.

1.  Save the following example of code as RemoveSampleCode.xml to use to remove your dialog definitions.

    ```
    <?xml version="1.0" encoding="UTF-8"?>
    <request type="update" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xsi:noNamespaceSchemaLocation="PCM_1.0.xsd">
    
        <!-- remove all dialog definitions that are currently deployed -->
        <portal action="delete">
           <dialog-set>
                <dialog name="*" />
            </dialog-set>
        </portal>
    </request>
    ```

2.  Run the following task from the wp_profile_root/PortalServer/bin directory to remove your dialog definitions:

    -   AIX® and Linux™: `./xmlaccess.sh -user userID -password password -url http://local\_host:local\_port/wps/config -in RemoveSampleCode.xml -out delete.xml`
    -   Windows™: `xmlaccess.bat -user userID -password password -url http://local\_host:local\_port/wps/config -in RemoveSampleCode.xml -out delete.xml`


???+ info "Related information"  
    -   [Syntax elements for the XML configuration interface command line](../../../portal_admin_tools/xml_config_interface/working_xml_config_interface/using_xml_config_cmd_line/cmdline_syntax/basic_xml_cmdln_syntax/adxmltsk_cmdln_sntx_elements.md)

