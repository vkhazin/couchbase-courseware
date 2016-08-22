# Why NoSql Databases #


* History, hype, and industry trends
* Rdbms strengths and shortcomings - strong consistency, rich ecosystem, weak scalability and limited availability options
*  NoSql strength and weaknesses - replication and sharding built-in, high scalability and availability, limited ecosystem, eventually consistency
*  CAP theorem - pick two out of consistency, availability, and partition tolerance
*  Search Engines, Big Data, and Data Streaming - where Rdbms used to answer all needs, NoSql takes a different approach for now
*  Polyglot persistency - no more one size fits all, for different needs - different tools
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

# History, hype, and industry trends #

![Still following me](../../media/NoSqlStopFollowingMe.png)

_Image credit [@perez](https://twitter.com/perez)_
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

