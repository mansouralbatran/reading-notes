# SQL vs NoSQL Database Differences Explained with few Example DB

![image](https://www.thorntech.com/wp-content/uploads/2019/01/SQLvsNoSQL.jpg)
## SQL vs NoSQL: High-Level Differences

* SQL databases are primarily called as Relational Databases (RDBMS);
* SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column store
* SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.
## SQL Database Examples
1. MySQL Community Edition
MySQL database is very popular open-source database. It is generally been stacked with apache and PHP, although it can be also stacked with nginx and server side javascripting using Node js. The following are some of MySQL benefits and strengths:

Replication: By replicating MySQL database across multiple nodes the work load can be reduced heavily increasing the scalability and availability of business application
Sharding: MySQL sharding os useful when there is large no of write operations in a high traffic website. By sharding MySQL servers, the application is partitioned into multiple servers dividing the database into small chunks. As low cost servers can be deployed for this purpose, this is cost effective.
Memcached as a NoSQL API to MySQL: Memcached can be used to increase the performance of the data retrieval operations giving an advantage of NoSQL api to MySQL server.
Maturity: This database has been around for a long time and tremendous community input and testing has gone into this database making it very stable.
Wide range of Platforms and Languages: MySql is available for all major platforms like Linux, Windows, Mac, BSD and Solaris. It also has connectors to languages like Node.js, Ruby, C#, C++, C, Java, Perl, PHP and Python.
Cost effectiveness: It is open source and free.
##  CouchDB
CouchDB is also a document based NoSQL database. It stores data in form of JSON documents. The following are some of CouchDB benefits and strengths:
Schema-less: As a member of NoSQL family, it also have dynamic schema which makes it more flexible, having a form of JSON documents for storing data.
HTTP query: You can access your database documents using your web browser.
Conflict Resolution: It has automatic conflict detection which is useful while in a distributed database.
Easy Replication: Implementing replication is fairly straight forward