# N1QL - Declarative Query Language #

* One or more <a href="http://developer.couchbase.com/documentation/server/current/n1ql/n1ql-language-reference/createprimaryindex.html" target="_blank">indexes</a> required:  
```
CREATE PRIMARY INDEX ON `beer-sample`
CREATE INDEX ix_beer_name ON `beer-sample`(name)
```
