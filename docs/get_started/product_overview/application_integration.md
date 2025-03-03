---
tags:
    - Script Application
    - Portlet
    - Application Integration
    - Development
    - DXClient
    - Digital Data Connector
hide: tags
---

# Application Integration

HCL DX provides multiple ways for application developers to integrate application content into the digital experiences created with the product. In addition, our rich [forms building](forms_building.md) capabilities enable non-technical users to create rich data capture applications.

## Build with Modern Frameworks

!!! tip "New development recommendation"
    For most new applications, we recommend customers consider Script Applications first.

HCL DX enables developers to build applications for the platform using commonly available front-end development skills. The **Script Application** enables applications built with most front-end frameworks to be integrated to [sites built with HCL DX](site_building.md), including placing applications built with different frameworks on the same page. Script Applications can also be rendered alongside traditional java Portlets.

Script Applications include access to various HCL DX frameworks and APIs for content targeting, access to user login information or access to shared render parameters, Portlet preferences, and live text. Script Applications also work with HCL DX's modular theme to optimize download size.

For the business leader considering using HCL, Script Applications provide a way to access the power of HCL DX with commonly available skills.

## Protecting your Existing Investments

HCL DX enables customer who have existing investments in applications to retain those and integrate them into sites built on the platform.

### Portlets

Portlets developed using the JSR 168 or JSR 286 specifications can be hosted on HCL DX. JSF can also be used for Portlet development, with some constraints that are documented elsewhere on this site.

### Existing Web Applications

Web Application Bridge provides organizations with flexibility to integrate existing web applications. The capability provides a proxied web environment that enables presentation of external web content without requiring URL redirection or content introspection. This technology makes it easier than ever to integrate existing web applications and dynamically present content through HCL DX.

### Digital Data Connector

HCL DX provides [Digital Data Connector (DDC)](../../extend_dx/ddc/index.md), a framework to integrate live data from external data sources on your pages via [Web Content Manager](content_management.md) presentation components. DDC can be used to integrate product data from HCL Commerce or enterprise social network information from HCL Connections.

The power of Digital Data Connector is that you can use all the HCL DX content management facilities for managing your external data visualizations. This includes content syndication, version handling, workflow, and targeting. Since the presentation is managed via content management, changes to data display can be easily managed without needing development skills, and controlled via the content management workflows.

Digital Data Connector is extensible and can be used in conjunction with HCL Volt MX Foundry to gain access to a wide range of back-end services.

### HCL Connections

Integrate the power of HCL Connections with HCL Digital Experience. Choose the deployment type for your organization and follow the installation and configuration steps to integrate HCL Connections with HCL DX.

### HCL Volt MX Foundry

HCL Digital Experience can be integrated with HCL Volt MX Foundry. Both products can be installed in the same Kubernetes cluster using one Kubernetes namespace per product. 

### HCL Leap

HCL Digital Experience can be integrated with HCL Leap. Both products can be installed in the same Kubernetes cluster using the same Kubernetes namespace.

### Unified Task List

Use the Unified Task List portlet to integrate with business process solutions such as IBM Process Server, WebSphere Lombardi Edition, and other enterprise resource planning software.

### Java Connector Architecture

A portal provides access to content, data, and services that are located throughout the enterprise. These services include predefined connectors and portlets, and tools for creating additional connectors and portlets.

### IBM MobileFirst

Integrate HCL Digital Experience with MobileFirst to provide multi-channel support to your web communities.

## HCLSoftware U learning materials

For an introduction and a demo on how to use the Digital Data Connector, go to [Digital Data Connector](https://hclsoftwareu.hcltechsw.com/component/axs/?view=sso_config&id=3&forward=https%3A%2F%2Fhclsoftwareu.hcltechsw.com%2Fcourses%2Flesson%2F%3Fid%3D1451). To try it out yourself, refer to [Digital Data Connector for Beginners Lab](https://hclsoftwareu.hcltechsw.com/images/Lc4sMQCcN5uxXmL13gSlsxClNTU3Mjc3NTc4MTc2/DS_Academy/DX/Developer/HDX-DEV-100_Digital_Data_Connector_for_Beginners.pdf) and corresponding [Digital Data Connector for Beginners Lab Resources](https://hclsoftwareu.hcltechsw.com/images/Lc4sMQCcN5uxXmL13gSlsxClNTU3Mjc3NTc4MTc2/DS_Academy/DX/Developer/HDX-DEV-100_Digital_Data_Connector_Lab_Resources.zip).

???+ info "Related information"
    - [Integration](../../extend_dx/integration/index.md)
