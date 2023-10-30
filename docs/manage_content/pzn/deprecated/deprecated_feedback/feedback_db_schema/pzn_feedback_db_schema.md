# Feedback database schema

The Feedback schema, within the Feedback database, stores data about your Web site visitors' actions. This schema is closely aligned with the Tivoli Site Analyzer schema.

Any application that can connect to a standard SQL database can make use of the data that has been logged to the Feedback database schema.

For instance, you can use the data in the Feedback database schema to:

-   Generate reports using reporting software.
-   Integrate OnLine Analytical Processing \(OLAP\) tools.
-   Create your own data integration tools.

-   **[Feedback schema tables](pzn_feedback_schema_tables.md)**  
Learn about the feedback schema tables and the fields or columns they contain.
-   **[Key value pairs](pzn_key_value_pairs.md)**  
The additional information passed by rule logging events and certain bean logging events is logged to the Feedback database in the form of key value pairs.


???+ info "Related information"
    - [FeedbackListener](../feedback_and_analytics/listeners_and_persistence/pzn_feedbacklistener.md)
    - [Reports](../feedback_analytics_cfg/pzn_reports.md)

