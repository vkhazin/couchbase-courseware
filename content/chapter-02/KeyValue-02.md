# Key-Value Databases - cont'd #

* May implement different consistency models: eventual consistency, versions, transaction consistency
* Redis and Apache Cassandra - eventually consistent
* Couchbase - strongly consistent when accessing object by key within a cluster
* In-memory only vs. disk persistence
* Memcached and Oracle Coherence - memcached does not replicate, Coherence does
* Redis and Riak - persist to disk, not always as reliably as Rdbms
* In general, key-value stores offer no query language
* Value is stored as a blob requiring no upfront data modeling or schema definition
* Scale out by implementing partitioning, replication and auto recovery
* Scale up by maintaining the database in RAM by avoiding locks, latches and low-overhead calls
* Perfect for: session management, user/profile stores, and data caching with expiry/auto-eviction functionality available
* Less than ideal for: ad-hoc data queries, reporting, dashboards