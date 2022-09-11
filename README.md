# apigee-devlopment-2022
Stop/start order
The order of stopping and starting the subsystems is important. Start and stop scripts are provided that take care of that for you for Edge components running on the same node.

Stop order
If you install Edge on multiple nodes, then you should stop Edge components on those nodes in the following stop order:

1) Management Server (edge-management-server)
2) Message Processor (edge-message-processor)
3) Postgres Server (edge-postgres-server)
4) Qpid Server (edge-qpid-server)
5) Router (edge-router)
6) Edge UI (edge-ui)
7) Cassandra (apigee-cassandra)
8) OpenLDAP (apigee-openldap)
9) PostgreSQL database (apigee-postgresql)
10) Qpidd (apigee-qpidd)
11) ZooKeeper (apigee-zookeeper)

Start order
If you install Edge on multiple nodes, then you should start Edge components on those nodes in the following start order:

1) Cassandra (apigee-cassandra)
2) OpenLDAP (apigee-openldap)
3) PostgreSQL database (apigee-postgresql)
4) Qpidd (apigee-qpidd)
5) ZooKeeper (apigee-zookeeper)
6) Management Server (edge-management-server)
7) Message Processor (edge-message-processor)
8) Postgres Server (edge-postgres-server)
9) Qpid Server (edge-qpid-server)
10) Router (edge-router)
11) Edge UI (edge-ui)
