
# Wide Column Databases - cont'd#

## Contrast to Rdbms ##
* Wide column stores also called extensible record stores
* Store data in records with an ability to hold very large numbers of dynamic columns
* Column names as well as the record keys are not fixed, and since a record can have billions of columns
* Share the characteristics of document schema-free however implementation is different
* Cassandra also supports collections as a column data type
* Good fit for: massive write load, need to always write to db, truly large volumes of data (hundreds of terabytes)
