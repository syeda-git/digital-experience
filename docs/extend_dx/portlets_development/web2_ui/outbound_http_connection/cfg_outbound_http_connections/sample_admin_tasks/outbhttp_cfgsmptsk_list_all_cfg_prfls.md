# Listing all available configuration profiles

To create a file that contains all profiles that are registered at the outbound HTTP connection configuration, follow the procedure that is given here.

1.  Start the following portal configuration engine task:

    -   AIX® and Linux™:

        ```
        ./ConfigEngine.sh list-outbound-http-connection-profiles 
                          -DListFileName=/tmp/list.xml
        ```

    -   Windows™:

        ```
        ConfigEngine.bat  list-outbound-http-connection-profiles 
                          -DListFileName=/tmp/list.xml
        ```

    The task returns a list of all installed profiles. Example:

    ```
    profile: OutboundProfileType=system 
    profile: OutboundProfileType=global 
    profile: OutboundProfileType=scoped ApplicationScopeRef=PA_Search_Center 
    ```



