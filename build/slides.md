# Chapter One - Why NoSql Databases #

* History, hype, and industry trends
* Rdbms strengths and shortcomings - strong consistency, rich ecosystem, weak scalability and limited availability options
* NoSql strength and weaknesses - replication and sharding built-in, high scalability and availability, limited ecosystem, eventually consistency
* CAP theorem - pick two out of consistency, availability, and partition tolerance
* Search Engines, Big Data, and Data Streaming - where Rdbms used to answer all needs, NoSql has taken a different approach, for now
* Polyglot persistence - no more one size fits all, for different needs - different tools
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

# History of Databases - cont'd#

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

# CAP theorem#
![Still following me](../../media/CapTheorem.png)

---

# CAP theorem and beyond#

## Pick two out of three ##
* Consistency - all nodes see all the data at the same time
* Availability - any node can execute read/write operations
* Partition tolerance - cluster continues to operate despite node(s) failure

## Realistic choices ##
* CP - Consistency/Partition Tolerance: wait for a response from the partitioned node which could result in a timeout error
* AP - Availability/Partition Tolerance: get the most recent version of the data possibly stale data
* Understanding the trade-offs available to you is the key to success

---

# Search Engines, Big Data, and Data Streaming #

## Search Engines ##
* The search engine is arguably one of the most important inventions of the 20th century
* Search by keyword feels more natural than strict Sql syntax, especially for unstructured data
* Unstructured data source: emails, logs, social media, audio, video, images...

# Big Data - Volume, Velocity, Variety #
* IDC estimates the volume of digital data will grow 40% to 50% per year
* Every 2 minutes we generate amount of data equal to all data accumulated till year 2000
* Big data "size" is a constantly moving target ranging from a few dozen terabytes to many petabytes

# Data Streaming #
* Data generated continuously by data sources
* Data streaming send in data simultaneously
* Data is processed sequentially and incrementally on a record-by-record basis
---

# Rdbms Approach #

## Ms Sql Server ##
* Database Engine
* Analytic Services
* Reporting Services
* Integration Services
* and more...

## Oracle Database Technologies ##
* Database
* Data Mining and Warehouse
* Exdata
* Database firewall
* about 60 technologies listed <a href="http://www.oracle.com/technetwork/database/database-technologies/index.html" target="_blank">on Oracle web site</a>
---

# NoSql Approach #

## Started as a specialty offering ##
* Neo4j - relationships as a core aspect of its data model 
* CouchDB - JSON documents, access your documents and query your indexes via HTTP
* MongoDB - Building on the Best of Relational with the Innovations of NoSQL
* Cassandra - the right choice for scalability, high availability and <a href="http://techblog.netflix.com/2011/11/benchmarking-cassandra-scalability-on.html" target="_blank">linear scalability</a>
* Couchbase - document database with a distributed architecture for performance, scalability, and availability
* Solr - highly reliable and scalable distributed indexing, replication and load-balanced querying
* ElasticSearch - distributed, open source search and analytics engine, designed for horizontal scalability, reliability, and easy management
---

# NoSql Approach  - cont'd#

## Continuing as multi-purpose ##
* Elastic.co - data collection, data visualization, data security, graph, and Big Data integration
* Cassandra with DataStax - advanced indexing and search, analytics and streaming, graph support
* Couchbase - multi model, advanced querying and indexing, analytics and streaming, mobile and IoT extensions
* MongoDB - visual data exploration, streaming, integration with Tableu for reporting and BI

## Variety ##
...Oh, and there are more than <a href="http://nosql-database.org/" target="_blank">255 NoSql databases</a>
---

# Polyglot Persistence #

* Store data using multiple database technologies
* Database technology is chosen by individual applications or components of a single application
* Choice is based on the needs and requirements of the application
* Analogous to 'Polyglot Programming' - applications are using mixture of programming languages
![Polyglot Persistence](../../media/PolyglotPersistence.jpg)
---

# Cloud and NoSql #

* Private cloud, public cloud, hybrid cloud, and fog computing
* Data needs to be available in multiple geo locations - locally
* Cloud based Rdbms - close to classic Rdbms but not the same
* Azure Sql - lots of guidance and restrictions to be aware of
* Oracle Cloud Database - restrictions and guidance as well
* Aws Aurora - MySql compatible, not identical
* Aws, Azure, Google, Oracle - offer NoSql database technologies for a reason
* Lot's of DbaaS (database as a service) independent vendors, Sql and NoSql alike 
---

# Chapter One Summary #

* Reviewed history of database technologies
* Re-examined Rdbms strengths and weaknesses
* Reviewed NoSql myths and realities
* Learned to recognize NoSql design decisions and constraints
* Highlighted there is no size fits all for data persistence
* Defined how Could/Fog and NoSql are related to each other
* Feeling confused? Me too...
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

