# Create Documents and Views #

* Connect to the Couchbase instance we have created in the previous exercises
* Open Admin Ui be selecting 'Preview->Port 3000 Http' and adding port number 8091 in the address bar, e.g.:
```
http://couchbase-courseware-213242.nitrousapp.com:8091/
```

## Documents ##
* Select 'Data Buckets'
* Select 'Documents' next to 'beer-sample'
* Select one of the documents to edit
* Modify content and save
* Create new document

## Views ##
* Select 'Data Buckets'
* Select 'Views' next to 'beer-sample'
* Views are organized in a design document - unit of deployment
* There are development and production views
* Select 'Production Views' - review the examples
* Select 'Development Views' - create new view to list brewery id only
* Modify the newly created view to create count of documents by brewery id
* Psss: there is reduce panel on the right and there is arrow next to 'Filter Results' with 'group' check-box
* Intuitive is not it?