# Using custom cookie transformation handlers

You can use custom cookie transformation handlers to allow custom program extensions to get programmatic control over the outbound HTTP connection.

You define custom cookie transformation handlers in a cookie rule. The interface provides two methods for getting programmatic control in the following two phases of the outbound HTTP connection:

-   Before the HTTP request header is sent to the remote connection. The transformation handler receives a cookie that applies to the cookie rule.
-   After the response header is read. The transformation handler receives a cookie that was set in a `Set-Cookie` header definition.

Application developers can use a custom cookie transformation handler to modify the name, path, domain, or value of the affected cookie, or to produce analytic or statistical information about the cookie.

-   **[Implementing a custom cookie transformation filter](outbhttp_impl_cust_cookie_xform_fltr.md)**  
Application developers can implement a custom cookie transformation filter.
-   **[Registering a custom cookie transformation filter](outbhttp_reg_cust_cookie_xform_fltr.md)**  
For a custom cookie transformation filter to take effect, you must register it.


???+ info "Related information"
    - [Cookie rules](../../cfg_outbound_http_connections/cfg_structure/outbhttp_cfg_strctr_cookie_rul.md)

