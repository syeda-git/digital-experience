# Database Management Systems

Configure the connection between HCL Digital Experience and your database management system. The Database Transfer configuration option in the Configuration Wizard assigns users and permissions, creates databases, obtains support for database collation, and transfers your database.

-   **[DB2: Database transfer](./dbtransfer_db2/index.md)**  
Your portal is installed with an Apache Derby database. The database that is immediately available for use is good for demonstration and portlet and theme development environments. Otherwise, you must configure portal to use a production-level database. Use the Configuration Wizard to transfer the data and configure a new database server.
-   **[IBM DB2: Database transfer](../db_mgmt_sys/dbtransfer_db2i/index.md)**  
Your portal is installed with an Apache Derby database. The database that is immediately available for use is good for demonstration and portlet and theme development environments. Otherwise, you must configure portal to use a production-level database. Use the Configuration Wizard to transfer the data and configure a new database server.
-   **[DB2 z/OS: Database transfer](../db_mgmt_sys/dbtransfer_zOS/index.md)**  
Your portal is installed with an Apache Derby database. The database that is immediately available for use is good for demonstration and portlet and theme development environments. Otherwise, you must configure portal to use a production-level database. Use the Configuration Wizard to transfer the data and configure a new database server.
-   **[SQL: Database transfer](../db_mgmt_sys/dbtransfer_sql/index.md)**  
Your portal is installed with an Apache Derby database. The database that is immediately available for use is good for demonstration and portlet and theme development environments. Otherwise, you must configure portal to use a production-level database. Use the Configuration Wizard to transfer the data and configure a new database server.
-   **[Oracle: Database transfer](../db_mgmt_sys/dbtransfer_oracle/index.md)**  
Your portal is installed with an Apache Derby database. The database that is immediately available for use is good for demonstration and portlet and theme development environments. Otherwise, you must configure portal to use a production-level database. Use the Configuration Wizard to transfer the data and configure a new database server.
-   **[Manual Steps: Database Transfer option in the Configuration Wizard](../db_mgmt_sys/dbtransfer_manual/index.md)**  
The database transfer option in the Configuration Wizard includes manual steps. Some manual steps include scripts for you or your database administrator to run. For reference only, you can see the manual steps in this section of the product documentation. Use the Configuration Wizard to complete the deployment configuration. The wizard generates specific instructions and scripts based on your unique input.
-   **[Oracle: Creating JCR table spaces (Automatic Storage Management)](../db_mgmt_sys/oracle_create_tablespaces.md)**  
If you configured your database with Automatic Storage Management, you might need to perform additional manual instructions to create JCR table spaces when you use the Database Transfer option in the Configuration Wizard. If you select the option to let the wizard create your database schemas and assign permissions, you must perform the steps in this topic after you run the setup database script.
-   **[Assigning custom table spaces](../db_mgmt_sys/custom_tablespace/index.md)**  
You cannot use the Database Transfer option in the configuration wizard to assign custom table spaces on your database server. You can perform manual steps to assign custom table spaces.
-   **[DB2: Enabling support for high availability data replication](../db_mgmt_sys/db2_hadr.md)**  
Optional: To prevent data loss on DB2, modify the JCR schema to support high availability data replication (HADR).
-   **[Connecting to existing database domains](../db_mgmt_sys/connect_domains.md)**  
View the steps to share a database domain between two separate HCL Digital Experience instances (instance1 and instance2), where instance2 is connected to an instance1 database domain.


???+ info "Related information"  
    -   [Container Staging](../../manage/container_configuration/container_staging.md)

