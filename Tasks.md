Possible tasks:
====

Analyse fulltext engine search traffic. Based on patterns, divide users into groups. For instance:

* **real user** - more devices used by single user (PC, tablet, mobile, ...), are identified as an independent/single user
* **autonomous** scripts (robots)
* **paranoids** - those users who purge browser's cache (delete cookies very often) or those who use browser's anonymous mode
* **specific query patterns** - during lunch, after 7 o'clock news, in the office, during weekends
* **misc** some other patterns

Identify common patterns/habits of defined groups (queries, time, domains, IP addresses, visited URL, ...)

More information:
===============

Users habits are very specific. Someone searches just in work, someone only in the evening. Some groups of users use fulltext search as a "gateway to the internet" (newspapers, social networks, ...) - that means they:
1. insert search request
2. visit result url
3. spend some time there
4. come back
5. search something else
6. leave to next result url

Same user can utilise more than one device, possibly in parallel.

IP adresses, session id nor longTermCookie can't ensure that it's one single user. Devices can be shared by family members, colleagues, coffee shop visitors or someone else.

Robots that visit Seznam's fulltext are very diverse. Some examples:

* SEO agency robots, checking their client's web position for specific search query 
* backlink attackers, searching limited set of queries or clicking to limited set of URLs
* foreign search engine robots, indexing search results from Seznam.cz

Some robots are very simple - asking same question over and over again or utilise same time window day by day. On the other hand, some robots are very smart. They randomly choose queries from huge set of possible queries, acting in the random time, clicking on random results or scroll through different pages...

You can consider to analyse mainly search queries or URL. Some queries are repeating every day (weather, facebook, ...), some queries are performed only once and never repeated again. 

Frequent phenomenons are "Internet Jumpers" - trending topics. These queries have rapidly growing occurence (gossip news, politics topics, new products anouncements, ...). The set of URLs or second level domains connected to these queries is very limited. SEO robots can have similar patterns as "trending topics" - small set of queries, often focused around client's brand or website and related microsites.


## Images

#### Attacks 1
![attacks 1](https://raw.githubusercontent.com/hackathonBI/Seznam/master/img/utok1.png)

#### Attacks 2
![attacks 2](https://raw.githubusercontent.com/hackathonBI/Seznam/master/img/utok2.png)

#### Attacks 3
![attacks 3](https://raw.githubusercontent.com/hackathonBI/Seznam/master/img/utok3.png)

#### Internet Jumpers
![internet jumpers](https://raw.githubusercontent.com/hackathonBI/Seznam/master/img/prirozeni-skokani.png)

