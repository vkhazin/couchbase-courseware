# Search Engines #

## Characteristics ##
* Flexible schema, not schema free per ce
* Entire document/data set is indexed
* Uses more space due to data de-normalization and indexing
* Typically no joins
* No constraints, no referential integrity, no uniqueness rules are enforced
* No transactions and so-so consistency, e.g. ElasticSearch split-brain problem
* Many are based on flexible and powerful <a href="https://lucene.apache.org/core/2_9_4/queryparsersyntax.html" target="_blank">lucene</a>: Title:Couchbase AND PublishedDate:[2016-01-01 TO 2018-01-01] AND Description:NoSql*
* Psss-psss: Couchbase is working on <a href="http://developer.couchbase.com/documentation/server/current/fts/full-text-intro.html" target="_blank">Full Text Search</a>