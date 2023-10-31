# What's new in CF19

This HCL Digital Experience 9.5 Container Update release includes updated production releases of Digital Experience 9.5 core Portal and Web Content Manager, Content Composer, Digital Asset Management, and Experience API images. New additions include additional guidance to deploy to Google Kubernetes Engine (GKE), Hybrid deployment support, Progressive Web Application delivery, Google Analytics integration, Mobile Preview, DXClient and DXConnect tooling supporting CICD release processes, Kaltura video support, new Web Content Manager REST APIs, new HCL Digital Experience ‘How To’ videos, and more.

This site describes new features in each release. Go to the [HCL Software Support Site](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0013939&sys_kb_id=9bd40c1f1bbf5cd0534c4159cc4bcbbd#CF17){:target="_blank"} and [HCL DX Software Fix list](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0013939&sys_kb_id=519ebc84db1c341055f38d6d13961959){:target="_blank"} for the list of software fixes, including Container Update releases. 

You can access product software at [HCL Software Licensing Portal](https://www.hcltech.com/software/support/release){:target="_blank"}. See [Step-by-step guide to downloading DX products and accessing Customer Support](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0077878&sys_kb_id=2cde06a31b885494c48197d58d4bcbe2){:target="_blank"} for more information.

You can access the latest software requirements and updates that support HCL Digital Experience solutions from the HCL Support pages topic: [HCL Digital Experience V9.5, V9.0, and V8.5 detailed system requirements](https://support.hcltechsw.com/csm?id=kb_article&sysparm_article=KB0013514&sys_kb_id=17d6296a1b5df34077761fc58d4bcb03).

## Deploy HCL Digital Experience 9.5 Container to Google Kubernetes Engine (GKE)

Learn how to deploy HCL Digital Experience (DX) 9.5 CF19 and higher container release along with Ambassador to Kubernetes, as verified in [Google Kubernetes Engine (GKE)](https://console.cloud.google.com/marketplace/details/google-cloud-platform/container-engine){:target="_blank"}.

See the [Deploy HCL Digital Experience 9.5 Container to Google Kubernetes Engine (GKE)](https://help.hcltechsw.com/digital-experience/9.5/containerization/google_gke.html){:target="_blank"}<!-- (../../9.5/containerization/google_gke.md) --> topic for more information.

## Hybrid Deployment

The HCL Digital Experience 9.5 Hybrid deployment and topics deliver capability to deploy and manage HCL Digital Experience 9.5 core Portal Server and Web Content Manager services on premises, and connect to cloud native components Digital Asset Management, Content Composer, Experience API and related services in a production environment.

See the [Hybrid Deployment](https://help.hcltechsw.com/digital-experience/9.5/containerization/operator_backup_and_recovery_procedures.html){:target="_blank"}<!-- (../../9.5/containerization/hybrid_deployment.md) --> topic for more information.

## Progressive Web Application support

Develop support that adds native mobile application experience and performance to your web site using browser-based functionality.

See the [Progressive Web Application](https://help.hcltechsw.com/digital-experience/9.5/install/progressive_web_applications.html){:target="_blank"}<!-- (../../9.5/install/progressive_web_applications.md) --> topic for more information.

## Google Analytics integration

Learn how to set up integration of Digital Experience sites with Google Analytics and view the resulting web analytics tracking to assess the effectiveness of your DX site pages with end user audiences.

See the [Integrate Google Analytics with HCL Digital Experience](https://help.hcltechsw.com/digital-experience/9.5/install/integrate_google_analytics.html){:target="_blank"}<!-- (../install/integrate_google_analytics.md) --> topic for more information.

## Mobile Preview

Use the Mobile Preview simulator to view the presentation of Digital Experience site page components on select mobile devices.

See the [Mobile Preview](https://help.hcltechsw.com/digital-experience/9.5/install/mobile_preview.html){:target="_blank"}<!-- (../../9.5/install/mobile_preview.md) --> topic for more information.

## DXClient and DXConnect tooling supporting CICD release processes

HCL Digital Experience CF19 and higher includes a DXClient toolset, and DX Connect servlet that provides developers and administrators with an approach to deploy changes or improvements to the HCL Digital Experience platform,and automate processes in the development and delivery process.

!!!note
    The DXClient tool is not supported for use with HCL DX 9.5 deployments in Red Hat OpenShift or supported Kubernetes platforms. Use of the DXClient tool with those platforms will be available in future HCL DX 9.5 update releases.

See the [DXClient and DXConnect tooling supporting CICD release processes](https://help.hcltechsw.com/digital-experience/9.5/containerization/dxclient.html) topic for more information.

## Digital Asset Management and Kaltura Integration

Learn how to configure Kaltura Video Content Management System integration to accelerate HCL Digital Asset Management rich media integration to HCL Digital Experience site pages and content.

See the [Configure DAM - Kaltura integration](https://opensource.hcltechsw.com/digital-experience/cf205/productfeatures/digital_asset_mgmt/configure_dam_kaltura/) topic for more information.

## New Digital Experience REST APIs

New HCL DX APIs are introduced with the HCL DX CF19 release:

-   [Web content image renditions interactions REST API](https://help.hcltechsw.com/digital-experience/9.5/wcm/manage_web_content_image_renditions_interactions_by_using_rest.html){:target="_blank"}<!-- (../wcm/manage_web_content_image_renditions_interactions_by_using_rest.md) -->
-   [Web Content Library Locale Query](https://help.hcltechsw.com/digital-experience/9.5/wcm/wcm_rest_crud_libraries.html#wcm_rest_crud_libraries__read_existing_library){:target="_blank"}<!-- (../wcm/wcm_rest_crud_libraries.html#wcm_rest_crud_libraries__read_existing_library) -->
-   [Workflow Comments API](https://help.hcltechsw.com/digital-experience/9.5/wcm/wcm_rest_crud_workflow.html#wcm_rest_crud_workflow__section_q5l_qw1_knb){:target="_blank"}<!-- (../wcm/wcm_rest_crud_workflow.html#wcm_rest_crud_workflow__section_q5l_qw1_knb) -->
-   [Using XML Access to export and import Digital Asset Management assets](https://help.hcltechsw.com/digital-experience/9.5/admin-system/adxmldam.html){:target="_blank"}<!-- (../../9.5/admin-system/adxmldam.md) -->

## New HCL Digital Experience ‘How To’ Videos

Take advantage of new step by step guidance for HCL Digital Experience practitioners presented in several new videos. See the following HCL Digital Experience Help Center topics:

-   [Configure the OpenLDAP container image to the HCL DX 9.5 Container Deployment](https://help.hcltechsw.com/digital-experience/9.5/containerization/configure_openldap_image.html){:target="_blank"}<!-- (../../9.5/containerization/configure_openldap_image.md) -->
-   [How to manage syndicators and subscribers](https://help.hcltechsw.com/digital-experience/9.5/panel_help/wcm_syndication.html){:target="_blank"}<!-- (../../9.5/panel_help/wcm_syndication.md) -->

<!-- ???info "Related information"
    - [Deploy HCL Digital Experience 9.5 Container to Google Kubernetes Engine \(GKE\)](../../9.5/containerization/google_gke.md)
    - [Hybrid Deployment](../../9.5/containerization/hybrid_deployment.md)
    - [Progressive Web Application](../../9.5/install/progressive_web_applications.md)
    - [Integrate Google Analytics with HCL Digital Experience](../install/integrate_google_analytics.md)
    - [Mobile Preview](../../9.5/install/mobile_preview.md)
    - [DXClient and DXConnect tooling supporting CICD release processes](../../9.5/containerization/
    - [DXClient and DXConnect tooling supporting CICD release processes](../../9.5/containerization/deploy_dx_components_using_hcl_dx_client_and_dx_connect.md)
    - [Configure DAM - Kaltura integration](https://corp.kaltura.com/video-content-management-system/)
    - [Web content image renditions interactions REST API](../wcm/manage_web_content_image_renditions_interactions_by_using_rest.md)
    - [Web Content Library Locale Query](../wcm/wcm_rest_crud_libraries.html#wcm_rest_crud_libraries__read_existing_library)
    - [Workflow Comments API](../wcm/wcm_rest_crud_workflow.html#wcm_rest_crud_workflow__section_q5l_qw1_knb)
    - [Using XML Access to export and import Digital Asset Management assets](../../9.5/admin-system/adxmldam.md)
    - [Configure the OpenLDAP container image to the HCL DX 9.5 Container Deployment](../../9.5/containerization/configure_openldap_image.md)
    - [How to manage syndicators and subscribers](../../9.5/panel_help/wcm_syndication.md)

    -->