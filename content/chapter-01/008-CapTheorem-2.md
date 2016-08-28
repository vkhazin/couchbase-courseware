# CAP theorem and beyond#

## Pick two out of three ##
* Consistency - all nodes see all the data at the same time
* Availability - any node can execute read/write operations
* Partition tolerance - cluster continues to operate despite node(s) failure

## Realistic choices ##
* CP - Consistency/Partition Tolerance: wait for a response from the partitioned node which could result in a timeout error
* AP - Availability/Partition Tolerance: get the most recent version of the data possibly stale data
* Understanding the trade-offs available to you is the key to success
