# Information that the Consumer exchanges with the Producer

Before a Consumer can consume portlets from a Producer, the Consumer needs specific information about the Producer. Depending on your configuration, you might also need to provide information about your Consumer portal to the Producer.

The information that Producers and Consumers exchange includes the following items:

## WSRP service description

WSRP Consumers need technical information about the WSRP services that the Producer provides. This information is described in the Web Service Description Language (WSDL) document of the Producer. The Consumer can use the information in the WSDL document to set up communication with the Producer.

The WSDL document provides information about various aspects and properties of the Producer:

-   The WSRP services that the Producer provides
-   The WSRP interfaces that the Producer supports
-   The end-point addresses of the WSRP services.

If the WSRP Producer is an HCL Portal, then Consumers of WSRP services can access the WSDL document of the Producer at the following URL:

```
 http://producer_portal_host:producer_port/wp_contextRoot/wsdl/wsrp_service.wsdl
```

!!!note "Notes"
    1.  The host and port and the wp_contextRoot directory must match the host and port of the Producer HCL Portal installation.

    2.  If the communication with the Producer is set up to use Secure Socket Layer communication, the Consumer must use **HTTPs** to address this URL: <br> `http**s**://producer_portal_host:producer_port/wp_contextRoot/wsdl/wsrp_service.wsdl`

If the WSRP service Producer is not a HCL Portal, then the owner or administrator of the Producer portal must provide the information to the Consumer.

## WSRP interfaces

The WSRP standard defines a set of four web service interfaces. The interfaces are listed here:

-   **Service Description**

    This interface is mandatory. It provides the self-description of the Producer and a description of the available portlets.

-   **Markup**

    This interface is mandatory. It is an interface for requesting and interacting with markup fragments.

-   **Portlet Management**

    This interface is optional. It provides operations for managing the lifecycle of the hosted portlets and their persistent state.

-   **Registration**

    This interface is optional. It is not supported by the current implementation of the WSRP Producer in HCL Portal. However, the HCL Portal Consumer can handle Producers that support WSRP registration interfaces.


The Producer can provide some or all of these interfaces to the Consumers as appropriate. The Producer describes these WSRP interfaces in the Web Services Description Language (WSDL) document as described under [WSRP service description](../../../wsrp/portal_wsrp_producer/wsrp_producer_info/index.md#wsrp-service-description). The WSDL document provides general technical information about the web services that the Producer provides.

## WSRP web service configuration and user information

The Producer can use a specific security or web service configuration for the provided WSRP services. This configuration can include a specific web service security configuration. The configuration of the WSRP web services on the Consumer portal must be compatible with the web service configuration of the Producer portal. For example, the Producer might configure message authentication according to the WS-Security standard for the WSRP services. In this case, the WSRP Consumer web services must also be configured for message authentication. Depending on the actual web service configuration, the Producer and Consumer portals might have to use the same user registry.

If the Producer portal has security configured for its WSRP services, the administrator of the Producer portal must assign access permissions for the provided portlets to the users of the Consumer portal. To do so, the Producer uses Portal Access Control. In this case, the Producer must obtain the required user information from the Consumer.

## Registration information

If the Producer requires registration by the Consumer portal, the Producer must provide the required registration information to the Consumer.

## Group IDs and handles of portlets

A Consumer portal can consume a remote portlet from a Producer portal by using the XML configuration interface. In this case, the Consumer portal administrator must specify the handle and groupid of the remote portlet. Therefore, the Producer must provide this information to the Consumer.

The portlet handle and group ID are listed in the WSRP service description of the Producer. The portlet handle for each portlet that the Producer provides is listed in a `portletHandle` tag. The group ID for each portlet that the Producer provides is listed in the `groupID` tag of the service description.

???+ info "Related information"  
    -   [How Producer and Consumer portals communicate](../../../wsrp/learning_wsrp/wsrpc_comint.md)

