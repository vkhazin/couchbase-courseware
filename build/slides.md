# Why NoSql Databases #


* History, hype, and industry trends
* Rdbms strengths and shortcomings - strong consistency, rich ecosystem, weak scalability and limited availability options
* NoSql strength and weaknesses - replication and sharding built-in, high scalability and availability, limited ecosystem, eventually consistency
* CAP theorem - pick two out of consistency, availability, and partition tolerance
* Search Engines, Big Data, and Data Streaming - where Rdbms used to answer all needs, NoSql takes a different approach for now
* Polyglot persistency - no more one size fits all, for different needs - different tools
* Cloud and NoSql consideration - a different view on Rdbms, NoSql support is strong and growing
---

# History of Databases #

* 1960's Navigational - records are found primarily by following references from other records
    * From the era of magnetic tapes with sequential access
    * Navigational references allowed to locate next record on the tape
    * Later systems added B-trees to provide alternate access paths
    * Examples: IBM Information Management System, CODASYL - Conference/Committee on Data Systems Languages
* 1970's Relational databases - entities referencing other entities plus addition of "search" capabilities
	* Present data in tabular form, i.e. as a collection of tables with each table consisting of a set of rows and columns
	* Provided relational operators to manipulate the data in tabular form
	* Later ACID-compliant transaction processing with strong database consistency characteristics and high level of database security were introduced
	* Examples: Oracle, MS Sql Server, MySql, IBM DB2, PostgreSql.
---

# History of Databases Cont'd#

* 1990's Object-Oriented - combine database capabilities with OOP language capabilities
    * Data has been seen as objects and their attributes rather than rows and columns
    * Provided an object-oriented language (sometimes as extensions to SQL) as alternative to purely relational SQL.
    * The early commercial products were integrated with various languages e.g. GemStone - Smalltalk
    * An attempt at standardization of querying language - Object Query Language (OQL).
    * Examples: Gemstone , Gbase, ITASCA, TORNADO, and etc.
* 2000's NoSql - New Sql, Not just Sql, non relational - answer to demand for massively distributed databases with high partition tolerance.
	* Triggered by the needs of Web 2.0 companies such as Facebook, Google, and Amazon.com
	* Motivated by simplicity of design, simpler and massive "horizontal" scaling to clusters of machines and finer control over availability
	* Many compromise consistency in favor of availability, partition tolerance, and speed
	* Examples: MongoDb, Cassandra, CouchDB, Couchbase, Neo4J, and many more

---

# Rdbms strengths and shortcomings #


## Strengths ##
* Simple data structure - tables
* Limit redundancy or duplication of data
* Data inconsistencies are avoided
* Vendor independent logical data modeling
* Relatively 'standard' ad-hoc queries support using Sql
* Rich Etl and Reporting tools ecosystem

## Weaknesses
* Difficult to represent hierarchies of data and recursive queries
* Limited support for complex data types and with limited computation syntax
* Designed to run on a single server to maintain integrity of the data
* Scalability and elasticity is a huge challenge for relational databases
* Latest architectural changes only hide the underlying problem, e.g. master-slave

<p style="text-align: right;">
	<i>
		Rdbms - Relational data management system
	</i>
	<i>
		Sql - structured query language
	</i>
	<i>
		Etl - extract, transform, load
	</i>
</p>


---

# History, hype, and industry trends #

<p style="text-align: right;">
	<i>
		image credit: <a href="https://twitter.com/perez" target="_blank">@perez</a>
	</i>
</p>

![Still following me](../../media/NoSqlStopFollowingMe.png)
---

# NoSql strengths and shortcomings #


## Strengths ##
* High availability/Alway-On availability
* Horizontal scalability, hopefully linear scalability
* Cross data centers replication
* Big Data and Streaming support
* Flexibility and freedom to choose: type and vendor

## Weaknesses
* Data duplication is common
* Limited portability between NoSql vendors
* No joins, foreign keys, unions, or joins
* Limited ACID support, ACID 2.0 has been introduced

<p style="text-align: right;">
	<i>
		ACID - Atomicity, Consistency, Isolation, Durability
	</i>
	<i>
		ACID2 - Associative, Commutative, Idempotent, Distributed
	</i>
</p>

---

# CAP theorem and beyond #
![Still following me](../../media/CapTheorem.png)

---

# CAP theorem and beyond Cont'd#

## Pick two out of three ##
* Consistency - all nodes see all the data at the same time
* Availability - any node can executee read/write operations
* Partition tolerance - cluster continues to operate despite node(s) failure

## Realistic choices ##
* CP - Consistency/Partition Tolerance: wait for a response from the partitioned node which could result in a timeout error
* AP - Availability/Partition Tolerance: get the most recent version of the data possibly stale data

---

# Additional Features #

* Data encryption
* Restful api for server administration
* Spatial views
* Global secondary indexes
* Authentication and Authorization
* Ldap integration
* Auditing for administrators
---

