# Exporting and importing WCM libraries

This section provides information about how to export and import WCM libraries using DXClient.

!!! note 
    WCM export and import supports the WCM JCR nodes format.

## Export WCM libraries

The `wcm-library-export` command is used to export the WCM libraries from the source server to an output location in the <working-directory>/store/ folder.

-   **Command description**

    ```
    dxclient wcm-library-export
    
    ```

-   **Help command**

    This command shows the help document about the `wcm-library-export` command:

    ```
    dxclient wcm-library-export -h
    ```

-   **Command options**

    Use this attribute to specify the user name that is required to authenticate to the server:

    ```
    -dxUsername <value>
    ```

    Use this attribute to specify the password that is required to authenticate to the server:

    ```
    -dxPassword <value>
    ```

    Use this attribute to specify the hostname of the target DX server:

    ```
    -hostname <value>
    ```

    Use this attribute to specify the port number of the `cw_profile` (for Kubernetes Environment, `dxConnectPort` is 443):

    ```
    -dxConnectPort <value>
    ```

    Use this attribute to specify the user name that is required for authenticating to the `cw_profile`:

    ```
    -dxConnectUsername <value>
    ```

    Use this attribute to specify the password that is required for authenticating to the `cw_profile`:

    ```
    -dxConnectPassword <value>
    ```

    Use this attribute to specify the user name of the DX WAS server:

    ```
    -dxWASUsername <value>
    ```

    Use this attribute to specify the password of the DX WAS server:

    ```
    -dxWASPassword <value>
    ```

    Use this attribute to specify the profile name of the DX core server:

    ```
    -dxProfileName <Profile name of the DX core server> 
    ```

    Use this attribute to specify the names of the WCM libraries of the DX core server (for example, "hello_library,demo_library"):

    ```
    -librariesName <value>
    ```

    Use this attribute to specify the export libraries. This value can be either true or false. If the value is true, then export the all libraries:

    ```
    -exportAllLibraries <value>
    ```

    Starting in CF210, use this attribute to specify the context of the virtual portal that contains the WCM Library that you want to export, if any:

    ```
    -virtualPortalContext <value>
    ```

    Log files from running the command can be found in the logs directory of the DXClient installation.

-   **Example:**

    ```
     dxclient wcm-library-export -dxProtocol <dxProtocol> -hostname <hostname> -dxPort <dxPort> -dxUsername <dxUsername> -dxPassword <dxPassword>  -hostname <hostname> -dxConnectUsername <dxConnectUsername> -dxConnectPassword <dxConnectPassword> -dxWASUsername <dxWASUsername> -dxProfileName <dxProfileName> -librariesName <librariesName> 
    ```


## Import WCM libraries

The `wcm-library-import` command is used to import the WCM libraries from the source server to the target server.

-   **Command description**

    ```
    dxclient wcm-library-import
    ```

-   **Help command**

    Use this attribute to specify the user name that is required to authenticate to the server:

    ```
    -dxUsername <value> 
    ```

    Use this attribute to specify the password that is required to authenticate to the server:

    ```
    -dxPassword <value>
    ```

    Use this attribute to specify the hostname of the target DX server:

    ```
    -hostname <value>
    ```

    Use this attribute to specify the port number of the `cw_profile` (for Kubernetes Environment, `dxConnectPort` is 443):

    ```
    -dxConnectPort <value>
    ```

    Use this attribute to specify the user name that is required for authenticating to the `cw_profile`:

    ```
    -dxConnectUsername <value>
    ```

    Use this attribute to specify the password that is required for authenticating to `cw_profile`:

    ```
    -dxConnectPassword <value>
    ```

    Use this attribute to specify the user name of the DX WAS server:

    ```
    -dxWASUsername <value>
    ```

    Use this attribute to specify the password of the DX WAS server:

    ```
    -dxWASPassword <value>
    ```

    Use this attribute to specify the profile name of the DX core server:

    ```
    -dxProfileName <Profile name of the DX core server> 
    ```

    Use this attribute to specify the path to a zip file or folder that contains the WCM libraries:

    ```
    -libFilePath <value>
    ```

    Starting in CF210, use this attribute to specify the context of the virtual portal that contains the WCM Library that you want to import, if any:

    ```
    -virtualPortalContext <value>
    ```

    Log files from running the command can be found in the logs directory of the DXClient installation.

!!! example

    ```
    dxclient wcm-library-import -dxProtocol <dxProtocol> -hostname <hostname> -dxPort <dxPort> -dxUsername <dxUsername> -dxPassword <dxPassword>  -hostname <hostname> -dxConnectUsername <dxConnectUsername> -dxConnectPassword <dxConnectPassword> -dxWASUsername <dxWASUsername> -dxProfileName <dxProfileName> -libFilePath <libFilePath> 
    ```


## Limitations & Troubleshooting

1. The attribute `-dxConnectHostname` is deprecated in CF202 and later releases. It is recommended that you start using the replacement parameter `-hostname` starting from CF202 wherever necessary.
2. CF206 onwards, we are supporting the `zip/tar.gz` file formats to export and import WCM libraries.
3. Ensure that the size of the `zip/tar.gz` file of WCM import is not more than 256MB. This limitation will be addressed in the future release.
4. In the Kubernetes environment, import could fail because of connection timeout set in load balancer. Find troubleshooting tips [here](../troubleshooting_dxclient.md#troubleshooting-for-some-known-issues). 