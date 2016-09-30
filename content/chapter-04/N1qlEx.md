# N1QL Exercise #

* Login into your virtual environment, wake it up if required 
* Connect to your single node cluster user terminal window:
```
/opt/couchbase/bin/cbq -u Administrator -p WhoNeedsSecurity
```
* Execute your first N1QL query:
```
select * from `beer-sample` limit 5; <enter>
```
* Results shown are for 'limit 1':
```
{
    "requestID": "857531e2-aa68-4a7f-894e-b242f9d0b804",
    "signature": {
        "*": "*"
    },
    "results": [
        {
            "beer-sample": {
                "address": [
                    "563 Second Street"
                ],
                "city": "San Francisco",
                "code": "94107",
                "country": "United States",
                "description": "The 21st Amendment Brewery offers a variety of award winning house made brews and American grilled cuisine in a comfortable loft li
ke setting. Join us before and after Giants baseball games in our outdoor beer garden. A great location for functions and parties in our semi-private Brewers Loft.
 See you soon at the 21A!",
                "geo": {
                    "accuracy": "ROOFTOP",
                    "lat": 37.7825,
                    "lon": -122.393
                },
                "name": "21st Amendment Brewery Cafe",
                "phone": "1-415-369-0900",
                "state": "California",
                "type": "brewery",
                "updated": "2010-10-24 13:54:07",
                "website": "http://www.21st-amendment.com/"
            }
        }
    ],
    "status": "success",
    "metrics": {
        "elapsedTime": "27.592626ms",
        "executionTime": "27.564695ms",
        "resultCount": 1,
        "resultSize": 1055
    }
}
cbq>
```
* Now experiment with composing different queries with where clause, e.g.:
```
WHERE type = "brewery"
```
* Add a order clause e.g.:
```
ORDER BY state, type
```
* Select a nested value e.g.:
```
SELECT address[0] FROM `beer-sample` LIMIT 1
```
* <a href="http://developer.couchbase.com/documentation/server/current/n1ql/n1ql-language-reference/from.html" target="_blank">There is also joins and there are more than one time of joins</a>