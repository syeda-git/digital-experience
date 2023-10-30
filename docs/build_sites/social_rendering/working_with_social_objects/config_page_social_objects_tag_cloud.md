# Configuring a page with lists of social objects for Tag Cloud support

Learn how to enable Tag Cloud portlet support on your portal page. You can enable Tag Cloud support if you are using a default portal theme profile or a custom portal theme profile.

-   If you are using default portal theme profiles within your portal installation, complete the following steps to enable Tag Cloud portlet support on your portal page:

    1.  Locate the page in the Manage pages portlet.

    2.  Click **Edit Page Properties** for the specific page.

    3.  Click **Advanced options**.

    4.  Click **I want to set parameters**.

    5.  Add the new parameter resourceaggregation.profile with the value set as the profile override for the specific page.

        For example, `profiles/profile_search_tag.json`.

        !!! note
            The search\_tag theme profile is a hidden profile, therefore it cannot be selected in the theme profile drop-down list. This profile needs to be set manually.

    6.  Click **Add**.

    7.  Click **OK** to save the new parameter.

    8.  Click **OK** to save your changes to the page properties.

-   If you are using a custom theme, complete the following steps to enable Tag Cloud support on your portal page:

    1.  Verify that your page inherits the default portal theme or a custom theme that supports the default theme profiles.

    2.  Locate the theme profile definition file by using WebDAV. For more information about accessing theme profile definition files, see *Profile schema definition* in the related links.

    3.  Open your theme profile JSON file and add the following lines to the `moduleIDs` JSON array:

        !!! note 
            If one or more of the following theme modules are already in the list of `moduleIDs`, you do not have to add them again.

        -   `wp_pagebuilder_ui`
        -   `wp_tagging_rating_tagcloud`
        -   `dojo`
    4.  Save your changes and restart your portal server.




???+ info "Related information"
    - [Profile schema definition](../../themes_skins/the_module_framework/writing_module/themeopt_mod_pro_def.md)
    - [Using the portal Tag Cloud with lists of social objects](../working_with_social_objects/using_portal_tagcloud_with_social_objects/index.md)


