# Configuring overlay reports

In order to activate overlay reports for your site, you need to configure some security-related settings.

To allow connections with the report provider, you need to configure the AJAX Proxy. Proceed as follows:

1.  Add the IBM® Coremetrics® Web Analytics site to the default dynamic policy.

    To do this, proceed with the following steps:

    1.  Open the WebSphere® Integrated Solutions Console.

    2.  Click **Resources > Resource Environment > Resource Environment Providers >WP ConfigService > Custom Properties > New...**.

    3.  Use the property name `wp.proxy.config.urlreplacement.default_policy.1` and the value `https://welcome.coremetrics.com/*` .

        !!!note
            If this name is already in use, increment the counter of the key wp.proxy.config.urlreplacement.default_policy .

    4.  Click **Apply**.

    5.  Click **Save**.

2.  Import the Coremetrics certificate into your server truststore.

    You can complete this step either by using the `wsadmin` command `retrieveSignerFromPort` of the `AdminTask` object, or manually as described here:

    1.  Open the WebSphere Integrated Solutions Console.

    2.  In a stand-alone enviroment: Click **Security > SSL certificate and key management > SSL Configurations > NodeDefaultSSLSettings > Key stores and certificates > NodeDefaultTrustStore > Signer certificates > Retrieve from port**.

        In a portal cluster environment: Click **Security > SSL certificate and key management > SSL Configurations > CellDefaultSSLSettings > Key stores and certificates > CellDefaultTrustStore > Signer certificates > Retrieve from port**. By alternative, you can also select each node individually and apply the following settings to each node in the cell.

    3.  Fill the fields as follows:

        -   For the host: welcome.coremetrics.com
        -   For the port: 443
        -   For the alias: coremetrics or another identifying string of your choice.

    4.  Click **Retrieve signer information**.

    5.  Click **Apply**.

    6.  Click **Save**.

3.  Store your Coremetrics user information in a credential vault slot as described under Configuring credential vaults for overlay reports.

4.  Restart the portal server for the changes to take effect.

5.  If required, configure the limit of outbound HTTP connections.

    The data for the overlay reports is retrieved through the AJAX proxy. The AJAX proxy has a configuration parameter for setting the maximum number of concurrent outbound connections. This limit also affects the number of overlay reports that can be retrieved from the Coremetrics API server concurrently. If you want to have more overlay reports retrieved, configure the limit as described under *Configuration metadata for outbound HTTP connections*.

!!!note
    Additional to the limit set by the AJAX proxy, Coremetrics also enforces a limit on the number of concurrent connections from the same host. When that limit is reached, the portal displays message EJQGB0000E instead of the overlay report. In this case the user can refresh the portal page until the error message disappears; the successful analytics results are cached in the browser.


???+ info "Related information"  
    -   [Configuration metadata for outbound HTTP connections](../../../../../../extend_dx/portlets_development/web2_ui/outbound_http_connection/cfg_outbound_http_connections/xml_format_outbound_http/desc_outbound_http_cfg_script/outbhttp_cfg_script_metadata.md)

