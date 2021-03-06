Introduction to MongoDB
On this page

Document Database
Key Features
Welcome to the MongoDB 4.2 Manual! MongoDB is a document database designed for ease of development and scaling. The Manual introduces key concepts in MongoDB, presents the query language, and provides operational and administrative considerations and procedures as well as a comprehensive reference section.

MongoDB offers both a Community and an Enterprise version of the database:

MongoDB Community is the source available and free to use edition of MongoDB.
MongoDB Enterprise is available as part of the MongoDB Enterprise Advanced subscription and includes comprehensive support for your MongoDB deployment. MongoDB Enterprise also adds enterprise-focused features such as LDAP and Kerberos support, on-disk encryption, and auditing.
Document Database
A record in MongoDB is a document, which is a data structure composed of field and value pairs. MongoDB documents are similar to JSON objects. The values of fields may include other documents, arrays, and arrays of documents.

A MongoDB document.
The advantages of using documents are:

Documents (i.e. objects) correspond to native data types in many programming languages.
Embedded documents and arrays reduce need for expensive joins.
Dynamic schema supports fluent polymorphism.
Collections/Views/On-Demand Materialized Views
MongoDB stores documents in collections. Collections are analogous to tables in relational databases.

In addition to collections, MongoDB supports:

Read-only Views (Starting in MongoDB 3.4)
On-Demand Materialized Views (Starting in MongoDB 4.2).
Key Features
High Performance
MongoDB provides high performance data persistence. In particular,

Support for embedded data models reduces I/O activity on database system.
Indexes support faster queries and can include keys from embedded documents and arrays.
Rich Query Language
MongoDB supports a rich query language to support read and write operations (CRUD) as well as:

Data Aggregation
Text Search and Geospatial Queries.
SEE ALSO

SQL to MongoDB Mapping Chart
SQL to Aggregation Mapping Chart
High Availability
MongoDB’s replication facility, called replica set, provides:

automatic failover
data redundancy.
A replica set is a group of MongoDB servers that maintain the same data set, providing redundancy and increasing data availability.

Horizontal Scalability
MongoDB provides horizontal scalability as part of its core functionality:

Sharding distributes data across a cluster of machines.
Starting in 3.4, MongoDB supports creating zones of data based on the shard key. In a balanced cluster, MongoDB directs reads and writes covered by a zone only to those shards inside the zone. See the Zones manual page for more information.
Support for Multiple Storage Engines
MongoDB supports multiple storage engines:

WiredTiger Storage Engine (including support for Encryption at Rest)
In-Memory Storage Engine.
In addition, MongoDB provides pluggable storage engine API that allows third parties to develop storage engines for MongoDB.

//Test Data
[
{
"Newspaper":"Log Angeles Times",
"Daily Circulation, 2004":983727,
"Daily Circulation":653868,
"Changes in Daily Circulation, 2004-2013":-34,
"Pulitzer Prize Winners and Finalists, 1990-2003":44,
"Pulitzer Prize Winners and Finalists, 2004-2014":41,
"Pulitzer Prize Winners and Finalists, 1990-2014":85,
},
{
"Newspaper":"Washington Post",
"Daily Circulation, 2004":983727,
"Daily Circulation":653868,
"Changes in Daily Circulation, 2004-2013":-34,
"Pulitzer Prize Winners and Finalists, 1990-2003":44,
"Pulitzer Prize Winners and Finalists, 2004-2014":41,
"Pulitzer Prize Winners and Finalists, 1990-2014":85,
},
{
"Newspaper":"Washington Post",
"Daily Circulation, 2004":983727,
"Daily Circulation":653868,
"Changes in Daily Circulation, 2004-2013":-34,
"Pulitzer Prize Winners and Finalists, 1990-2003":44,
"Pulitzer Prize Winners and Finalists, 2004-2014":41,
"Pulitzer Prize Winners and Finalists, 1990-2014":85,
},
{
"Newspaper":"Washington Post",
"Daily Circulation, 2004":983727,
"Daily Circulation":653868,
"Changes in Daily Circulation, 2004-2013":-34,
"Pulitzer Prize Winners and Finalists, 1990-2003":44,
"Pulitzer Prize Winners and Finalists, 2004-2014":41,
"Pulitzer Prize Winners and Finalists, 1990-2014":85,
},
{
"Newspaper":"Washington Post",
"Daily Circulation, 2004":983727,
"Daily Circulation":653868,
"Changes in Daily Circulation, 2004-2013":-34,
"Pulitzer Prize Winners and Finalists, 1990-2003":44,
"Pulitzer Prize Winners and Finalists, 2004-2014":41,
"Pulitzer Prize Winners and Finalists, 1990-2014":85,
}
]


------------------
MongoDB 4.2
https://www.mongodb.com/download-center/community
https://www.mongodb.com/products/compass
https://docs.mongodb.com/manual/aggregation/


