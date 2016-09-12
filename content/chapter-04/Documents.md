# Documents #

* Data container typically in a form of Json document 
* Often enough stores aggregated and/or de-normalized data
* Can also reflect a different representation of the data
* May store binary data, serializeable document, or legacy document instead of Json document
* Additionally to data every document may store meta-data
* CAS - compare and swap value of the document, used for optimistic concurrency control
* Expiry - expiration time 	of the document, 0 means never expires