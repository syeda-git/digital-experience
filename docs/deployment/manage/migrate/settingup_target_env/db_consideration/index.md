# Database considerations

Depending on the type of database that you use, there might be extra considerations or tasks to complete before and after you migrate your data. Review the information that is tailored for your database type to ensure the migration process completes successfully.

-   **[Configuring transaction logging space](mig_cfg_transaction_log_space.md)**  
When you migrate from earlier versions of Portal, certain portions of the actual database migration use database transactions that can contain large volumes of data change. In order for the database to accommodate these transaction changes, the amount of space available to the database transaction logs might need to be increased.
-   **[Oracle: Disabling the auto space advisor background task](mig_pre_oracle_disableasa.md)**  
To prevent deadlocks during migration, you must complete a task to disable the Oracle background task called "Auto Space Advisor" before your run the upgrade-profile task during migration using the Configuration Wizard. After you complete migration, you can enable "Auto Space Advisor" as a post-migration task.
-   **[DB2 database migration considerations](db2_migration_consideration/index.md)**  
Database migration is one of the most time consuming portions of the migration process. If you are migrating from DB2®, review the following topics to improve the speed of the database migration process.


