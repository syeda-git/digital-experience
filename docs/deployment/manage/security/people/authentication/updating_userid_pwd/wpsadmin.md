# Changing the HCL Digital Experience administrator password

HCL Digital Experience treats wpsadmin (the administrator) as any other user, just with more permissions granted. With a normal configuration, it is possible to change the wpsadmin or equivalent password through the user interface, just like any other user can manage their own password through the user interface. However, if the wpsadmin account is also used for more than just the administrator, then additional changes, outlined in other steps in this section, must be made to accommodate the change.

Perform the following steps to change the administrator password:

!!!note
    You can also change the Administrator password, like any other user password, using an LDAP editor.

1.  Log in to HCL Digital Experience as an administrator.

2.  Click your user ID.

3.  Complete the appropriate fields to change your password.

4.  Click **OK**.

5.  Complete the following steps to change the information stored in the **SearchAdminUser** alias:

    1.  Log in to the WebSphere® Integrated Solutions Console.

    2.  Click **Security** \> **Global security**.

    3.  Under Authentication, click **Java Authentication and Authorization Service** \> **J2C authentication data**.

    4.  Edit the **SearchAdminUser** alias.

    5.  Update the user ID and/or password to match your HCL Digital Experience administrator information.

6.  Update the user ID and password for the RunAs role mapping for the StartupCheck application.

    To do so, proceed as follows:

    1.  Log in to the WebSphere Integrated Solutions Console.

    2.  Select **Enterprise Applications** \> **StartupCheck** \> **User RunAs roles**.

    3.  Update the user ID and password for the RunAs role mapping for the StartupCheck application.

7. Update the security settings for your search collections.

    1. Go to Portal Adminstration.

    2. Select **Admistration** \> **Search** \> **Setting** \> **Search Collections**

    3. Go into each colleciion and edit the Content Source.

    4. Choose the Security tab.

    5. Update the password for the already defined security realms. 

    6. Mkde sure to click Update and then Save. 



Additionally, you should also change the password in the wkplc.properties file, located in the [wp\_profile\_root](../../../../../../guide_me/wpsdirstr.md#wp_profile_root)/ConfigEngine/properties directory.


???+ info "Related information"
    - [Applying fix packs to your portal](../../../../manage_portal_using_iim/apply_fixpacks.md)


