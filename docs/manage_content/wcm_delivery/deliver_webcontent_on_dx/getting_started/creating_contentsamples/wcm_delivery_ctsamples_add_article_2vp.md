# Adding the Articles template page to a virtual portal

By default, virtual portals do not contain the Articles template page. To use the Articles template page in a virtual portal, follow the procedure given here.

1.  Syndicate the two libraries Web Content Templates 3.0 and Template Page Content 3.0 from the main portal installation to the virtual portal.

2.  To add the template page to the virtual portal, start the following portal configuration engine task:

    -   AIX® and Linux™:

        ```
        ./ConfigEngine.sh action-init-content-templating-pages
        -DVirtualPortalContext=virtual_portal_context_url
        -DWasPassword=adminpwd -DPortalAdminPwd=adminpwd
        ```

    -   Windows™:

        ```
        ConfigEngine.bat action-init-content-templating-pages
        -DVirtualPortalContext=virtual_portal_context_url
        -DWasPassword=adminpwd -DPortalAdminPwd=adminpwd
        ```

3.  To move the referenced content items into the PortalSite library, start the following portal configuration engine task:

    -   AIX and Linux:

        ```
        ./ConfigEngine.sh action-internalize-content-mappings-vp
        -DVirtualPortalContext=virtual_portal_context_url
        -DWasPassword=adminpwd -DPortalAdminPwd=adminpwd
        ```

    -   Windows:

        ```
        ConfigEngine.bat action-internalize-content-mappings-vp
        -DVirtualPortalContext=virtual_portal_context_url
        -DWasPassword=adminpwd -DPortalAdminPwd=adminpwd
        ```


After you complete these steps, the Articles template page is ready for you to use in the virtual portal.


