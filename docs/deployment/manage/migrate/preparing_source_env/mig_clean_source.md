# Clean up your source profile

During the migration, your source profile is exported. Basically, this export copies your profile to a back up folder. To speed up the process and prevent failures, delete or move unnecessary files from the profile folder.

Delete or move the following files from your profile folder:

-   HCL Digital Experience logs files in the wp_profile_root/logs directory. Some of these log files require you to stop the HCL Portal server.
-   ConfigEngine log files in the wp_profile_root/ConfigEngine/log directory.
-   Any application .ear files that are not installed; typically saved later versions.


