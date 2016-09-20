# Couchbase Server 4.5 #

## Course Outline ##
Develop and Operate highly scalable and agile database for modern Web, Mobile, and IoT systems.  

## Participants will learn ##
* Why and Where to use NoSql databases
* What are the Types of NoSql databases
* Data modeling with NoSql
* Why to choose Couchbase Server as document NoSql
* How to install and operate Couchbase Server in Cross Data-center Environment
* What are the tools available to build application using Java/Node.js/.Net sdk

## Prerequisites ##
* Rdbms database administration and/or development experience - create database/tables, backup/restore, and sql query familiarity
* System administration and scripting experience - yum package manager, linux shell
* Proficiency with programming or scripting languages - Java, JavaScript, .Net
* Familiarity with Restful/Soap web services
* Exposure to high availability/high performance system design

## Why NoSql Databases ##
* History, hype, and industry trends
* Rdbms strengths and shortcomings - strong consistency, rich ecosystem, weak scalability and limited availability options
* NoSql strength and weaknesses - replication and sharding built-in, high scalability and availability, limited ecosystem, eventually consistency
* CAP theorem - pick two out of consistency, availability, and partition tolerance
* Search Engines, Big Data, and Data Streaming - where Rdbms used to answer all needs, NoSql takes a different approach for now
* Polyglot persistence - no more one size fits all, for different needs - different tools
* Cloud and NoSql consideration - a different view on Rdbms, NoSql support is strong and growing

## Types of NoSql Databases ##
* Key/Value - simple read/write pattern, high availability, no query capabilities
* Document - read/write by key, query language, secondary indexes, and map reduce
* Wide Column Family - read/write by key, secondary indexes, multi-value sets as a column
* Graph - excels at storing and retrieving relationships between nodes
* Multi-Model - a combination of two or more of the above types

## Data Modeling with NoSql ##
* Group Exercise: use customer data and ask to map without fk/joins supported
* Linking - similar to Rdbms joins, familiar to data modelers, no/little query language support
* Upside down approach - model the data usage not the data storage
* De-normalization and Aggregates - duplicates and pre-processed data is Okay if not Great
* Application side joins - when reads and writes are fast data access patterns change
* Search engines do searches better, keyword searches is likely a requirement
* Map/Reduce and Data Streaming do data analysis better and Big Data is a likely target
* Group exercise: key strategy for key/value and document store

## Couchbase Server - document NoSql ##
* Couchbase as a key/value and as a document NoSql
* Architecture - cluster, nodes, buckets, documents, and views
* Exercise: setup one node cluster on linux, access Server Ui, create first document
* Document, N1QL, and Views - how it all comes together
* Exercise: populate few documents, build views, and insert/retrieve data using Admin Ui
* N1QL an equivalent to sql in Rdbms, but with some key differences
* Exercise: query data with N1QL using shell

## Couchbase Server Cluster Operation ##
* Nodes, clusters and cross data centre replication - 
* Exercise: join previously stand-alone nodes into 2 clusters
* Cross data centre replication
* Exercise: configure cross clusters data replication between 2 clusters
* Auto fail-over, Backup, and Restore
* Exercise: fail one node in cluster, backup and restore one node in a cluster

## Build application using Java/Node.js/.Net sdk ##
* Sdk object/model model - overview of one/two sdk based on customer preference
* Exercise: connect to Couchbase cluster, retrieve few documents
* Object model for read/write with fall-back to replica read
* Exercise: write a document, read a document, read a document from replica
* Object model for views
* Exercise: query couchbase using Views object model
* Object model for N1QL queries
* Exercise: query couchbase using N1QL
