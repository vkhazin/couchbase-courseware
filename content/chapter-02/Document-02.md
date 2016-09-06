# Document Databases - cont'd #

* Store all information for a given object in a single document, and every stored document can be of different structure
* That in contrast to Rdbms where a given object may be stored across number of tables and rows
* Data duplication is common, foreign keys are often not welcome
* Document key is typically a string, such as url, file name, guid/uuid, or a random string
* Some document stores maintain a mapping, such as ElasticSeach for querying and aggregation support
* Consistency models differ by vendor/product
* Document can be updated or replaced, restful API is common
* Good fit for: rapid development, content management, catalogs, user generated content