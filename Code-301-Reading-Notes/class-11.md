# class-11

##  five differences between SQL and NoSQL databases:

 **SQL**                                                  |   **NoSQL**
 -----------------                                        |   --------
 Relational Databases                                     | non-relational database
 table based databases                                    |document based
 have predefined schema                                   | ave dynamic schema 
vertically scalable                                       |horizontally scalable
 databases are not best fit for hierarchical data storage | its better for the hierarchical data storage
 
 ## What kind of data is a good fit for an SQL database?
SQL databases are good fit for the complex query intensive environment 

## Which type of database is best for scalability?
* 1. MySQL Community Edition
* 2. MS-SQL Server Express Edition
* 3. Oracle Express Edition

## What kind of data is a good fit a NoSQL database?
NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.

## Which type of database is best for hierarchical data storage?
* 1.MongoDB
* 2.CouchDB
* 3.Redis

## What does SQL stand for?
for Structured Query Language and it therefore is not a database itself 
but only a query language you can use to interact with a specific type of database.

## What is a realational database?
The other important part of SQL-based databases are relations.
<br>
You split data into multiple tables so that you avoid data duplication.
Therefore, you'll have a Users, Products and Orders table but each table
will only hold data that is not stored in one of the other tables.

## What type of structure does a relational database work with?
* users
* product
* orders

## What is a ‘schema’?
Data is stored as records in tables and each table has a clearly defined structure
- a set of fields which defines which data may go into the table and which data may not.

## What is a NoSQL database?
NoSQL is named like this because it basically follows the opposite approach of SQL databases.

* No schemas
* No relations
* NoSQL databases don't know the concept of joining tables/ collections.
<br>
You can manually do that 

## How does it work?
You can manually do that (by retrieving a foreign id in collection A and looking it up in collection B) but this will not be your typical flow.
<br>
Instead, you duplicate data across collections so that each collection yields exactly the data some part of your app might be looking for.

## What is inside of a Mongo database?
data , collection , server ,database 

## Which is more flexible - SQL or MongoDB? and why.

MongoDB is a Non-relational Database while SQL is a Relational Database.
While MongoDB supports JSON querying, a SQL Database uses SQL query processing. 
The basic characteristics make MongoDB a more dynamic and complex
option that is fit for hierarchical data while a SQL Database
remains more predefined and suited for other kinds of data storage

## What is the disadvantage of a NoSQL database?
* Increased flexibility might lead you to work sloppy and postpone data structure decisions
* Duplicate data means that you have to update multiple collections and documents if that data changes - not just one record in one table as you would do it in the SQL world

