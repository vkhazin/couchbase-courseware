# Joins in Rdbms #

## Rdbms ##
* Sql - structured query language
* ANSI publishes SQL: 2011 or ISO/IEC 9075:2011 - standard for the SQL database query language
* Today's syntax:
~~~
select b1.name, b2.name
from beers b1
inner join breweries b2
	on b2.brewery_id = b1.brewery_id
~~~
* Older syntax
~~~
select b1.name, b2.name
from beers b1, breweries b2
where b2.brewery_id = b1.brewery_id
~~~
