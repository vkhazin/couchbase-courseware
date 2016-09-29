# N1QL Exercise #

* Login into your virtual environment, wake it up if required 
* Can also query data via native framework and language integration
* One or more <a href="http://developer.couchbase.com/documentation/server/current/n1ql/n1ql-language-reference/createprimaryindex.html" target="_blank">indexes</a> required:  
```
CREATE PRIMARY INDEX ON `beer-sample`
CREATE INDEX ix_beer_name ON `beer-sample`(name)
```
* N1QL query:
```
SELECT * FROM `beer-sample` WHERE name='<beer name>'
```
* Node.js query:
```
bucket.query(couchbase.N1qlQuery.fromString("SELECT name FROM `beer-sample` WHERE name='<beer name>'"));
```
* Java query:
```
bucket.query(Query.simple("SELECT name FROM `beer-sample` WHERE category='<beer name>'"));
```
* .Net query:
```
var query = from db in bucket.Queryable<BeerSample>(bucket) where beer.name == "<beer name>"
```
* Number of <a href="http://developer.couchbase.com/documentation/server/current/tools/tools-ref.html" target="_blank">tools</a> provided for N1QL development and monitoring
