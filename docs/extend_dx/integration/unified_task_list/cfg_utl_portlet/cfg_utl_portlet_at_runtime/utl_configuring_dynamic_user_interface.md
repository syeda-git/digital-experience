# Configuring dynamic user interface

Create a dynamic page and register it using the ConfigEngine.

1.  Create a page, give it a unique ID, such as wps.utl, and place the Unified Task List portlet on the new page.

2.  Create the dynamic page template and give it a unique ID. Make sure that the page is set to inherit parent theme in the page options.

3.  Open a command prompt.

4.  Change to the IBM\WebSphere\wp_profile\ConfigEngine directory.

5.  Enable the Unified Task List portlet page to start dynamic pages by running the following command:

    -   AIX® and Linux™: `./ConfigEngine.sh action-enable-page-as-extension-node-wp.dynamicui.config -DPageUniqueName=wps.utl`
    -   Windows™: `ConfigEngine.bat action-enable-page-as-extension-node-wp.dynamicui.config -DPageUniqueName=wps.utl`

    Where -DPageUniqueName is the value of the unique ID you previously specified.



