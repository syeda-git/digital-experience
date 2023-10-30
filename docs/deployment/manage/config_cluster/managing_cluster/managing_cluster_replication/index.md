# Managing replication in your cluster

IBM WebSphere Application Server provides a replication service. This service transfers data, objects, or events among application servers. Data replication can be used to make data for session manager, dynamic cache, and stateful session beans available across many application servers in a cluster.

Review the following information to manage replication:

!!!note
    By default, the cluster scripts enable dynamic caching for each cluster member. The replication type is set to NOT SHARED.

-   **Dynamic caching**

    Data replication service (DRS) is the internal WebSphere® Application Server component that replicates data among application servers. There are several types of data replication, and HCL Portal can use data replication for dynamic caching and for memory-to-memory replication of session data. Enabling data replication for dynamic caching in a cluster environment is necessary to maintain data integrity between multiple HCL Portal nodes in the cluster. Replication also helps improve performance by generating data once and then replicating it to other servers in the cluster.

    -   AIX®, Linux™ and Windows™: [Dynamic cache service settings](http://www-01.ibm.com/support/knowledgecenter/SSAW57_8.5.5/com.ibm.websphere.nd.doc/ae/udyn_rcachesettings.html)

-   **Distributed sessions**

    HCL Portal can use the WebSphere® Application Server capabilities to support HTTP session failover, which enables one node in a cluster to access information from the existing HTTP session in a failure in the cluster node originally handling that session. This capability is referred to as distributed sessions. WebSphere® Application Server provides two techniques that can be used for distributed sessions, either of which can be used in a HCL Portal cluster. Distributed session support is not enabled by default, so you must determine whether to provide this capability in your cluster. And, if so, which of the two techniques you use: memory-to-memory session replication and database session persistence.

    !!!warning
        The memory-to-memory session application can lead to low memory conditions if failures cause replication to fail. This condition can occur because the local and backup sessions are stored in the JVM memory. Therefore, failures with replicating the session data can prevent freeing the memory that is allocated for the backup session.

    -   AIX®, Linux™ and Windows™:
        -   For general information, read [Session management support](https://www.ibm.com/docs/en/was/9.0.5?topic=sessions-session-management-support).
        -   For memory-to-memory information, read [Memory-to-memory replication](https://www.ibm.com/docs/en/was/9.0.5?topic=SSEQTP_9.0.5/com.ibm.websphere.nd.multiplatform.doc/ae/cprs_memory2memory.html).
        -   For database session information, read [Configuring for database session persistence](https://www.ibm.com/docs/en/was/9.0.5?topic=sessions-configuring-database-session-persistence).


