# Application Side Joins #

* Joins are rarely supported in NoSql, Couchbase is rather an exception
* Joins are implemented during design time as oppose to query execution time
* Rdbms query time almost always mean a performance penalty
* Distributed nature of NoSql makes execution time joins even more problematic
* Embedding nested entities reduces the need for query execution time joins
* Many-to-many links typically require query execution time and are handled by application
* Data stored in multiple, possibly remote, systems requires application side joins