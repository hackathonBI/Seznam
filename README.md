# Data Description

Provided data from Seznam.cz contains search requests results in json format. RAW samples are [here](https://github.com/hackathonBI/Seznam/tree/master/sample%20data). 

Every json looks like this sample:

```
	{
	    "autocompleted": false,
	    "ip": "7c5322fddb8ed445",
	    "long_session": "8a2e2556a258d526",
	    "page": 0,
	    "query": "8bcb2593e02e650f",
	    "result": [
	        {
	            "domain": "b1fd423014701ad9",
	            "l2domain": "54007382001a4234",
	            "url": "c8a9302c5802d45d"
	        },
	        {
	            "domain": "30d47fd3f258cb52",
	            "l2domain": "f5cb1c0456bcc780",
	            "url": "532a597f86478342"
	        }
	    ],
	    "short_session": "93659c18967734aa",
	    "time": 40689465.51,
	    "wordCount": 2
	}
```

__Legend__

* **autocompleted** - request was inserted with autocomplete feature
* **ip** - client IP address
* **long_session** - long term client ID
* **page** - SERP number
* **query** - searched query
* **wordCount** - count of words in search query
* **short_session** - short term client ID (expires with browser session)
* **time** - query timestamp (can be used for sorting queries in proper order)
* **other_clicks** - timestamp of click onto any non-query result object (ads, pagination, additional query, etc...)
* **result** - field with query results
  * **domain** - full hostname (search.seznam.cz)
  * **l2domain** - level 2 domain (seznam.cz)
  * **url** - full URL
  * **clicks** - in case of click, here is

Seznam's list of business problems: [TASKS](https://github.com/hackathonBI/Seznam/blob/master/Tasks.md).