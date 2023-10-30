# Using programmatic extensions for outbound HTTP connections

To extend the functions of an outbound connection, portal administrators can implement a custom outbound service filter.

For example, such access can be required in the following cases:

-   A portal administrator wants to open an outbound HTTP connection to a back end system that requires a specific HTTP request header setting.
-   A portal administrator wants to feed a third-party site analysis program with information about an outbound HTTP connection. In this case, the outbound connections service calls custom code whenever the outbound connection is opened to the specific remote site. The custom code feeds the third-party site analysis program with the information about the remote connection.

-   **[Custom outbound service filters](custom_outbound_svc_filters/index.md)**  
Custom outbound service filters provide a plug point for application developers. They can use these filters to add custom function to the processing logic of a policy.
-   **[Using custom cookie transformation handlers](using_custom_cookie_transformation_handlers/index.md)**  
You can use custom cookie transformation handlers to allow custom program extensions to get programmatic control over the outbound HTTP connection.


???+ info "Related information"
    - [Policy rules](../cfg_outbound_http_connections/cfg_structure/outbhttp_cfg_strctr_policy_rul.md)

