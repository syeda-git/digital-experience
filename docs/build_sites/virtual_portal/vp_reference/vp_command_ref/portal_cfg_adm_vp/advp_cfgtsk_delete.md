# Task: delete-virtual-portal

Portal ConfigEngine task that deletes a virtual portal.

Use this task to delete a virtual portal by using its object ID. To determine the correct object ID of the virtual portal, use the task `list-all-virtual-portals`.

## Parameters

-   **VirtualPortalObjectId**

    The object ID of the virtual portal. This input is mandatory for identification of the virtual portal that you want to delete.


## Syntax

You pass the parameters in the parameter list for each configuration task as appropriate. You do this by either of the following methods:

-   Specifying the parameter and value that is preceded by -D on the command line.
-   Defining them in the file wkplc.properties.

    !!! note 
        The property file must be encoded in the ISO 8859-1 character encoding format.


-   **AIX®**

    ./ConfigEngine.sh delete-virtual-portal -DPortalAdminPwd=password -DWasPassword=password -DVirtualPortalObjectId=objectID\_of\_virtual\_portal\_to\_delete

-   **Linux™**

    ./ConfigEngine.sh delete-virtual-portal -DPortalAdminPwd=password -DWasPassword=password -DVirtualPortalObjectId=objectID\_of\_virtual\_portal\_to\_delete

-   **Windows™**

    ConfigEngine.bat delete-virtual-portal -DPortalAdminPwd=password -DWasPassword=password -DVirtualPortalObjectId=objectID\_of\_virtual\_portal\_to\_delete


???+ info "Related information"
    - [Modifying a virtual portal](../../../adm_vp_task/vp_adm_task/advp_tsk_modify.md)

