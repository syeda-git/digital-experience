# Analyzing user behavior by Active Site Analytics

You can collect data about user behavior in your portal and send that data to a service for analysis. For this purpose the portal provides Active Site Analytics \(ASA\).

The portal provides a rich set of page metadata as part of its themes and skins. Examples are:

-   Page title
-   Page identifier
-   Portlet title
-   Portlet identifier.

You can write scripts to retrieve the data. Such scripts are called aggregators. HCL Portal provides several sample aggregators. They are located in the `[PortalServer\_root](../reference/wpsdirstr.md#wp_root)/doc/js-samples` directory of your portal installation. You can customize these or write your own aggregators to collect page metadata and more. For the samples, refer to the topic Writing an aggregator for active site analytics.

Administrators add the aggregator scripts to pages as required. When they do this, the aggregator is injected into markup of the page the next time it is rendered. You can select the point of injection arbitrarily; for example, this can be just before the closing body tag of the HTML markup. Refer to the following flow graphic: 
![When a user clicks a portlet, the aggregator obtains the portlet ID information for Site Analytics.](../../../../../images/asa_scenario_m.jpg)

-   **[Collecting analytics data](../user_behavior_by_asa/collecting_analytics_data/index.md)**  
Before you can send data about user behavior in your portal to a service for analysis, you need to collect that data. See the following topics for information about how to do this.
-   **[Displaying overlay analytics reports](../user_behavior_by_asa/displaying_overlay_analytics_reports/index.md)**  
You can use Active Site Analytics to show graphical statistics reports about individual portal resources, such as pages or portlets. These reports are called Active Site Analytics overlay reports.
-   **[Analytics tags and site promotions](../user_behavior_by_asa/analytics_tags_site_promo/index.md)**  
To obtain further analytics information from your portal, you can use analytics tags for your portal resources. You can also use analytics tags for site promotions.


???+ info "Related information"
    - [Writing an aggregator for Active Site Analytics](../user_behavior_by_asa/collecting_analytics_data/writting_aggregator_for_asa/index.md)
    - [HCL Portal 8 Integration with IBM Digital Analytics \(Coremetrics\)](https://support.hcltech.com/csm?id=kb_article&sysparm_article=KB0074915&sys_kb_id=2742800e1bda809083cb86e9cd4bcb4a)

