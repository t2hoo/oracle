- 👋 Hi, I’m @t2hoo


# Introduction To Oracle Database :

## History of Oracle:
http://www.dba-oracle.com/t_history_oracle.htm

## What is meaning of i, g and c in Oracle Database Version: 

Larry Ellison, Bob Miner, Ed Oates and Bruce Scott founded Oracle in 1977 with an initial name as Project Oracle. Later renamed Relational Software Inc (RSI), released Oracle Database release 2, 3…8, 8i, 9i, 10g, 11g and 12c which is the latest release.

Oracle is a dominant player in Relation Database Management system competing against IBM, SQL Server and many other open source databases. Each release added some features to the database as per the industry requirements and trends.


This suffix i, g, and c actually denotes major feature introduced in Oracle Database. Internally these versions are further divided into five numeric segments (XX.X.X.X.X) separated by periods.

i – INTERNET
‘i’  stands for the INTERNET. 8i and 9i are major releases under this suffix. Oracle 8i was the first database to support internet technologies such as Java and HTTP. Oracle 9i release in 2001 added support for XML, Data Compression which increased performance.

g- GRID COMPUTING
“g’ stands for Grid Computing. 10g and 11G were major releases under this suffix. Oracle 10g introduced in 2003, with emphasis on the “g” for grid computing.


This is how Oracle Defines Grid computing in Oracle 11G.

“Grid computing turns computing into a utility, where users don’t care where the data resides, or what computer processes a request. Users request information or computation and have it delivered – as much as they want, whenever they want.

For the DBA, the grid is about resource allocation, information sharing, and high availability. Oracle Database with Real Application Clusters and Oracle Clusterware provide the infrastructure for your database grid. Automatic Storage Management provides the infrastructure for a storage grid. Oracle Enterprise Manager Grid Control provides you with the holistic management of your grid”.

c – CLOUD
“c” stands for “Cloud”. 12c is latest and major release under this suffix. As per Wikipedia,

“Cloud computing is an information technology (IT) paradigm, a model for enabling ubiquitous access to shared pools of configurable resources (such as computer networks, servers, storage, applications, and services), which can be rapidly provisioned with minimal management effort, often over the Internet”.

In addition to many new features, this new version of the Oracle Database implements a multitenant architecture, which enables the creation of pluggable databases (PDBs) in a multitenant container database (CDB).

## Support :
![Support](https://github.com/t2hoo/oracle/blob/2e349b66928ecb596f2d4c3d686e1856ed68464d/img/19c_timelines.jpg)

## 11g vs 12c :


Sr. No.	Key	Oracle 11g	Oracle 12c
1
Basic
It was released in released in 2008 and has no pluggable database
It is High performance RDbMS which is released in 2014. It is pluggable database.
2
Identity column
We can't set primary key to raise automatically
We can set primary key to rise automatically.
3
JSON type
We can't store Json directly to the column as Oracle 11g doesn't have JSON column type.
Oracle has introduced JSON column type.
4.
Cloud support
Oracle 11g doesn't have cloud services
It provides Oracle cloud services.
5.
In-memory capabilities
No in-memory capabilities
It has in-memory capabilities.


## Course Agenda : 
### What is a Table? -
A table is an arrangement of information in rows and columns containing cells that make comparing and contrasting information easier. As you can see in the following example, the data is easier to read in a table format.
### DBMS vs RDBMS
![image](https://user-images.githubusercontent.com/89846476/132714755-a4e774a4-53d0-4cfa-beb8-64ad630ba13e.png)

### What is Distributed Database? - 
In a distributed database, there are a number of databases that may be geographically distributed all over the world. A distributed DBMS manages the distributed database in a manner so that it appears as one single database to users. In the later part of the chapter, we go on to study the factors that lead to distributed databases, its advantages and disadvantages.
A distributed database is a collection of multiple interconnected databases, which are spread physically across various locations that communicate via a computer network.
### Data Models & ERM - 

#### Data Modeling
Data modeling is a technique to document a software system using diagrams and symbols. It is used to represent communication of data.

The highest level of abstraction for the data model is called the Entity Relationship Diagram (ERD). It is a graphical representation of data requirements for a database.

#### Entity Relationship Diagram
The main value of carefully constructing an ERD is that it can readily be converted into a database structure.

There are three components in ERD.

##### Entities: Number of tables you need for your database.
##### Attributes: Information such as property, facts you need to describe each table.
##### Relationships: How tables are linked together.

##### Entity
Entities are the basic objects of ERDs. These are the tables of your database. Entity are nouns and the types usually fall into five classes: concepts, locations, roles, events or things.
For example: students, courses, books, campus, employees, payment, projects.

A specific example of an entity is called an instance. Each instance becomes a record or a row in a table.
For example: the student John Smith is a record in a table called students.

##### Relationships
Relationships are the associations between the entities. Verbs often describe relationships between entities. We will use Crow's Foot Symbols to represent the relationships. Three types of relationships are discussed in this lab. If you read or hear cardinality ratios, it also refers to types of relationships.

![image](https://user-images.githubusercontent.com/89846476/132718716-2dd73850-a6e3-46cb-aff0-2b2c9d81c4bc.png)


##### One to One Relationship (1:1)
A single entity instance in one entity class is related to a single entity instance in another entity class.

For example:
Each student fills one seat and one seat is assigned to only one student.
Each professor has one office space.
One to Many Relationship (1:M)
A single entity instance in one entity class (parent) is related to multiple entity instances in another entity class (child)

For example:
One instructor can teach many courses, but one course can only be taught by one instructor.
One instructor may teach many students in one class, but all the students have one instructor for that class.
Many to Many Relationship (M:M)
Each entity instance in one entity class is related to multiple entity instances in another entity class; and vice versa.

For example:
Each student can take many classes, and each class can be taken by many students.
Each consumer can buy many products, and each product can be bought by many consumers.
The detailed Crow's Foot Relationship symbols can be found here. Crow's Foot Relationship Symbols

##### Many to many relationships are difficult to represent. We need to decompose a many to many (M:M) relationship into two one-to-many (1:M) relationships.

##### Attributes
Attributes are facts or description of entities. They are also often nouns and become the columns of the table. For example, for entity student, the attributes can be first name, last name, email, address and phone numbers.

### About Primary key & foreign key - 

##### Primary Key
Primary Key* or identifier is an attribute or a set of attributes that uniquely identifies an instance of the entity. For example, for a student entity, student number is the primary key since no two students have the same student number. We can have only one primary key in a table. It identify uniquely every row and it cannot be null.

##### Foreign key
A foreign key+ (sometimes called a referencing key) is a key used to link two tables together. Typically you take the primary key field from one table and insert it into the other table where it becomes a foreign key (it remains a primary key in the original table). We can have more than one foreign key in a table.

An Example
Here's a sample crowsfoot diagram from a past offering of CS270 taught here at the University of Regina. We've redrawn the diagrams using more modern diagramming tools, but the content is unchanged. It uses a lot of ERD symbols.

![image](https://user-images.githubusercontent.com/89846476/132716090-14c92307-1c05-4aa5-a413-0b3c5f39e19f.png)


### SQL and Types of SQL Statements -
Data Definition Language (DDL) Statements
Data definition language (DDL) statements let you to perform these tasks:

Create, alter, and drop schema objects

Grant and revoke privileges and roles

Analyze information on a table, index, or cluster

Establish auditing options

Add comments to the data dictionary

The CREATE, ALTER, and DROP commands require exclusive access to the specified object. For example, an ALTER TABLE statement fails if another user has an open transaction on the specified table.

The GRANT, REVOKE, ANALYZE, AUDIT, and COMMENT commands do not require exclusive access to the specified object. For example, you can analyze a table while other users are updating the table.

Oracle Database implicitly commits the current transaction before and after every DDL statement.

Many DDL statements may cause Oracle Database to recompile or reauthorize schema objects. For information on how Oracle Database recompiles and reauthorizes schema objects and the circumstances under which a DDL statement would cause this, see Oracle Database Concepts.

DDL statements are supported by PL/SQL with the use of the DBMS_SQL package.

See Also:

PL/SQL Packages and Types Reference
The DDL statements are:


ALTER ... (All statements beginning with ALTER)
ANALYZE
ASSOCIATE STATISTICS
AUDIT
COMMENT
CREATE ... (All statements beginning with CREATE)
DISASSOCIATE STATISTICS
DROP ... (All statements beginning with DROP)
FLASHBACK ... (All statements beginning with FLASHBACK)
GRANT
NOAUDIT
PURGE
RENAME
REVOKE
TRUNCATE
Data Manipulation Language (DML) Statements
Data manipulation language (DML) statements access and manipulate data in existing schema objects. These statements do not implicitly commit the current transaction. The data manipulation language statements are:


CALL
DELETE
EXPLAIN PLAN
INSERT
LOCK TABLE
MERGE
SELECT
UPDATE
The SELECT statement is a limited form of DML statement in that it can only access data in the database. It cannot manipulate data in the database, although it can operate on the accessed data before returning the results of the query.

The CALL and EXPLAIN PLAN statements are supported in PL/SQL only when executed dynamically. All other DML statements are fully supported in PL/SQL.

Transaction Control Statements
Transaction control statements manage changes made by DML statements. The transaction control statements are:


COMMIT
ROLLBACK
SAVEPOINT
SET TRANSACTION
All transaction control statements, except certain forms of the COMMIT and ROLLBACK commands, are supported in PL/SQL. For information on the restrictions, see COMMIT and ROLLBACK.

Session Control Statements
Session control statements dynamically manage the properties of a user session. These statements do not implicitly commit the current transaction.

PL/SQL does not support session control statements. The session control statements are:


ALTER SESSION
SET ROLE
System Control Statement
The single system control statement, ALTER SYSTEM, dynamically manages the properties of an Oracle Database instance. This statement does not implicitly commit the current transaction and is not supported in PL/SQL.

Embedded SQL Statements
Embedded SQL statements place DDL, DML, and transaction control statements within a procedural language program. Embedded SQL is supported by the Oracle precompilers and is documented in the following books:

### Oracle Database 12c Architecture -
### HR Schema in this Course -



- 📫 reach me at - tanmaya_ise@rediffmail.com

