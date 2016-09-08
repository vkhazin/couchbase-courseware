# De-normalization and Aggregation #

* Data duplication and de-normalization are first-class citizens
* Data is copied into multiple documents to optimize query processing
* Data volumes are increased, does it matter as much in nowadays?
* Cost of storage in 1956 - $9,200/mb, in 2016 - 0.00003/mb
* Collection of data we interact with as a unit translated into aggregation
* Domain Driven Design could have impacted the notion
* Aggregates make it easier to manage data storage over a cluster 
* Aggregation often achieved using materialized views as supported by Couchbase