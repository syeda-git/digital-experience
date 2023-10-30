# Backing up the HCL Portal File System

Periodically run an automated backup procedure for the HCL Portal file system.

Prerequisites: [Completing prerequisites for backup](i_wadm_t_bkup_prereq_winlinux.md)

1.  If you are performing an online backup, go to Step 3.

2.  If you are performing an offline backup, stop all servers.

    1.  If applicable, stop all external HTTP servers.

    2.  Stop all of the HCL Portal servers.

3.  Back up all HCL Portal files and sub-directories under the directory PortalServer_root.

4.  Back up all IBM® WebSphere® Application Server files under the directory wp_profile_root to capture the complete runtime environment.

5.  Back up other WebSphere Application Server files under the directory AppServer_root.

6.  Back up the IBM Installation Manager agent data location. This location contains information about the installed offerings and fixes. For details on the default location of this directory, see Agent Data Location in the Related information section.

7.  Back up additional custom files outside of the PortalServer, profile, or AppServer directories; such as SSL certificates or shared libraries; that your HCL Portal server might use.

???+ info "Related information"
    - [Backing up and restoring Installation Manager](https://www.ibm.com/docs/en/installation-manager/1.8.5?topic=manager-backing-up-restoring-installation)
    - [Backing up IBM Installation Manager agent data and shared files for recovery with IBM Business Process Manager \(BPM\)](https://www.ibm.com/support/pages/node/727017)

