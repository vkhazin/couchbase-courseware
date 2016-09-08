# Joins in Document Store #

## Couchbase ##
* No standard, at least, for now
* Couchbase specific N1QL syntax:
~~~
select b1.name, b2.name
from beers b1
inner join breweries b2
	on keys b1.brewery_id
~~~
* beers and breweries are bucket names, not table names