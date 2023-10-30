# Creating the analytics tag root label

If you use site analytics on your migrated HCL Digital Experience, you need to create the analytics tag root label.

To do this, proceed as follows in the newly migrated environment:

1.  Change to the following directory that contains the HCL Digital Experience tools:

    -   AIX® and Linux™: PortalServer_root/bin
    -   Windows™: PortalServer_root\bin

2.  Create the analytics tag root label by running the following command:

    -   AIX and Linux:

        ```
        ./xmlaccess.sh 
        -url http://example\_server.com:port/wps/config
        -user wpsadmin -password wpsadminpwd 
        -in [PortalServer\_root](../reference/wpsdirstr.md#wp_root)/base/wp.asa.server.impl/config/templates/create_asa_tag_root.xml
        -out results.xml
        
        ```

    -   Windows:

        ```
        xmlaccess.bat 
        -url http://example\_server.com:port\wps\config
        -user wpsadmin -password wpsadminpwd 
        -in [PortalServer\_root](../reference/wpsdirstr.md#wp_root)\base\wp.asa.server.impl\config\templates\create_asa_tag_root.xml
        -out results.xml
        
        ```

    As an alternative, you can also use the portal administration portlet **Import XML** to perform this import.

3.  After the request has been processed, make sure that the import process has returned the following message:

    `<status element="all" result="ok">`


Your site analytics tags are now ready for you to work.


