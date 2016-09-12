# Buckets #

* Logical groups of items used to organize, manage, and analyze the data
* Memcached type: in-memory scale-out, key-value cache, uses Least Recently Used algorithm to evict items when short on Random Access Memory (RAM)
* Couchbase type: highly-scalable, distributed data storage, with replication and cross-data center replication
* Operates through RAM, data stored in RAM and persisted to disk, asynchronously
* Configurable number of replicas per bucket, consistency level is defined by client SDK
* Live re-balancing to redistribute load between resources and nodes in a cluster