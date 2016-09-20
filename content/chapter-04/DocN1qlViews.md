# Document, N1QL, and Views #

* Document - primarily entity stored in a database, unit of work for CRUD (create, retrieve, update, and delete) operations
* Document can store data with more structure than its equivalent row/record in Rdbms
* <a href="http://www.couchbase.com/n1ql" target="_blank">N1QL</a> - declarative query language that extends SQL for JSON:  
```
select name from `beer-sample`
```
* One or more <a href="http://developer.couchbase.com/documentation/server/current/n1ql/n1ql-language-reference/createprimaryindex.html" target="_blank">indexes</a> required:  
```
CREATE PRIMARY INDEX ON `beer-sample`
CREATE INDEX ix_beer_name ON `beer-sample`(name)
```
* Views - materialized representation of a query on documents with spatial and MapReduce support:  
```
function (doc, meta) {
	emit(doc.brewery_id, null);
}
```
* Psss: don't forget to select 'group' check-box for MapReduce grouping
* Indexes and Views are updated <a href="http://developer.couchbase.com/documentation/server/4.5/developer-guide/query-consistency.html" target="_blank">asynchronously</a>. 
