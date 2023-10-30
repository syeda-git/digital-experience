# Configuration Wizard runtime properties

The Configuration Wizard reads a properties file at startup. You can change these values and restart the wizard to control runtime behaviors.

The properties file is found here: `AppServer/profiles/cw_profile/installedApps/*your_node_cellname*/wizard.ear/wizard.war/display.properties`. All property changes require a restart of server1 before they take effect.

The following actions are supported:

-   **Run the wizard in non-execution mode**

    It is possible to run the wizard in a non-execution mode. The instance is created and the wizard proceeds through the steps. However, no commands are run. This method is useful with the printDebug parameter to debug issues. It is also useful to create the custom data that is used to run the wizard silently. Set the value to false to enable this mode.

-   **Enable tracing**

    To enable tracing, add the printDebug parameter to the display.properties file. Set the value to true.



