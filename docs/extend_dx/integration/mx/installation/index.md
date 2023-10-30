# Installing HCL Volt MX Foundry to integrate with HCL Digital Experience

HCL Digital Experience (DX) can be integrated with HCL Volt MX Foundry. Both products can be installed in the same Kubernetes cluster using one Kubernetes namespace per product. Common parts of the deployments can be reused which is described [in the Configuration section](../configuration/index.md).

## Deploy HCL Digital Experience using Helm

For the deployment and installation of DX, refer to the [Deploy Container Platforms Using Helm](../../../../deployment/install/container/helm_deployment/overview.md) page of this documentation. This integration guide assumes that DX is deployed and configured successfully.

## Deploy HCL Volt MX Foundry using Helm

For the deployment and installation of MX Foundry, refer to [HCL Volt MX Documentation: Installation Guide for Volt MX Foundry Containers Helm Installation](https://opensource.hcltechsw.com/volt-mx-docs/95/docs/documentation/Foundry/voltmxfoundry_containers_helm/Content/Introduction.html).

!!! important
    HCL DX customers with entitlements to the [HCL Digital Experience Cloud Native 9.5 offering](../../../../get_started/product_overview/offerings.md) can download Volt Foundry entitlements in their Flexnet entitlement to DX Cloud Native 9.5.1, and may disregard instructions to obtain Volt Foundry entitlements in HCL Volt MX 9.5 Flexnet offerings. 
