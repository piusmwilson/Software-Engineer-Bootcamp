# DATABASE ADMINISTRATION

A Basic learning resource documentation guide of databases and database administration for Database  Administrator,Developers and other Database users.

## TABLE OF CONTENTS

- [INTRODUCTION](#introduction)
- [WHAT IS DATABASE ADMINSTRATION](#what-is-database-adminstration)
- [WHO IS A DATABASE ADMINISTRATOR(DBA)](#who-is-a-database-administratordba)
- [WHY DATABASES](#why-databases)
- [WHAT IS A DATABASE](#what-is-a-database)
- [DATA MODELS IN DATABASES](#data-models-in-databases)
- [TYPES OF DATABASES](#types-of-databases)
- [BASIC DATABASE TERMINOLOGY](#basic-database-terminology)
- [DATABASE DATA TYPES](#database-data-types)
- [TYPES OF KEYS IN DATABASES](#types-of-keys-in-databases)
- [RELATIONAL AND NON-RELATIONAL DATABASES](#relational-and-non-relational-databases)
  - [Relational Databases](#relational-databases)
  - [Non-Relational Databases](#non-relational-databases)
- [ACID PROPERTIES](#acid-properties)
- [The DATABASE BASE PHILOSOPHY AND CAP THEOREM](#the-database-base-philosophy-and-cap-theorem)
  - [Base Philosophy](#base-philosophy)
  - [CAP Theorem](#cap-theorem)
- [DATABASE MANAGEMENT SYSTEMS (DBMS)](#database-management-systems-dbms)
- [DATABASE NORMALIZATION](#database-normalization)
  - [Normal Forms](#normal-forms)
  - [Applications of Normal Forms in DBMS](#applications-of-normal-forms-in-dbms)  
  - [Advantages of Normal Forms](#advantages-of-normal-forms)
  - [Some Important Points about Normal Forms](#some-important-points-about-normal-forms)
- [DATABASE QUERYING](#database-querying)
  - [Structured query language (SQL)](#structured-query-language-sql)
  - [The Origin of SQL](#the-origin-of-sql)
  - [SQL Datatypes](#sql-datatypes)
  - [The SQL Sub-Languages](#the-sql-sub-languages)
  - [SQL Commands](#sql-commands)
    - [DDL | Data Definition Language](#ddl--data-definition-language)
    - [DQL | Data Query Language](#dql--data-query-language)
    - [DML | Data Manipulation Language](#dml--data-manipulation-language)
    - [DCL | Data Control Language](#dcl--data-control-language)
    - [TCL | Transaction Control Language](#tcl--transaction-control-language)
  - [Frequently used SQL Commands](#frequently-used-sql-commands)
  - [The SQL Process](#the-sql-process)
    - [SQL Query Execution Order](#sql-query-execution-order)
  - [Other Notable Database Languages](#other-notable-database-languages)
  - [Query Optimization](#query-optimization)
  - [SQL Indexing](#sql-indexing)
    - [What is an Index?](#what-is-an-index)
    - [Some Indexing Use cases](#some-indexing-use-cases)
  - [SQL Views](#sql-views)
  - [SQL Unions](#sql-views)
  - [SQL JOINS](#sql-joins)
    - [Types of SQL Joins](#types-of-sql-joins)
  - [SQL Automation](#sql-automation)
  - [Common Table Expressions(CTEs) in SQL](#common-table-expressionsctes-in-sql)
    - [What are Common Table Expressions (CTEs)?](#what-are-common-table-expressions-ctes)
    - [Types of CTEs](#types-of-ctes)
    - [CTE vs Subquery](#cte-vs-subquery)
    - [CTE vs. Temporary Tables](#cte-vs-temporary-tables)
  - [Difference between SQL, MySQL and and MsSQL](#difference-between-sql-mysql-and-and-mssql)
  - [The difference between SQL and NoSQL](#the-difference-between-sql-and-nosql)
- [DATABASE HASHING](#database-hashing)
  - [Hashing in DBMS](#hashing-in-dbms)
  - [Properties of Hashing in DBMS](#properties-of-hashing-in-dbms)
  - [Hash Organization](#hash-organization)
  - [Types of Hashing](#types-of-hashing)
    - [Static Hashing](#static-hashing)
    - [Dynamic Hashing](#dynamic-hashing)
- [THE DATABASE DESIGN PROCESS](#the-database-design-process)
- [DATABASE SECURITY](#database-security)
  - [Security Features](#security-features)
  - [Security Principles](#security-principles)
  - [Roles](#roles)
- [BUSINESS INTELLIGENCE](#business-intelligence)
  - [Transactional Data and Analytical Data processing](#transactional-data-and-analytical-data-processing)
  - [Data Warehouses](#data-warehouses)
    - [Data Warehouse Designed Criteria](#data-warehouse-designed-criteria)
    - [The Bottom-Up and Top-Down Data warehouse Design Approachs](#the-bottom-up-and-top-down-data-warehouse-design-approachs)
    - [Benefits of Data Warehouses include](#benefits-of-data-warehouses-include)
  - [Operational Data Stores (ODS)](#operational-data-stores-ods)
  - [Data Marts](#data-marts)
  - [Data Lakes](#data-lakes)
  - [What Is ETL?](#what-is-etl)
    - [ETL Pipelines](#etl-pipelines)
    - [Characteristics Of an ETL Pipeline](#characteristics-of-an-etl-pipeline)
    - [How Does ETL work?](#how-does-etl-work)
  - [Data Mining and Machine Learning](#data-mining-and-machine-learning)
- [CHOOSING A DATABASE PLATFORM](#choosing-a-database-platform)
- [CONCLUSION](#conclusion)
- [SQL CHEATSHEET](#sql-cheatsheet)
  - [Data Types](#data-types)
  - [SQL Essentials](#sql-essentials)
  - [Query](#query)
- [SQL INTERVIEW QUESTIONS](#sql-interview-questions)
  - [Basic SQL Questions](#basic-sql-questions)
  - [Intermediate SQL Questions](#intermediate-sql-questions)
  - [Advanced SQL Questions](#advanced-sql-questions)
- [FREQUENTLY ASKED QUESTIONS (FAQ)](#frequently-asked-questions-faq)
- [GLOSSARY](#glossary)
- [RESOURCES AND REFERENCES](#resources-and-references)
- [KEYWORDS](#keywords)

## INTRODUCTION

A database is one of the most important parts of a software system, whether for an application or a data warehouse project and as such, it's becomes important to have good foundation knowledge of databases and a way of evaluating them when planning a project or taking on database adminstration projects.

Picking a database is a long-term commitment, therefore you should not underestimate the time you spend planning your data needs and scope as well as where and how you will store this data because a database is the foundation of your application providing secure, reliable storage and access to all of your information. Therefore without trustworthy data, you don’t have much of an application.

**Data** is raw facts, and can be **_Quantitative_ or _Qualitative_** where **Quantitative** data is numeric and  **Qualitative** data is descriptive.

Data is collected, stored and processed to derive **Information** that possess context, relevance, and purpose yielding insightful knowledge for the bearer of that information.

**Knowledge** is collection of experience, beliefs or perceptions gained from  facts or concepts relevant to all matters of life coursety of accumulated information over time. It can be viewed as information that facilitates action.

Once we have aggregated, analyzed and put our data into understandable context that generates useful information to build knowledge, we can then use this acquired knowledge to make decisions, set policies, and even spark innovation.

Explicit knowledge typically refers to knowledge that can be expressed into words or numbers while tacit knowledge includes insights and intuitions, and is difficult to transfer to another person by means of simple communications therefore someone is said to have wisdom when they can combine their knowledge and experience to produce a deeper understanding of a topic. It often takes many years to develop wisdom on a particular topic, and requires patience.

When this data is discovered, sometimes it has to be stored somewhere, where it can then be retrieved for processing to derive useful information and insights. This is where **databases** come in hand and thus the need for **database administration**.

Data visualization is the graphical representation of information and data. These graphical representations (such as charts, graphs, and maps) can quickly summarize data in a way that is more intuitive and can lead to new insights and understandings. Just as a picture of a landscape can convey much more than a paragraph of text attempting to describe it, graphical representation of data can quickly make meaning of large amounts of data.

Many times, visualizing data is the first step towards a deeper analysis and understanding of the data collected by an organization. Examples of data visualization software include Tableau, PowerBI, and R Studio.

This documentation resources endevours to explore all the basic knowledge and concepts that a beginner on database administration can utilize to learn what there is to know about databases and how to manage them making way for exploring a deep understanding the world of databases.

## WHAT IS DATABASE ADMINSTRATION?

## WHO IS A DATABASE ADMINISTRATOR(DBA)

A Database Administrator is a person who is responsible for executing different set of activities which help in managing a database.
He/She ; -

- creates and administers databases to make sure they operate efficiently and without error.
- Make modifications to the database structure.
- Maintain databases and update permissions.
- Merge old databases into new ones as and when required.
- Backing up and restoring data to prevent data loss.

to mention but a few.
Often times DBA can also specialize depending on the company, industry or just the nature of work.

Types of DBA include but not limited to;-

- **Administrative DBA** - Maintains databases, backups, security, patching, replications etc.
- **Development DBA** - Builds SQL queries, procedures, functions. Same as programmer.
- **Database Architect** - Builds database structures with clients and implements.
- **Data warehouse DBA** - Responsible for merging data from multiple sources into one warehouse.

and many more.

## WHY DATABASES?

Data is a valuable resource in a business or organization and almost all software programs require data to be useful, therefore the goal of many information systems is to be able to transform data into information in order to generate knowledge that can be used for decision making.

In order to do this, the system must be able to take data, allow the user to put the data into context, and provide tools for aggregation and analysis and databases are designed for such purposes.

## WHAT IS A DATABASE?

A Database is a structured set or collection of data often organised into tables, each consisting of rows and column, stored in a computer. Each row in a table represents a specific instance or record, and each column holds a specific type of data.

Databases are designed to provide efficeint access to data, and serve an important function for many individuals and companies, by providing effective and practical ways to organize and store information using or on a computer.

Business Analysts, QAs, Database Administrators and developers among other *'technical actors'* use database languages to design, maintain and monitor databases and their related management systems.

Stored data can be searched quickly with the options for;- Data Validation, Parallel Access, Access control, Computation & aggregation.

## DATA MODELS IN DATABASES

Databases can be organized in many different ways by using different models. The data model of a database is the logical structure of data items and their relationships. There have been several data models. Since the 1980s, the relational data model has been popularized.

In a relational database, data is organized into tables (or relations), with each table consisting of a set of fields which define the structure of the data stored in that table. A record is one instance of a set of fields in a table. Think of the records as the rows (or tuple) of the table and the fields as the columns of the table.

Even though the relational database model is the most used database model today, many other database models exist that provide different strengths than the relational model and some companies are looking to provide large-scale database solutions by moving away from the relational model to other, more flexible models.

The hierarchical database model, popular in the 1960s and 1970s, connected data together in a hierarchy, allowing for a parent/child relationship between data. The document-centric model allowed for a more unstructured data storage by placing data into “documents” that could then be manipulated.

A special field or a combination of fields that determines the uniqueness of a record is called primary key (or key). A key is usually the unique identification number of the records. Check out [A Relational Model Of Data For Large Shared Data Banks](https://github.com/piusmwilson/business-information-technology-library/blob/main/resources/A%20Relational%20Model%20of%20Data%20for%20Large%20Shared%20Data%20Banks-codd.pdf), on the earliest mentions of relational data models.

## TYPES OF DATABASES

- **Relational Databases** store data in tables with predefined schemas and relationships and are useful for applications requiring complex queries and ACID transactions. Examples of Relational Databases include MySQL, Microsoft SQL Server, Oracle Database and PostgreSQL databases.

- **Hierarchical Databases** organizes data in a tree-like structure with parent-child relationships and are useful for representing hierarchical data like file systems and XML documents. Examples of Hierarchical Databases include IBM IMS, and Windows Registry databases.

- **Object-Oriented Databases** store data as objects, following OOP principles and are Ideal for applications with complex data models. Examples of Object-Oriented Databases include ObjectDB, and db4o databases.

- **In-Memory Databases** can store an entire database in RAM for extremely fast data access used for caching and high-speed transactions. Examples of In-Memory Databases include Redis, and Memcached databases.

- **Key-Value Store Databases** store data as key-value pairs for fast retrieval and are ideal for caching, session storage, and real-time data access. Examples of Key-Value Store Databases include Redis, and Amazon DynamoDB databases.

- **Document Databases(_document-oriented_)** store data in flexible, semi-structured document formats like JSON or XML and are used for unstructured or rapidly changing data. Examples of Document Databases include MongoDB, and Couchbase databases.

- **Graph Databases** store data as nodes and edges used to represent complex relationships like recommendation engines and social networks. Examples of Graph Databases Neo4j, and Amazon Neptune databases.

- **Vector Databases** are designed for storing and searching high-dimensional vectors and ideal for AI applications and similarity searches like recommendation systems, image/video search. Examples of Vector Databases include Faiss, and Milvus databases.

- **Embedded Databases** are lightweight databases embedded within applications used in desktop, mobile applications, and IoT devices. Examples of these Embedded Databases include SQLite, and RocksDB databases.

- **Wide-Column Store Databases(_Column-family stores_)** store data in flexible columns to optimize reading a specific attribute.
They are useful for applications dealing with large volumes of data and running analytical queries and their examples include Cassandra, and HBase databases.

- **Time-Series Databases** are optimized for storing and querying time-stamped data and very useful for monitoring systems, financial data and real-time analytics. Examples of Time-Series Databases include InfluxDB, and Prometheus databases.

- **Text Search Databases** are optimized for indexing and searching text data and often used for content-heavy applications like search engines. Examples of Text Search Databases include Elasticsearch, and Solr databases.

- **Spatial Databases** are used to store and query location-based data and are ideal for GIS, location-based services, and mapping applications. Examples of Spatial Databases include PostGIS(_PostgreSQL_), MongoDB Spatial and Oracle Spatial databases.

- **Blob Store Databases** are optimized for storing and retrieving large objects like images, videos, files and often used for content delivery networks and backup systems. Examples of Blob Store Databases include Amazon S3, and HDFS databases.

- **Ledger Databases** provides an immutable, append-only record system and are deal for blockchain applications like supply chain and financial transactions. Examples of Ledger Databases include QLDB, and Hyperledger Fabric databases.

- **Blockchain Databases** BigchainDB, IBM Blockchain.
- **Distributed Databases** Apache Cassandra, Amazon DynamoDB.

## BASIC DATABASE TERMINOLOGY

- A **database hierarchy** is a way of organising data in a structured manner so it can be easily accessed, managed and updated.
- A **Schema diagram** is a database schema containing primary keys and foreign key dependencies, table name, relation name, attribute name. A schema diagram will have relation table names and attribute names along with the column.
- A **database schema** is the logical view of the entire database.
- **Relational database schema** is a set of relation schemas and a set of integrity constraints.
- A **relational schema** is used to describe a relation made up of a *relation name R* and a *list of attributes A1,A2,A3------An,* *e.g ``Employee(Name, EmployeeNo, Age, Address, Telno)``*
- **Relational data models**, first introduced by a computer scientist & mathematician called Ted Codd in 1970, represent data as a collection of tables.
- A **table**, also called a relation is a set of tuples, the most basic unit of a database consisting of ``rows`` and ``columns`` of data. A single table holds ``records``, and each record is stored in a ``row`` of the table. Tables are the most used type of database objects, or structures that hold or reference data in a relational database. Also note that each row is a tuple which in turn is set of (***Attributes, value***) pairs.
- **Views** are logical representations of data assembled from one or more database tables.
- **Indexes** are lookup tables that help speed up database lookup functions.
- **Reports** consist of data retrieved from one or more tables, usually a subset of that data that is selected based on search criteria.
- A **Relation state** or relation instance is a set of tuples at a given time.
- A **relationship** is an association among 2 or more entities.
- **Entity-Relationship(E-R) Models** describe entities, attributes and relationships of a database.They let us represent several kind of constraints that schema diagrams may not.
- The **Degree** or **Arity** of a relation is the number of attributes in a relation schema, e.g in Employee example, the degree or arity will be 5.
- **Degree of relationship** denotes the number of entity types that participate in a relationship.
- A **unary relationship** exists when there is an association with only one entity.
- A **binary relationship** exists when there is an association among two entities.
- A **tunary relationship** exists when there is an association among three entities.
- **Cardinality** is the total number of tuples present in a relation.
- **Cardinality ratio** is the maximum number of relationship instances that an entity can participate in. The possible cardinality ratios for binary relationships are 1:1, 1:N, N:1, M:N.
- A **domain** is a set of atomic values allowed for an attribute.
- **Column headers** are attributes.
- **Attributes** that have a primary key contraints/dependancy are underlined and foreign key constraint/dependency are represented with arrows.
- **Database Keys** are attribute or a set of attributes which help you uniquely idenify a record or a row of data in a relation(table). They also ensure data integrity by forcing identity of the said data as well as help identify and establsih relationship between tables.

## DATABASE DATA TYPES

When defining the fields in a database table, we must give each field a data type and most modern databases allow for several different data types to be stored.

Some of the more common data types include:

- **Text:** for storing non-numeric data that is brief, generally under 256 characters. The database designer can identify the maximum length of the text.
- **Number:** for storing numbers. There are usually a few different number types that can be selected, depending on how large the largest number will be.
- **Boolean:** a data type with only two possible values, such as 0 or 1, “true” or “false”, “yes” or “no”.
- **Date/Time:** a special form of the number data type that can be interpreted as a number or a time.
- **Currency:** a special form of the number data type that formats all values with a currency indicator and two decimal places.
- **Paragraph Text:** this data type allows for text longer than 256 characters.
- Object: this data type allows for the storage of data that cannot be entered via keyboard, such as an image or a music file.

It's  important to properly define the data type of a field because:

- A data type tells the database the kind of data it's handling to ascertain what functions can be performed with the data. For example, if we wish to perform mathematical functions with one of the fields, we must be sure to tell the database that the field is a number data type.

- It helps a database ascertain that proper amount of storage space is allocated for our data. For example, if the ``EmployeeName`` field is defined as a ``Text(50)`` data type, this means _50_ characters are allocated for each name we want to store. If a employee’s name is longer than _50_ characters, the database will truncate it.

When a database is being designed, a “data dictionary” is created to hold the metadata, defining the fields and structure of the database. Metadata is the _“data about data”_.

**Examples of metadata of database are:**

- number of records
- data type of field
- size of field
- description of field
- default value of field
- rules of use.

## TYPES OF KEYS IN DATABASES

- A **Primary Key** is a unique identifier for each record in a table. It cannot have a null value and must be unique across the entire table.
- A **Composite Key** is a combination of two or more columns used as a primary key, often used when a single column is not sufficient to uniquely identify a record.
- A **Foreign Key** is a field in a table that matches the primary key of another table. It creates a link between the two tables and is used to establish a relationship between them.
- An **Alternate Key** is a unique identifier for a record that is not the primary key often used as a secondary way to look up data in the table.
- A **Surrogate Key** is a unique identifier signed to a record in a table, typically by the database rather than the user.
- A **Candidate Key** is a unique identifier for a record in a table that could potentially be used as a primary key.

## RELATIONAL AND NON-RELATIONAL DATABASES

Databases can be categorised into Relational databases _(Miscrosoft SQL Server(MsSQL), Oracle, PostgreSQL, MySQL)_ or Non-Relational/NoSQL databases _(MongoDB, Rediscover, Cassandra, etc)_.

Often times Relational databases are called SQL Databases, but this is because the original databases where all relational following the traditional SQL. Non-Relational databases are called NoSQL because they are more dynamic in the way their data is accessed or interacted with compared to their Relational counterparts.

### Relational Databases

Relational databases are commonly used to store and query structured data. The data is stored in tables that represent entities, such as customers, products, or sales orders. Each instance of an entity is assigned a primary keythat uniquely identifies it; and these keys are used to reference the entity instance in other tables.

For example, a customer's primary key can be referenced in a sales order record to indicate which customer placed the order. This use of keys to reference data entities enables a relational database to be normalized; which in part means the elimination of duplicate data values so that, for example, the details of an individual customer are stored only once; not for each sales order the customer places. The tables are managed and queried using Structured Query Language (SQL), which is based on an ANSI standard, so it's similar across multiple database systems.

Relational Databases are designed to capture and record data via OLTP _(Online Transaction Process)_. Online Transaction Processing (OLTP) is a data capture system capable of recording multiple concurrent transactions.

OLTPs use a relational database that can process a large number of relatively simple transactions e.g insertions, queries, updates and deletions, etc with rapid processing. It enables the real time execution of large numbers of database transactions by large numbers of people.

Organisations used OLTP to provide information to OLAP.

Online Analytical Processing (OLAP) is a system created to mainly process huge amounts of data. Multi-dimensional databases(MDB/Cube) also called ***OLAP Cube*** extends the row by column format of a traditional relational databases cannot be a data warehouse and typically outputs of Data warehouses

A **Normalized data format**, also called _Normalized Data store(NDS)_ is a database concept of removing redundancy from databases while a **Denormalized data format** encourages data redundancy in databases. _Dimensional data model_ is a sub-version of denormalized data format widely used for data ware housing. Data stores built using dimensional data models are called _Dimensional Data Store(DDS)_. Read more about [DATABASE NORMALIZATION](#database-normalization) here.

### Non-Relational Databases

Non-relational databases are data management systems that don’t apply a relational schema to the data. Non-relational databases are often referred to as NoSQL database, even though some support a variant of the SQL language.

**There are four common types of Non-relational database commonly in use.**

- **Key-value databases** in which each record consists of a unique key and an associated value, which can be in any format.
- **Document databases**, which are a specific form of key-value database in which the value is a JSON document _(which the system is optimized to parse and query)_.
- **Column family databases**, which store tabular data comprising rows and columns, but you can divide the columns into groups known as column-families. Each column family holds a set of columns that are logically related together.
- **Graph databases**, which store entities as nodes with links to define relationships between them.

## ACID PROPERTIES

- **Atomicity:** each transaction is treated as a single unit, which succeeds completely or fails completely. For example, a transaction that involved debiting funds from one account and crediting the same amount to another account must complete both actions. If either action can't be completed, then the other action must fail.

- **Consistency:** transactions can only take the data in the database from one valid state to another. To continue the debit and credit example above, the completed state of the transaction must reflect the transfer of funds from one account to the other.

- **Isolation:** concurrent transactions cannot interfere with one another, and must result in a consistent database state. For example, while the transaction to transfer funds from one account to another is in-process, another transaction that checks the balance of these accounts must return consistent results - the balance-checking transaction can't retrieve a value for one account that reflects the balance beforethe transfer, and a value for the other account that reflects the balance afterthe transfer.

- **Durability:** when a transaction has been committed, it will remain committed. After the account transfer transaction has completed, the revised account balances are persisted so that even if the database system were to be switched off, the committed transaction would be reflected when it is switched on again.

## The DATABASE BASE PHILOSOPHY AND CAP THEOREM

### BASE Philosophy

    - Basically Available- System will stay up using replication/sharding.
    - Soft state- No guarantee that data is consistent, reads can yield stale data.
    - Eventual Consistency- If we wait long enough, reads will yield consistent data.

### CAP Theorem

Consistency, Availability and partition Tolerance

## DATABASE MANAGEMENT SYSTEMS (DBMS)

To the computer, a database looks like one or more files. In order for the data in the database to be stored, read, changed, added, or removed, a software program must access it.

There is a category of software applications called database management systems (DBMS), whose purpose is to create a database, change a database’s structure, or simply do analysis among other database related activities.

A DBMS is a software system that provides users and applications with the ability to access and manipulate data stored in a database. It essentially provides tools for defining, constructing, and manipulating databases, as well as providing security and backup features.

DMBS examples include MySQL, Oracle, Microsoft SQL Server, etc.

## DATABASE NORMALIZATION

An important concept to understand when designing databases is normalization, a way of designing a database while reducing data redundancy and ensuring data integrity.

Normalization is the process of minimizing redundancy from a relation or set of relations. Redundancy in relation may cause _insertion, deletion_, and _update_ anomalies. So, it helps to minimize _(eliminate or reduce)_ the redundancy in database tables using **_Normal forms_**.

- There are several levels of normalization, each with its own set of guidelines, known as **Normal forms** which are a series of guidelines that help to ensure that the design of a database is efficient, organized, and free from data anomalies.

### Normal Forms

The **_(1NF, 2NF, 3NF, BCNF, 4NF,_** and **_5NF)_** normal forms in database administration, are how relational databases are arranged to help reduce data redundancy, preserve data integrity and increase data consistency. And by resolving various kinds of data anomalies and dependencies _(partial, transtive, multi-valued, functional, & join)_, each subsequent normal form expands upon the one that came before it.

- **First normal form (1NF)** is the most basic level of normalization. In 1NF, each table cell should contain only a single value _(Atomic Values)_, and each column should have a unique name _(Unique Column Identifier)_. The first normal form helps to eliminate duplicate data and simplify queries.

- **Second normal form (2NF)** eliminates redundant data by requiring that each non-key attribute be dependent on the primary key. This means that each column should be directly related to the primary key, and not to other columns _(No Partial Dependency)_.

- **Third normal form (3NF)** builds on 2NF by requiring that all non-key attributes are independent of each other. This means that each column should be directly related to the primary key, and not to any other columns in the same table _(No Transitive Dependency)_.

- [**Boyce–Codd normal form**(or BCNF or 3.5NF)](https://en.wikipedia.org/wiki/Boyce%E2%80%93Codd_normal_form) is a normal form used in database normalization. It is a slightly stronger version of the third normal form (3NF) and ensures that each determinant in a table is a candidate key. In other words, BCNF ensures that each non-key attribute is dependent only on the candidate key. _BCNF was developed in 1974 by Raymond F. Boyce and Edgar F. Codd to address certain types of anomalies not dealt with by 3NF as originally defined_.

- **Fourth Normal Form (4NF)** is a further refinement of BCNF that ensures that a table does not contain any multi-valued dependencies.

- **Fifth Normal Form (5NF)** also known as Project Join Normal Form(PJNF) is the highest level of normalization and involves decomposing a table into smaller tables to remove data redundancy and improve data integrity. _(No join Dependency, Meaning if Join Dependency exsists, Decompose the table.)_

### Applications of Normal Forms in DBMS

- **Data consistency:** Normal forms ensure that data is consistent and does not contain any redundant information. This helps to prevent inconsistencies and errors in the database.
- **Data redundancy:** Normal forms minimize data redundancy by organizing data into tables that contain only unique data. This reduces the amount of storage space required for the database and makes it easier to manage.
- **Response time:** Normal forms can improve query performance by reducing the number of joins required to retrieve data. This helps to speed up query processing and improve overall system performance.
- **Database maintenance:** Normal forms make it easier to maintain the database by reducing the amount of redundant data that needs to be updated, deleted, or modified. This helps to improve database management and reduce the risk of errors or inconsistencies.
- **Database design:** Normal forms provide guidelines for designing databases that are efficient, flexible, and scalable. This helps to ensure that the database can be easily modified, updated, or expanded as needed.

### Advantages of Normal Forms

- **Simplified database design:** Normalization provides guidelines for organizing tables and data relationships, making it easier to design and maintain a database.
- **Reduced data redundancy:** Normalization helps to eliminate duplicate data in tables, reducing the amount of storage space needed and improving database efficiency.
- **Improved data consistency:** Normalization ensures that data is stored in a consistent and organized manner, reducing the risk of data inconsistencies and errors.
- **Improved query performance:** Normalized tables are typically easier to search and retrieve data from, resulting in faster query performance.
- **Easier database maintenance:** Normalization reduces the complexity of a database by breaking it down into smaller, more manageable tables, making it easier to add, modify, and delete data.

Overall, even though using normal forms in DBMS helps to reduce data redundancy, increase data consistency, improve data quality & database performance, increase database performance & efficiency, as well as simplify database design and maintenance, higher levels of normalization can lead to more complex database designs and queries, therefore it is important to strike a balance between normalization and practicality when designing a database.

### Some Important Points about Normal Forms

- BCNF is free from redundancy caused by Functional Dependencies.
- If a relation is in BCNF, then 3NF is also satisfied.
- If all attributes of relation are prime attribute, then the relation is always in 3NF.
- A relation in a Relational Database is always and at least in 1NF form.
- Every Binary Relation _(a Relation with only 2 attributes)_ is always in BCNF.
- If a Relation has only singleton candidate keys( i.e. every candidate key consists of only 1 attribute)_, then the Relation is always in 2NF _(because no Partial functional dependency possible)_.
- Sometimes going for BCNF form may not preserve functional dependency. In that case go for BCNF only if the lost FD(s) is not required, else normalize till 3NF only.
- There are many more Normal forms that exist after BCNF, like 4NF and more. But in real world database systems it’s generally not required to go beyond BCNF.

## DATABASE QUERYING

Once you have a database designed and loaded with data, you will need a way to interact with the database and the data stored in it.

This process of performing the various critical tasks on databases is called database querying and among other things helps ensure database management systems function correctly and that databases are secure, up-to-date while operating at peek performance.

The languages used for database querying are referred to as *SQL Sub-Languages* under Structured Query Language(SQL) pronounced “sequel,” or simply stated as S-Q-L.

### Structured query language (SQL)

Structured query language (SQL) is a standardized, domain-specific programming language for managing _(e.g. storing and processing information)_ relational databases or performing various operations on the data in them.

SQL is not case sensitive, but generally it's keywords are written in uppercase especially for big projects which have intense database querying. Also, being dependent on text lines, SQL statements can be written as a single SQL statement on one or multiple text lines.

Therefore, by using Structure Query Language(SQL) statements, you as a database user at any one time can perform most of the actions in a database.

Initially created in the 1970s, SQL is tremendously powerful when it comes to Database Management, and regularly used not only by database administrators, but also by developers writing data integration scripts and data analysts looking to set up and run analytical queries.

Like any well-designed programming tool, SQL includes certain commands that every developer should be familiar with while working with databases.

SQL queries and other operations take the form of commands written as statements, aggregated into programs that enable users to add, modify or retrieve data from database tables.

The term SQL is pronounced ```ess-kew-ell```, ```ɛsˌkjuːˈɛl```,```S-Q-L``` or sometimes ```siːkwəl```, sequel for historical reasons.

SQL was designed to be used both as a stand-alone language for interactive queries and as an application development language for online transaction processing (OLTP).

### The Origin of SQL

In the late 1960s when the first database appeared, [Edgar Frank (Ted) Codd](https://en.wikipedia.org/wiki/Edgar_F._Codd), an English computer scientist at IBM was working on one of his articles, called [“A Relational Model of Data for Large Shared Data Banks”](https://github.com/piusnmuhumuza/bootcamp/blob/master/Database%20Adminstration/docs/A%20Relational%20Model%20of%20Data%20for%20Large%20Shared%20Data%20Banks-codd.pdf). This article officially started the relational database era, and made him the father of SQL in a manner of speaking.
However, his brilliant idea wasn’t immediately adopted or used, Until 1973, when a project called ‘System R’ was started with Don Chamberlin and Ray Boyce as the leading scientists, and surprisingly, Codd wasn’t assigned to that project.

SQL was initially developed at [IBM](https://en.wikipedia.org/wiki/IBM) by [Donald D. Chamberlin](https://en.wikipedia.org/wiki/Donald_D._Chamberlin) and [Raymond F. Boyce](https://en.wikipedia.org/wiki/Raymond_F._Boyce) after learning about the relational model from [Edgar F. Codd](https://en.wikipedia.org/wiki/Edgar_F._Codd) in the early 1970s. This version, initially called **SEQUEL** ***(Structured English QUEry Language)***, was designed to manipulate and retrieve data stored in IBM's original [Quasi-Relational database management system](https://github.com/piusnmuhumuza/bootcamp/blob/master/Database%20Adminstration/docs/aQuasiDistributedArchitecture.pdf), [System R](https://en.wikipedia.org/wiki/IBM_System_R), which a group at [IBM San Jose Research Laboratory](https://en.wikipedia.org/wiki/IBM_Research#Almaden_in_Silicon_Valley) had developed during the 1970s.

Chamberlin and Boyce's first attempt at a relational database language was SQUARE (Specifying Queries in A Relational Environment), but it was difficult to use due to subscript/superscript notation. After moving to the San Jose Research Laboratory in 1973, they began work on a sequel to [SQUARE](https://github.com/piusmwilson/business-information-technology-library/blob/main/resources/SQUARE%20(Specifying%20Queries%20in%20A%20Relational%20Environment).pdf).

The original name SEQUEL, which is widely regarded as a pun on QUEL, the query language of Ingres, was later changed to SQL (dropping the vowels) because "SEQUEL" was a trademark of the UK-based Hawker Siddeley Dynamics Engineering Limited company. The label SQL later became the acronym for Structured Query Language. [Read More here](https://en.wikipedia.org/wiki/SQL).

Check out the [Early History Of SQL](https://github.com/piusmwilson/business-information-technology-library/blob/main/resources/Early_History_of_SQL.pdf) Document for some more details on SQL's Origins.

### SQL Datatypes

An SQL Datatype is used to define the values that a column can contain. Every column is required to have a name and data type in the database table.

SQL Data types include the Binary, Numeric, Extra numeric, String, Date data types.

### The SQL Sub-Languages

Although SQL is essentially a declarative language (4GL), it also includes procedural elements. The scope of SQL includes data query, data manipulation _(insert, update, and delete)_, data definition _(schema creation and modification)_, and data access control.

Originally based upon relational algebra and tuple relational calculus, SQL consists of many types of statements, which may be informally classed as [sublanguages](https://en.wikipedia.org/wiki/Sublanguage 'Sublanguages: A sublanguages is a subset of a language. Sublanguages occur in natural language, computer programming language, and relational databases.'), commonly: **a Data Query Language (DQL)**, **a Data Definition Language (DDL)**, **a Data Control Language (DCL)**, and **a Data Manipulation Language (DML)**. Even though these sub-languages are mainly grouped into four categories, there is another one called;- the **Transaction Control Language (TCL)**.

SQL can perform various tasks like create a table, adddata to tables, drop the table, modify the table, set permission for users. Therefore SQL commands are instructions used to communicate with the database to perform specific tasks, functions, and queries of data.

### SQL Commands

![SQL Commands](https://github.com/piusnmuhumuza/bootcamp/blob/master/Database%20Adminstration/images/sql-commands.jpg "SQL Commands") *The common Structured Query Language(SQL)  Commands organised by their sub-languages.*

The five types of SQL commands_(DDL, DQL, DML, DCL, and TCL)_ are:

#### DDL | Data Definition Language

DDL,a set of SQL commands, mainly dealing with database schema descriptions is used to describe/define the database schema.
Also called data definition commands;- ```CREATE```, ```ALTER```, ```RENAME```, ```TRUNCATE```,``COMMENT`` & ``DROP``, commands are primarily used by privileged **Developers** and not **general users** to create, design, modify/alter, or destroy/delete the structure/layout of the objects stored in the database but not the data itself.

**The DDL Commands** include;-

- The **``CREATE``** command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
- The **``DROP``** command is used to delete objects from the database.
- The **``ALTER``** command is used to alter the structure of the database.
- The **``TRUNCATE``** command is used to remove all records from a table, including all spaces allocated for the records are removed.
- **``COMMENT``** is used to add comments to the data dictionary.
- The **``RENAME``** command is used to rename an object existing in the database.

#### DQL | Data Query Language

Data query language is part of the base grouping of SQL sub-languages and consists of just one command, ``SELECT``, used to get specific data from tables.

The purpose of DQL commands is to get the schema relation based on the query passed to it, e.g. When adding FROM or WHERE data manipulators to the ``SELECT`` statement, thus the reason this statement is sometimes _considered part/grouped with the DML commands_.

Nonetheless, the SQL ``SELECT`` statement is strictly an example of DQL, whose statements are used for performing queries on the data within schema objects.

#### DML | Data Manipulation Language

Primarily used by everyone but most specifically data analyst who write queries that target data. commands;- ```INSERT```, ```UPDATE```, ```DELETE```, are used to manipulate data in existing tables by adding, changing or removing data. Unlike DDL commands that define how data is stored, DML commands operate in the tables defined with DDL commands.

- The **``INSERT``** command is used to insert data into a table.
- The **``UPDATE``** command is used to update existing data within a table.
- The **``DELETE``** command is used to delete records from a database table.
- The **``LOCK``** command is used for Table control concurrency.
- The **``CALL``** command is a PL/SQL or JAVA subprogram.
- The **``EXPLAIN PLAN``** command describes the access path to data.

### DCL | Data Control Language

Primarily used by Database Administrators (DBA) for security accesses and control, these commands are used to grant or revoke user access privileges using;- ```GRANT```, ```REVOKE```, ```DENY``` commands.

- The **``GRANT``** command gives users access privileges to the database.

**Syntax:**

```sql
GRANT SELECT, UPDATE ON MY_TABLE TO SOME_USER, ANOTHER_USER;
```

- The **``REVOKE``** command withdraws the user’s access privileges given by using the GRANT command.

**Syntax:**

```sql
REVOKE SELECT, UPDATE ON MY_TABLE FROM USER1, USER2;  
```

- The **``DENY``** command even though not very common or getting deprecated is mean't to outright prohibit a user from accessing database objects and also overrides any granted accesses. [Read here](https://learn.microsoft.com/en-us/sql/t-sql/statements/deny-transact-sql?view=sql-server-ver16).

#### TCL | Transaction Control Language

Sometimes argued to be part of the sub-language set as well, TCL commands are used to change the state of some data -- for example, to ``COMMIT`` transaction changes or to ``ROLLBACK`` transaction changes.

A **transaction/Transactions group** is a set/collection of tasks that are executed as a _single entity/a single execution unit_. Each transaction commences with a particular task and ends when all of the tasks in the group are **_accomplished/successfully completed_**. The transaction fails when one or more of the tasks **_misses or fails_**. As a consequence, a transaction has just two *results/outcomes*: either it succeeds(**_Success_**) or it fails(**_failure_**).

**These are TCL commands that serve to manage transaction execution:**

- The **``BEGIN``** command initiates a transaction.
- The **``COMMIT``** command commits or terminates a transaction.
- The **``ROLLBACK``** Reverts a transaction if an error appears.
- The **``SAVEPOINT``** Creates a transaction save point.
- The **``SET TRANSACTION``** Defines the transaction’s parameters.

check out [TCL Full Form](https://www.geeksforgeeks.org/tcl-full-form/) for more.

### Frequently used SQL Commands

| SQL Command      | Syntax  | Description     |
| :---        |    :----:   |          ---: |
|ALTER TABLE     | `ALTER TABLE table_name ADD column_name datatype;`      | It is used for adding columns to a database table.   |
| AND  | `SELECT column_name(s)FROM table_nameWHERE column_1 = value_1  AND column_2 = value_2`       | This serves as an operator to combine two individual conditions.      |
|AS    | ```sql SELECT column_name AS ‘Alias’ FROM table_name;```      | This keyword in SQL is used in reTitle naming a table or columns using an alias name.  |
|AVG     | `SELECT AVG(column_name)FROM table_name;`      | It is used in aggregating a numerical column, returning its average.   |
|BETWEEN     | `SELECT column_name(s)FROM table_nameWHERE column_name BETWEEN value_1 AND value_2;`       | This operation filters the result within a specified range.  |
|CASE     | `SELECT column_name,CASE WHEN condition THEN ‘Result_1’WHEN condition THEN ‘Result_2’ELSE ‘Result_3’ENDFROM table_name;`       | It serves as a statement to create multiple outputs within a SELECT statement.  |
|COUNT    | `SELECT COUNT(column_name)FROM table_name;`      | This function takes a column name as an argument, then, counts the row number while the column is not NULL.   |
|CREATE TABLE     | `CREATE TABLE table_name (  column_1 datatype,   column_2 datatype,   column_3 datatype);`      | It creates a new table inside a dataset and defines the name for the table and columns inside it.   |
|DELETE     | `DELETE FROM table_nameWHERE some_column = some_value;`      | It is employed in the removal of rows from a table.   |
|GROUP BY    | `SELECT column_name, COUNT(*)FROM table_nameGROUP BY column_name;`       | It is a SQL clause used for aggregate functions in conjunction with the SELECT statement.   |
|HAVING     | `SELECT column_name, COUNT(*)FROM table_nameGROUP BY column_nameHAVING COUNT(*) > value;`       | Because the WHERE keyword cannot be used in aggregating functions, it is utilized in SQL.  |
|INNER JOIN     | `SELECT column_name(s)FROM table_1JOIN table_2  ON table_1.column_name = table_2.column_name;`       | If the Join condition is TRUE, it is used to merge rows from separate tables.  |
|INSERT    | `INSERT INTO table_name (column_1, column_2, column_3) VALUES (value_1, ‘value_2’, value_3);`      | It is used to insert new rows into a table.   |
|IS NULL/ IS NOT NULL     | `SELECT column_name(s)FROM table_nameWHERE column_name IS NULL;`       | It is an operator used with the WHERE clause to search for empty values.   |
|LIKE    | `SELECT column_name(s)FROM table_nameWHERE column_name LIKE pattern;`      | This special operator is used in conjunction with the WHERE clause to look for a certain pattern in a column.   |
|LIMIT    | `SELECT column_name(s)FROM table_nameLIMIT number;`      | It is a command that defines the maximum number of rows required in the result set.  |
|MAX     | `SELECT MAX(column_name)FROM table_name;`      | It is a function that accepts a number of columns as an input and returns the one with the highest value.  |
|MIN     | `SELECT MIN(column_name)FROM table_name;`      | This function takes as an argument a number of columns and returns the smallest value among them.   |
|OR     | `SELECT column_nameFROM table_nameWHERE column_name = value_1   OR column_name = value_2;`      | It acts as a filter operator employed in order to limit the result set to rows when either condition is TRUE.   |
|ORDER BY     | `SELECT column_nameFROM table_nameORDER BY column_name ASC;`       | It is a clause used to sort the result set numerically or alphabetically by a certain column. in this syntax *ASC* or *DESC* can be used.  |
|OUTER JOIN     | `SELECT column_name(s)FROM table_1LEFT JOIN table_2  ON table_1.column_name = table_2.column_name;`       | Even if the condition is NOT TRUE, it is issued to mix rows from different tables.   |
|ROUND     | `SELECT ROUND(column_name, integer)FROM table_name;`      | It is a function that accepts a column name and an integer as arguments and rounds the entries in a column to the number of decimal places provided by the integer.    |
|SELECT     | `SELECT column_name FROM table_name;`       | It is an SQL statement utilized to retrieve information from a database.  |
|SELECT DISTINCT    | `SELECT DISTINCT column_nameFROM table_name;`      | It is used to indicate that the statement is a query, which returns distinct values in the columns supplied.   |
|SUM     | `SELECT SUM(column_name)FROM table_name;`      | This function returns the sum of data from a specific column.   |
|UPDATE     | `UPDATE table_nameSET some_column = some_valueWHERE some_column = some_value;`      | It is used in modifying table rows.   |
|WHERE    | `SELECT column_name(s)FROM table_nameWHERE column_name operator value;`      | It is a clause used to limit the result set to rows when the condition is TRUE.   |
|WITH     | `WITH temporary_name AS (SELECT *FROM table_name)SELECT *FROM temporary_nameWHERE column_name operator value;`      | It is used to utilize an alias to store the result of a certain query in a transient table.   |
|    |       | |

![!SQL Chart](https://github.com/piusnmuhumuza/bootcamp/blob/master/Database%20Adminstration/images/sql-chart.jpg "SQL Chart") *The SQL Chart [sourced from Tech Kage](https://x.com/TheTechKage/status/1727321992494514252?s=20).*

### The SQL Process

When an SQL command is executing for any DBMS, the system figure out the best way to carry out the request and the SQL engine determines that how to interpret the task. In the process, various components are included, and these components can be the _optimization Engine, Query engine,_ and _Query dispatcher_, to mention but a few. All the non-SQL queries are handled by the classic query engine, but SQL query engine won't handle logical files.

#### SQL Query Execution Order

The SQL query execution order refers to how the query clauses are evaluated by the requirements or how to optimize database search results. We use clauses in a specific order, similar to how we plan something step by step and arrive at a desired result.

In SQL, the order in which queries are processed is typically defined by the logical query processing order which is different from the order in which the SQL statements are written in the query.

Here is the general logical order in which SQL queries are processed:

1. **FROM clause:**
The data sources (tables, views, etc.) specified in the FROM clause are processed first.
This involves reading the data from the tables and combining data from multiple sources if there are joins.

2. **WHERE clause:**
The WHERE clause is applied to filter the rows based on the specified conditions.
Rows that do not meet the criteria in the WHERE clause are excluded from further processing.

3. **GROUP BY clause:**
If a GROUP BY clause is present, rows are then grouped based on the specified columns.
Aggregate functions (like SUM, COUNT, AVG) are then applied to each group.

4. **HAVING clause:**
If a HAVING clause is present, it filters groups based on aggregate conditions.
Groups that do not meet the criteria in the HAVING clause are excluded.

5. **SELECT clause:**
The SELECT clause is then applied to the result set.
Columns are selected, and expressions are computed.

6. **ORDER BY clause:**
If an ORDER BY clause is present, the result set is then sorted based on the specified columns.

7. **LIMIT/OFFSET (if applicable):**
If there is a LIMIT or OFFSET clause _(used in some database systems)_, the final result set is then limited or offset accordingly.

### Other Notable Database Languages

- **SQL/XML**

The SQL/XML language is a combination of SQL and XQuery that supports the manipulation and storage of XML data in a database that works with SQL. It enables applications to perform SQL statements on XML data and vice versa.

 It's helpful when you want to extract content from an XML document or if you want to ensure compatibility with future optimizations or systems that may only support XML. (**XML Query Language (XQuery)**)

- **XQuery**

XQuery is a query and functional programming language that was designed by the World Wide Web Consortium (W3C)**[ responsible for framing XQuery 1.0.]** to meet specific requirements for querying and modifying XML data as well as processing XML documents. 

XQuery ([XML Query](https://en.wikipedia.org/wiki/XQuery)) queries and transforms collections of structured and unstructured data, usually in the form of XML, text and with vendor-specific extensions for other data formats (JSON, binary, etc).

Unlike relational data, which is predictable and has a regular structure, XML data is highly variable. XML data is often unpredictable, sparse, and self-describing.

Because the structure of XML data is unpredictable, the queries that you need to perform on XML data often differ from typical relational queries.

The XQuery language provides the flexibility required to perform these kinds of operations. For example, you might need to use the XQuery language to perform the following operations:

- Search XML data for objects that are at unknown levels of the hierarchy.
- Perform structural transformations on the data (for example, you might want to invert a hierarchy).
- Return results that have mixed types.
- Update existing XML data.

XML data and other databases that store data in a format analogous to HTML can be processed with XQuery. The main objective of XQuery is to provide query mechanisms for data extraction from real and virtual Web-based documents. It aims to link Web and database technologies with the help of XML.

- **OQL**

OQL, which stands for Object Query Language, is the standard language for object-oriented databases, which represent data as variables, functions or data structures.

These databases are popular with companies that want to store large amounts of complex data. Much like SQL does in relational databases, OQL gives you the option to perform queries and retrieve data in object databases.

- **GraphQL**

GraphQL is an open-source language that works with APIs, which are interfaces that allow users to interact with data. It provides a way to define the structure of data and how the system returns information in order to prevent the release of excessive amounts of data.

It's helpful when you want to extract data from multiple APIs, aggregate data from different sources or specify the data efficiently.

- **LINQ**

LINQ, or Language Integrated Query, is a language that extracts and processes data from XML documents, relational databases and other third-party sources.

With LINQ, you can access data through various sources without having to use a separate database language for each one. This ensures consistency among queries for objects, relational databases and XML, allowing you to filter, order and group operations.

### Query Optimization

SQL developers, database administrators (DBAs), database architects, database designers, and even data analysts use SQL statements to interact with databases in various way like adding or retrieving data, and if you've worked with databases in any of these roles for any amount of time then you've encountered slow running queries.

Sometimes the reason for the slow response time is due to the load on the system, and other times it is because the queries being run have not been written to perform as efficiently as possible.

It goes without saying inefficient queries can significantly degrade even the most powerful infrastructure's performance if left unchecked which is why Query optimization is an important skill for SQL developers and database administrators (DBAs).

Optimizing queries involves improving the efficiency and performance of SQL queries to retrieve data more quickly while consuming fewer resources. Techniques like _indexing, query re-writing, proper data modeling_ can enhance query execution speed.
e.g.,

```sql
-- Index Example
CREATE INDEX idx_customer_name ON customers (name);
```

```sql
-- Query Faster Example
SELECT customers.name, orders.order_date
FROM customers
JOIN orders ON customer.id = orders.customer_id;
```

```sql
-- Analyzing Query Performance Example
EXPLAIN SELECT * FROM employees;
```

Query tuning involves knowledge of techniques such as cost-based and heuristic-based optimizers, plus the tools an SQL platform provides for explaining a query execution plan.

Because Query optimization has a very big impact on the performance of a DBMS, developers and DBAs need to understand the query optimizer and the techniques it uses to select an access path and prepare a query execution plan, in order to improve the performance of SQL queries. 

Understanding execution plans and analysing query performance can help identify bottlenecks and optimize queries for better overall performance.

### Filtering & Sorting Data

- Filtering allows users to extract specific data from a table based on specified conditions using the WHERE clause.
e.g;-
  **A simple query for Filtering Data**

```sql
SELECT * 
FROM bakery.employees
WHERE salary > 40000 AND department = Barkey;
```

- Sorting arranges the data in a particular order (*ascending or descending*) based on one or more columns using the ORDER BY clause.

e.g;-
  **A simple query for Sorting Data**

```sql
SELECT * 
FROM bakery.employees
ORDER BY department ASC, title DESC;
```

### Grouping & Aggregating Data

- Grouping data combines rows with similar values in a specified column, allowing you to perform calculations or analysis on subsets of data.

- Aggregation functions _(e.g., SUM, AVG, COUNT)_ calculate summary values from grouped data, providing insights into data trends or patterns.
e.g;-

```sql
SELECT department, AVG(salary) AS salary
FROM bakery.employees
GROUP BY department;
```

- Grouping and aggregating are useful for generating reports, performing statistical analysis, or summarizing large datasets.

### Joins and Subqueries

- Joins combine rows from two or more tables based on related columns, allowing you to retrieve data from multiple tables simultaneously.

- Different types of joins *(e.g., INNER JOIN, LEFT JOIN, RIGHT JOIN)* define how the tables are matched and combined.
e.g.,

```sql
SELECT c.firstname_name, c.last_name, co.profuct_id, co.order_total
FROM bakery.customers c
JOIN bakery.customer_orders co
ON c.customer_id = co.customer_id;
```

Check out the [SQL Joins](#sql-joins) section for more explaination & examples.

- Subqueries are queries nested within other queries, providing a way to break down complex tasks and retrieve data based on intermediate results.
e.g.,

```sql
SELECT * 
FROM bakery.customers
WHERE customer_id IN (
                SELECT customer_id
                FROM bakery.ordered_items
);
```

- When working with large datasets then its better to use Joins over subqueries, as joins are faster.

### Window Functions

- Window functions allow you to perform calculations and aggregations over a specific window or subset of rows within a result set.

- They provide advanced analytical capabilities, such as calculating running totals, ranking, and finding moving averages.

- Window functions are often used in data analysis, reporting, and generating complex summary reports.
e.g.,

```sql
-- Window Function Example
SELECT first_name, salary,
RANK() OVER (ORDER BY salary DESC) AS salary_rank,
DENSE_RANK() OVER (ORDER BY salary DESC) AS salary_dense_rank,
ROW_NUMBER() OVER (ORDER BY salary DESC) AS salary_rank
FROM employees;
```

### SQL Indexing

Most databases require some form of indexing to keep up with performance benchmarks. A database index/SQL index is a lot like the index on the back of a book.

It saves you time and energy by allowing you to easily find what you're looking for without having to flick through every page. 

Database indexes work the same way thus making searching through a database is much simpler when the data is correctly indexed.

#### What is an Index?

An SQL index is a data structure that enhances the speed of data retrieval operations on a database table. This is achieved by creating a separate data structure that stores a subset of the table's columns, organized for optimized query performance. Think of it like having a map to navigate the data quickly.

Think of an index as a database object used to speed up the retrieval of rows from a table by creating a sorted list of values from one or more columns. It is a key-value pair where the key is used to search for data instead of the corresponding indexed column(s), and the value is a pointer to the relevant row(s) in the table.

To create an index in SQL, you typically use the CREATE INDEX statement and it is essential to name your indexes meaningfully and keep them updated as your data evolves.

Indexes provide an ordered representation of the data independent of where data is stored which dramatically reduce the time needed to search for specific data _(the look-up time of requested data)_ within large datasets, but the increase in reads performance comes with a trade-off. Like the need for additional storage and write operations some times becoming slower.

Although their usage requires careful planning to strike the right balance between read and write operations, too many indexes or improper use can lead to unintended consequences. It's therefore good to have the right indexing strategy.

Indexes are one of the most critical concepts for databases because without then, every query would require scanning the entire table, which is inefficient and time-consuming. They significantly enhance query performance, but their usage requires careful planning to strike the right balance between read and write operations and using them effectively, requires database users to know how they work.

#### Some Indexing Use cases

- The B-tree is one of the most commonly used indexing structures where keys are hierarchically sorted. When searching data, the tree is traversed down to the leaf node that contains the appropriate key and pointer to the relevant rows in the table. B-tree is most commonly used because of its efficiency in storing and searching through ordered data. Their balanced structure means that all keys can be accessed in the same number of steps, making performance consistent.

- Bitmap indexing is used for columns with few unique values. Each bitmap represents a unique value. A bitmap indicates the presence or absence of a value in a dataset, using 1’s & 0’s. For existing values, the position of the 1 in the bitmap shows the location of the row in the table. Bitmap indexes are very effective in handling complex queries where multiple columns are used.

- Hash indexes are best used when you are searching for an exact value match. The key component of a hash index is the hash function. When searching for a specific value, the search value is passed through a hash function which returns a hash value. That hash value tells the database where the key and pointers are located in the hash table.

- A composite index may be used when multiple columns are often used in a WHERE clause together. With a composite index, a combination of two or more columns are used to create a concatenated key. The keys are then stored based on the index strategy, such as the options mentioned above.

### SQL Views

A view is a virtual representation of an actual table that you can assemble up to your liking (before adding the actual one to your database). It features rows and columns, just like the real deal and can contain fields from one or more of the real tables from your database.

Views are a good way to visualize and review data coming from different tables within a single screen as they are just SQL statements stored in the database with an associated name.

A view can contain all rows of a table or selected rows from a table and can be created from one or many tables.

### SQL Unions

These are ```UNION```, ```UNION ALL``` and ```INTERSECT```.

- **UNION Operator**

The ``UNION`` operator is used to combine the result-set of two or more ``SELECT`` statements.

- Every ``SELECT`` statement within ``UNION`` must have the same number of columns.
- The columns must also have similar data types and columns in every ``SELECT`` statement must also be in the same order.
- The ``UNION`` operator selects only distinct values by default. To allow duplicate values, use ``UNION ALL``.

- **INTERSECT operator**

The ``INTERSECT`` operator is used to retrieve only the common rows that appear in the result sets of two or more ``SELECT`` queries.

- The columns in the ``SELECT`` queries must have compatible data types and appear in the same order.
- Unlike ``UNION``, ``INTERSECT`` does not remove duplicate rows from the result set. If there are duplicate rows in the individual result sets, they will all be included in the final result.
- MySQL does not have a built-in ``INTERSECT`` operator. To achieve the same functionality as ``INTERSECT``, you would need to use subqueries or other techniques to find the common
rows between two or more ``SELECT`` statements.

### SQL JOINS

Joins is are a powerful technique in SQL that allows us to query and retrieve data from multiple/different tables simultaneously by combining rows from two or more tables based on related columns.

#### Types of SQL Joins

Different types of joins _(e.g., INNER JOIN, LEFT JOIN, RIGHT JOIN)_ define how the tables are matched and combined.

- An **INNER JOIN** is a type of join that returns only the matching rows from both tables. Forexample, given **_Table A_** & **_Table B_**, an **Inner join** will return only the set of records that match in both **_Table A_** and **_Table B_** or the records that have matching values in both the left and right tables.

It's like finding the intersection of two sets. Perfect for retrieving data that share common values in specified columns!

Example: Inner join tA and tB, where **_tA_** is *Table A* & **_tB_** is *Table B*.

```SQL
SELECT c1, c2 FROM tA INNER JOIN tB ON condition;
```

- A **NATURAL JOIN** is just an inner equi-join where the join is implicitly created using any matching columns between the two tables

Example:

```sql
SELECT * FROM TableA NATURAL JOIN TableB
```

Natural joins automatically join tables based on column names, while inner joins require explicitly specifying the join columns in the ``ON`` or ``USING`` clause. Natural join returns only one instance of a common join column, while inner join returns duplicate join columns from both tables.

- The **LEFT JOIN or LEFT (OUTER) JOIN** returns all rows from the left table and the matching rows from the right table. This returns all records from the left table and the matched records from the right table. If no match is found, NULL values are returned for columns from the right table.

Left outer join produces a complete set of records from **_Table A_**, with the matching records _(where available)_ in **_Table B_**. If there is no match, the right side will contain null and is useful when you want all the data from the left table, regardless of whether there's a match in the right table.

Example: Left join tA and tB

```sql
SELECT c1, c2 FROM tA LEFT JOIN tB ON condition;
```

- The **RIGHT JOIN (or RIGHT OUTER JOIN)** is similar to the **_LEFT JOIN_** but includes all rows from the right table and the matching rows from the left table. This Join Returns all records from the right table and the matched records from the left table. If no match is found, NULL values are returned for columns from the left table.

Useful when you want all rows from the right table regardless of a match.

Example: Right join tA and tB

```sql
SELECT c1, c2 FROM tA RIGHT JOIN tB ON condition;
```

- A **FULL JOIN (or FULL OUTER JOIN)** returns all records or rows when there is a match in either the left or right table, showing matched records where possible. For unmatched records, it includes NULLs in the columns from the table without a match. It's like combining the results of **_LEFT_** and **_RIGHT JOINs_**.

Example: Perform full outer join

```sql
SELECT c1, c2 FROM tA FULL OUTER JOIN tB ON condition;
```

- The **SELF JOIN** involves joining a table with itself using aliases _(tableA and tableB are the same table with different aliases)_.

Commonly used to compare rows within the same table, for example, in hierarchical structures.

Example:

```sql
SELECT c1,c2

FROM tA A

JOIN tA AS B ON condition;
```

- The **CROSS JOIN** unlike other joins, it doesn't rely on any matching condition. It returns the Cartesian product of the two tables, combining every row from the first with every row from the second.

Example: Produce a Cartesian product of rows in tables

```sql
SELECT c1, c2 FROM tA CROSS JOIN tB;
```

A cross join is a Cartesian Product join – it is every record in Table A combined with every record in Table B. It gives the same results as not using a ``WHERE`` clause when querying two tables in MySQL

```sql
SELECT * from TableA CROSS JOIN TableB

SELECT * from TableA, TableB
```

- An **EQUI-JOIN** is a join operation in SQL that combines two tables based on a matching column between them. Simply put, an Equi Join returns all rows from both tables where the values in the specified columns are equal.

- The **Left Join Excluding Inner Join** will return all of the records in the left table _(table A)_ that do not match any records in the right table _(table B)_.

- The **Right Join Excluding Inner Join** will return all of the records in the right table _(table B)_ that do not match any records in the left table _(table A)_.

- The **Full Outer Excluding Inner Join** will return all of the records in _Table A_ and _Table B_ that do not have a matching record in the other table.

In practice, ``INNER JOIN`` and ``LEFT JOIN`` tend to be the most frequently used, where ``INNER JOIN`` is ideal for retrieving matching data from both tables, and ``LEFT JOIN`` ensures that all records from the left table are included, even if there are no matches in the right table.

You can also combine multiple joins in a single query, in which case you have to use parentheses to define the order of execution and apply your conditions wisely.

But to properly use SQL Joins, you need to ensure that the columns used in join conditions are properly indexed as efficient indexing and proper use of join types can significantly enhance ot impact the performance of your queries by allowing the database to quickly locate and retrieve the matching rows.Therefore, it's important to properly analyze your database schema, choose the right join type, and optimize your queries accordingly.

### SQL Automation

Automation in SQL refers to the process of automating reptitive tasks or operations using scripts, stored procedures, or schedulers. It helps improve efficiency by reducing manual effort and minimizing the chances of human error.

It can be used for tasks like data loading, backups, data transformations, and scheduled report generation.

### Common Table Expressions(CTEs) in SQL

Often time, When working with immense data in SQL, the queries can gradually begin too get complex, necessitating the need to create temporary tables within queries to which you can refer, which is exactly what **Common Table Expressions** do.

All good DBAs should have some knowledge about SQL **CTEs** or Common Table Expressions, their types, usage, and drawbacks and section attempts to briefly explore what SQL Common Table Expressions (CTE) are, how they function among other to knows. And also briefly touch on Subqueries.

#### What are Common Table Expressions (CTEs)?

A Common Table Expression (CTE), is a separate, smaller query or temporary result set within a larger query you’re building that can be used in a SQL query, exsisting only until the query is executed. They are powerful SQL constructs that helps simplify queries by acting as virtual tables in a database a db user can create during query execution, to be used by the query, and then get deleted after the query executes.

As one Vijay Kulkarni but it simply in his elaborate post, [Understanding Common Table Expressions (CTEs)](https://www.linkedin.com/pulse/understanding-common-table-expressions-ctes-vijay-kulkarni-t1tvf), "...while CTEs help organize and simplify SQL queries, they can also slow down performance, especially with complex operations or big datasets. Before using them in production code, weighing factors like query simplicity, speed, and ease of maintenance is crucial.
CTEs help manage complex data tasks at the same time always consider their impact on query performance before implementation."

It is essentially like making a temporary view that you can access throughout the rest of the query you are writing. CTEs break up complex queries into simpler, easy to read blocks of code that can connect and build on each other. And like a derived table, the result of a CTE is not stored and exists only for the duration of the query.

The primary motivation to implement CTEs in your code is to simplify the complexity of your queries and increase your code’s readability. If you are finding yourself using the same code for a certain CTE across multiple queries or models, that’s probably a good sign that CTE should be its own model or view.

CTEs are supported across most, if not all, modern data warehouses, namely;- snowflake, Amazon Redshift, Google BigQuery, Databricks, Postgres.

#### Types of CTEs

There are two-types of CTEs: **recursive** and **non-recursive**.

#### CTE vs Subquery

A subquery is a nested query that enables the integration of one query within another, and can often times be used in place of a CTE. Subqueries have different syntax than CTEs, but often have similar use cases and act as a tool to retrieve data from one table based on conditions derived from another table.

**A subquery can be dissected into distinct components:**

- **Outer Query:** This is the primary query that encloses the subquery. It executes and processes the result produced by the subquery.

- **Inner Query:** The subquery, residing within the outer query, extracts a set of data that's utilized by the outer query for further processing.

**Subqueries can be used to:**

- Add a new column to the main query result
- Create a filter
- Create a consolidated source from which to select the data

**Advantages of using Subqueries include:**

- **Enhanced Readability:** By breaking down complex problems into smaller, more comprehensible chunks, subqueries enhance the readability of SQL code.
- **Precise Filtering:** Subqueries enable precise filtering by allowing the use of aggregate functions and conditional logic.
- **Simplified Maintenance:** By segmenting complex logic, subqueries make the maintenance of SQL code more manageable.

**Disadvantages of using Subqueries include:**

- Intensive computational power is required.
- Longer Loading time.

Often analysts prefer CTEs over sub-queries becauses

- CTEs are more readable since they can be used to give structure to your query while Subqueries are typically less readable, especially if there are many nested queries.
- CTEs allows for recursiveness while Subquries don't.
- CTEs must have unique 'CTE_EXPRESSION_NAMES' when used in a query while Subqueries don’t always have to be explicitly named.
- CTEs cannot be used in a WHERE clause whereas Subqueries can be used in a WHERE clause.

#### CTE vs. Temporary Tables

At the end of this post, you will understand the differences and when to use one over the other.

- CTEs (Common Table Expressions) can make complex queries more readable and easier to maintain and are excellent for breaking down complex queries into simpler, more manageable parts thus most efficient for organizing query logic even though they don't inherently improve performance. Since CTEs do not store their results. They act as temporary views executed every time they are referenced.

- Temporary Tables come with Performance through Persistence where Temporary tables store data in the database's temporary storage (e.g., the tempdb in SQL Server). You can also define indexes on Temporary tables, thus this physical storage and indexes make the reads or joins faster.

CTEs are excellent for organizing and simplifying complex SQL queries without storing intermediate results, making them easy to read and maintain while Temporary Tables are better suited for performance optimization of large datasets, indexing, and reducing the need for repeated computations.

Even though CTEs facilitates readability, the performance on Temporary Tables is really hard to ignore for large datasets.

### Difference between SQL, MySQL and and MsSQL

SQL is a language used for interacting with relational databases, and MySQL is a specific implementation of a relational database management system that uses SQL. MySQL is just one example of a RDBMS that supports SQL.

Several database platforms use SQL, but with slight variations—each tends to have a slightly different syntax. **MySQL** and **Microsoft SQL Server (MSSQL)** are two of the most popular enterprise database systems in the world.

While MySQL is an open-source relational database management system (RDBMS), MSSQL Server RDBMS is developed by Microsoft.

**MySQL** emerged in the mid-1990s as one of the first open-source RDBMS, which significantly contributed to its immense popularity, particularly among startups why **Microsoft SQL Server**, on the other hand, has been around since the 1980s, making it an older product than MySQL. Although it has undergone numerous changes over the years, its core principles remain consistent.

### The difference between SQL and NoSQL

When it comes to choosing a database the biggest decision is picking a relational (SQL) or non-relational (NoSQL) data structure. SQL databases are primarily called Relational Databases (RDBMS); whereas NoSQL databases are primarily called non-relational or distributed databases.

Beyond SQL just being _relational_ and NoSQL being _non-relational_. SQL is structured query language used for relational databases, while NoSQL encompasses various database technologies like document stores _(each document can have its own schema. The problem with that approach is that your application must be able to handle all these different schemas without breaking things. It becomes harder if multiple apps write to the db and don't know each other's format.)_ or key-value pairs.

Each has its strengths and Weakness. For example the some of the key difference between SQL and No-SQL are:

- Relational databases which can be accessed with SQL (Structured Query Language) were developed in the 1970s with a focus on reducing data duplication as storage was much more costly than developer time while NoSQL _(“non SQL” or “not only SQL”)_ databases were developed in the late 2000s with a focus on scaling, fast queries, allowing for frequent application changes, and making programming simpler for developers.

- SQL uses a relational data model _(table-based)_ where data is stored in tables with rows and columns while NoSQL offers a variety of data models including key-value pairs, document-based, wide-column stores, and graph models.

- SQL requires you to use predefined schemas to determine the structure of your data before you work with it while NoSQL databases have a dynamic schemas for unstructured data thus their data is stored in many ways such as document-oriented, column-oriented, graph-based, or organized as a key-value stores. in other words, SQL enforces a strict schema with predefined tables, columns, and data types, making it more suitable for structured data while NoSQL typically use a dynamic schema, perfect for unstructured or evolving data.

- SQL Databases uses Structured Query Language (SQL) to perform operations such as data retrieval, insertion, update, and deletion, and excel at performing complex queries across multiple tables while NoSQL databases do not have a standard query language, thus each NoSQL database may have its query syntax or API, depending on its data model.

- SQL primarily scales vertically by increasing the hardware resources _(CPU, RAM, SSD)_ of a single server while NoSQL is designed for horizontal scalability, allowing distribution of load across multiple servers.

- SQL is optimized for complex queries and joins across multiple tables which can sometimes lead to slower performance for certain types of queries, especially as data volume grows while NoSQL is designed for high-performance, simple read/write operations. By denormalizing data and optimizing for specific access patterns, NoSQL databases can achieve extremely low latency for certain operations.

- SQL provides strong support for ACID transactions _(Atomicity, Consistency, Isolation, Durability)_, ensuring data validity even in the event of errors, and power failures, thus choosing consistency over availability while Many NoSQL databases uses BASE sacrifice ACID compliance for scalability and availability over consistency, although, some NoSQL databases offer tunable consistency models.

- SQL is well-suited for applications requiring complex queries and transactions, such as financial systems, e-commerce platforms, and applications with strong data consistency requirements while NoSQL is used in scenarios involving large volumes of rapidly changing, unstructured data, such as real-time web applications, IoT data processing, and big data analytics.

## DATABASE HASHING

Hashing is the process of transforming any given key or a string of characters into another value. This is usually represented by a shorter, fixed-length value or key that represents and makes it easier to find or employ the original string.

### Hashing in DBMS

It can be nearly hard to search all index values through all levels of a large database structure and then get to the target data block to obtain the needed data. The hashing method is basically used to index items and retrieve them in a Database since searching for a specific item using a shorter hashed key rather than the original value is faster.

It's A DBMS technique for searching for needed data on the disc without utilising an index structure and a method for calculating the direct position of an information record on the disk without the use of an index structure.

To generate the actual address of a data record, hash functions containing search keys as parameters are used.

### Properties of Hashing in DBMS

Data is kept in data blocks whose addresses are produced using the hashing function in this technique. Data buckets or data blocks are the memory locations where these records are stored.

In this case, a hash function can produce the address from any column value. The primary key is frequently used by the hash function to generate the data block’s address. To every complex mathematical function, a hash function is a basic mathematical function. The primary key can also be considered as the data block’s address, i.e. each row with the same address as a primary key contained in the data block.

The data block addresses are the same as the primary key value in the picture above. This hash function could alternatively be a simple mathematical function, such as exponential, mod, cos, sin, and so on. Assume we’re using the ``mod (5)`` hash function to find the data block’s address. In this scenario, the primary keys are hashed with the ``mod (5)`` function, yielding ``3, 3, 1, 4,`` and ``2``, respectively, and records are saved at those data block locations.

### Hash Organization

- **Bucket** – A bucket is a type of storage container. Data is stored in bucket format in a hash file. Typically, a bucket stores one entire disc block, which can then store one or more records.

- **Hash Function** – A hash function, abbreviated as h, refers to a mapping function that connects all of the search-keys K to that address in which the actual records are stored. From the search keys to the bucket addresses, it’s a function.

### Types of Hashing

Hashing is of the following types:

#### Static Hashing

Static hashing refers to a hashing technique that allows users to execute lookups on a dictionary set that has been finalised _(all the objects present in the dictionary are final and do not change)_.

Whenever a search-key value is given in static hashing, the hash algorithm always returns the same address. If the mod-4 hash function is employed, for example, only 5 values will be generated. For this function, the output address must always be the same. At all times, the total number of buckets available remains constant. Click here to learn more about static hashing.

#### Dynamic Hashing

Dynamic hashing is a mechanism for dynamically adding and removing data buckets on demand. The hash function aids in the creation of a huge number of values in this hashing.

The disadvantage of static hashing is that it doesn’t expand or contract dynamically as the database size grows or diminishes. Dynamic hashing is a technology that allows data buckets to be created and withdrawn on the fly. Extended hashing is another name for dynamic hashing.

In dynamic hashing, the hash function is designed to output a huge number of values, but only a few are used at first. Click here to learn more on dynamic hashing.

## THE DATABASE DESIGN PROCESS

1. The **Requirements Collection And Analysis Phase** involves understanding and documenting the necessary data requirements of the database users. The outcomes of this step is for the database designer to have a high level understanding of the various data requirements and functional requirements.

2. The **Functional Requirements Phase** is where the data designer finds out and defines the user-defined operations applied to the database. The outcome here is to have a high-level transaction specification.

3. The **Conceptual Design Phase** entails creation of a conceptual schema using high level conceptual data models for the database. This is essentially a data model providing concepts depicting how users perceive the data to be used in the database being designed. A conceptual schema is a concise description of the data requirements and detailed description of the entity types, relationships and constraints. This schema should be understandable and explainable to nontechnical people.

4. The **Logical Design Phase**
This is the actual implementation of the database, using a DBMS e.g MsSQL, MySQL, NoSQL etc. At this point the conceptual schema s transformed from a high level model to a database schema through Data model mapping.

5. The **Physical Design Phase** is where the internal storage structures, indexes, access paths etc are specified, application programs are designed and implemented as transactions corresponding to the high level transaction specifications from the functional requirements step.

## DATABASE SECURITY

Database security refers to the measures taken to protect databases from unauthorized access, use, disclosure, disruption, modification, or destruction. Databases contain sensitive information, such as customer data, financial data, and intellectual property. As such, it is important to protect them from unauthorized access.

Database Security explores concepts like _The need to secure a database, What objects can be secured, What Objects should be secured, User accounts, and Roles among other aspects of database administration.

### Security Features

These features(Authentication, Authorization, Availability, Integrity, Encryption, Recovery)ensure data Security for all senstive data that is being stored to, accessed and used from the various databases of an organisation or business.

- **Authentication** is essentially the process of confirming identity.
- **Authorization**  is the set of controls incorporated in data management systems rstricting access to data and/or actions performed by certain or desiginated users.

  - always apply the rule of least priviledges.
  - granting execute priviledges on procedures with no direct table access(Authorization Matrix).
  - Apply Application access assessment using a CRUD (**C=Create(Insert), R=Read(Select), U=Update, D=Delete**) Report/Matrix.
  - Restrict access to data contained in individual records(Row-level Access Control).

- **Availability** ensures that designated/authorised users or other parts of a system have the required continous access to the database to perform/complete their tasks.

- **Intergrity** ensures that database information is and remains intact and valid at all times during its lifetime. Some common integrity threats include SQL Injections _(Malicious code that tricks a database into executing unintended commands usually through input validation & data access vulnerabilities)._

- **Encryption** is the process of encoding messages or information in such a way that only authorized parties can read it. _(Hashing & Salting passwords are good examples.)_

- **Recovery** is the use of journalizing facilities to provide audit trails of transactions and database updates. _(Have a Disaster Recovery Plan)_

### Security Principles

- Development of a security plan should occur early in the development of a database. Security must be carefully designed, implemented and tested.

- A Security plan depends heavily on the size and nature of the database as well as its business requirements.

- In a database, different objects _(databases, tables, logins, user roles)_ can be subject to permission and rights based on who, where and for what or reason for access.

- A simplified security model would look like;- A user logins into a database server using a login ID and based on the Information in the master database about who, what, where, etc and the user ID can then be granted access to objects based on role permissions set by the database administrator. _E.g a guest, auditor, or analyst may have limited access compared to a DBA or database administrator_.

- In database security, there is what we call, server-level security which is essentially defining how users get access to the database server via available defined methods e.g user logins, memberships or group access, etc. A login is controlled by a user's credentials, often a username and password and once logged in, users will be known at the server-level by their login and the user-rights are determined by fixed roles that are server granted, revoked or otherwise.

### Roles

- Fixed server roles include;- sysadmin, serveradmin, securityadmin, procssadmin, setupadmin, bulkadmin, diskadmin, dbcreator and vary based on the database type.

- Other roles include;- the public role that is a fixed role but can have object permission like a standard role. Every user is automatically a member of the public roles and cannot be removed because the public role is the baseline level of permission. The SQL Server authentication mode used is setup when the SQLSERVER is installed and the windows authentication mode only as windows authentication is allowed while in mixed mode both windows & SQLSRVER authentications are allowed.

- Fixed database roles.

- Database objects include tables, views, stored procedures and columns. Every object is contained by a schema. A schema is owned and everything within the schema has an owner.

- A user may have access to a database but can and has to be granted permission to the individual database objects. Permissions maybe granted directly to the user or by assigning the permission to the role and assigning the user to the role, a preferred approach to security in relation to object permissions. Users may be assigned to multiple roles, thus there maybe multiple permission roles.

- Object permissions assigned/revoked/denied by means of GRANT, REVOKE and DENY, where by GRANT gives/assigns permissions, REVOKE removes permissions assigned, and DENY overrules GRANT. A user may have multiple permissions paths to an object.

**There are a number of ways to protect databases from security threats of which the most common methods include:**

- **Data encryption**, a process of converting data into a form that cannot be read without a special key, making it difficult for unauthorized users to access the data, even if they manage to gain access to the database itself.

- **Access control** a process of restricting who has access to the database and what they can do with it. This can be done by using usernames and passwords, as well as by implementing **_role-based access control (RBAC)_**.

- Enforcing **Physical security measures**, such as locked doors and security cameras, can help to protect the database from physical attacks.

- Doing regular **Data backup and recovery**, which is a process of creating copies of data and restoring it in case of a security breach or other disaster. This ensures that the data can be recovered even if it is lost or corrupted.

- **Database auditing**, a process of tracking changes to the database, that can help identify unauthorized access or changes to the data.

Now implementing these security measures doesn't make your databases systems 100% secure, but can go a long way to help orgainsations protect their databases systems from many security threats by ensuring some form of _confidentiality, integrity,_ and _availability_ of their senitive or critical business data.

**Databases Administrators can also follow some of the best practices below to ensure database security:**

- Always using strong passwords and passphrases that are atleast 8+ characters long as well as include a mix of upper and lowercase letters, numbers, and symbols. And these Passwords should be changed regularly, at least every 90 days.

- Using multi-factor authentication whenever possible. Multi-factor authentication adds an extra layer of security by requiring users to provide two or more pieces of identification, such as a password and a code sent to their phone.

- Database administrators and other database users need to continously keep database software as well as software around/has access it up to date. Software updates often include security patches that can help to protect against known vulnerabilities.

- Monitoring database activity should be one of the database administrator/ any database custodian's top daily to-do to flag any signs of unauthorized access, changes to the data or other forms of misuse on an organisation's database systems and related resources.

- It is also important to regularly back up databases. Database backups be done as part of a company's backup and recovery plan which should clearly define in what intervals database backups should regularly take place. This ensures that the data can be restored in case of a security breach or other disaster.

## BUSINESS INTELLIGENCE

The rise of Big Data and the availability of new tools and techniques, businesses have learned how to use information to their advantage.

The term business intelligence is used to describe the process that organizations use to take data they are collecting and analyze it in the hopes of obtaining a competitive advantage.

Besides using their own data, stored in data warehouses, firms often purchase information from data brokers to get a big- picture understanding of their industries and the economy. The results of these analyses can drive organizational strategies and provide competitive advantage.

### Transactional Data and Analytical Data processing

Data is at the core of most software applications and solutions. It can be represented in many formats, stored in files and databases, and used to record transactions or to support analysis and reporting.

- **Transactional Data Processing**

A transactional data processing system is what most people consider the primary function of business computing. A transactional system records transactions that encapsulate specific events that the organization wants to track. A transaction could be financial, such as the movement of money between accounts in a banking system, or it might be part of a retail system, tracking payments for goods and services from customers.
Think of a transaction as a small, discrete, unit of work.

Transactional systems are often high-volume, sometimes handling many millions of transactions in a single day. The data being processed has to be accessible very quickly. The work performed by transactional systems is often referred to as Online Transactional Processing (OLTP).

OLTP solutions rely on a database system in which data storage is optimized for both read and write operations in order to support transactional workloads in which data records are created, retrieved, updated, and deleted (often referred to as CRUD operations). These operations are applied transactionally, in a way that ensures the integrity of the data stored in the database.

To accomplish this, OLTP systems enforce transactions that support so-called ACID semantics. **ACID** Is a concept in databases transactions which stands for _Atomicity, Consistency, Isolation, Durability_.

OLTP systems are typically used to support live applications that process business data - often referred to as line of business (LOB) applications.

- **Analytical Data Processing**

Analytical data processing typically uses read-only (or read-mostly) systems that store vast volumes of historical data or business metrics. Analytics can be based on a snapshot of the data at a given point in time, or a series of snapshots.

The specific details for an analytical processing system can vary between solutions but a common architecture for enterprise-scale analytics looks like this:

- Operational data is extracted, transformed, and loaded (ETL) into a data lake for analysis.

- Data is loaded into a schema of tables - typically in a Spark-based data lakehouse with tabular abstractions over files in the data lake, or a data warehouse with a fully relational SQL engine.

- Data in the data warehouse may be aggregated and loaded into an online analytical processing (OLAP) model, or cube. Aggregated numeric values (measures) from fact tables are calculated for intersections of dimensions from dimension tables. For example, sales revenue might be totaled by date, customer, and product.

- The data in the data lake, data warehouse, and analytical model can be queried to produce reports, visualizations, and dashboards.

Data lakes are common in large-scale data analytical processing scenarios, where a large volume of file-based data must be collected and analyzed.

An OLAP model is an aggregated type of data storage that is optimized for analytical workloads. Data aggregations are across dimensions at different levels, enabling you to drill up/down to view aggregations at multiple hierarchical levels; for example to find total sales by region, by city, or for an individual address. Because OLAP data is pre-aggregated, queries to return the summaries it contains can be run quickly.

### Data Warehouses

This is a system that intergrates data from multiple different kinds of systems for business uses. It typically stores data in dimensional form which is de-normalised. It is a form of relational database designed for OLAP _(Online Analytical Process)_. The key difference between a transactional system and a data warehouse is that Data warehouses store and maintain history data.

Data warehouses are an established way to store data in a relational schema that is optimized for read operations – primarily queries to support reporting and data visualization and are mostly used for Analytics, Reporting and Business Intelligence(BI) to store current and historial data, summarised and refreshed from source systems. They can be normalised but it's not a very popular option and beats the purpose.

The concept of the data warehouse is simple: extract data from one or more of the organization’s databases and load it into the data warehouse (which is itself another database) for storage and analysis. However, the execution of this concept is not that simple.

#### Data Warehouse Designed Criteria

A data warehouse should be designed so that it meets the following criteria:

- It uses non-operational data. This means that the data warehouse is using a copy of data from the active databases that the company uses in its day-to-day operations, so the data warehouse must pull data from the existing databases on a regular, scheduled basis.

- The data is time-variant. This means that whenever data is loaded into the data warehouse, it receives a time stamp, which allows for comparisons between different time periods.

- The data is standardized. Because the data in a data warehouse usually comes from several different sources, it is possible that the data does not use the same definitions or units. For example, each database uses its own format for dates _(e.g., mm/dd/yy, or dd/mm/yy, or yy/mm/dd, etc.)_. In order for the data warehouse to match up dates, a standard date format would have to be agreed upon and all data loaded into the data warehouse would have to be converted to use this standard format. This process is called extraction-transformation-load (ETL).

#### The Bottom-Up and Top-Down Data warehouse Design Approachs

There are two primary schools of thought when designing a data warehouse: bottom-up and top-down.

- The bottom-up approach starts by creating small data warehouses, called data marts, to solve specific business problems. As these data marts are created, they can be combined into a larger data warehouse.

- The top-down approach suggests that we should start by creating an enterprise- wide data warehouse and then, as specific business needs are identified, create smaller data marts from the data warehouse.

#### Benefits of Data Warehouses include

- The process of developing a data warehouse forces an organization to better understand the data that it is currently collecting and, equally important, what data is not being collected.

- A data warehouse provides a centralized view of all data being collected across the enterprise and provides a means for determining data that is inconsistent.

- Once all data is identified as consistent, an organization can generate “one version of the truth”. This is important when the company wants to report consistent statistics about itself, such as revenue or number of employees.

- By having a data warehouse, snapshots of data can be taken over time. This creates a historical record of data, which allows for an analysis of trends.

- A data warehouse provides tools to combine data, which can provide new information and analysis.

### Operational Data Stores (ODS)

An Operational Data store(ODS) is a central database that provides a snapshot of the latest data from multiple transactional systems for operational reporting. 

It can sit in-between data sources and enterprise data warehouses, where it can be used to prepare data for storage in the data warehouse. In this way, the ODS works as a part of data warehousing strategy instead of replacing it.

Operational Data Stores contain the latest and most current operational data, providing  useful snapshot of business operations as they are in the moment from multiple sources typically used for reporting purposes. 

Often called Systems of Records (***Data Origination Systems***), ODS enables organisations to combine data in its original format from various sources into a single destination to make it available for business reporting.

### Data Marts

Data Mart is a popular data store considered as a sub-set of a data warehouse and is domain or subject oriented catering to a single business. A data mart is a structure/access pattern specific to data warehouse environments, used to retrieve client-facing data. Because it's usually dimensional in nature, it's therefore at times called a ***dimensional data mart***.

Data Marts in essence are a simple form of data warehouses focused on a single subject or line of business, such as sales, finance, or marketing drawing data from fewer sources than data warehouses.

### Data Lakes

Data Lakehouses are a more recent innovation that combine the flexible and scalable storage of a data lake with the relational querying semantics of a data warehouse. The table schema may require some denormalization of data in an OLTP data source (introducing some duplication to make queries perform faster).

A data lake is a centralised repository designed to store, process, and secure large amounts of structured data from relational databases ***(rows & columns)***, semi-structured ***(CSV,Logs, XML, JSON)***, and unstructured data ***(images, audio, video)***. It can store data in its native format and process any variety of it, ignoring size limit.

Where designed/made for large amounts of data, desinged to capture raw data (***Structured, Semi-structured & unstructured***). Data Lakes are used for ML & AI in its current state. Data from Data Lakes can be organised and put into Databases or Data Warehouses.

While a data lake stores current and historical data for one or more systems in its raw form for the purpose of analysing the data, a database stores current data required to power an application and data warehouses store structured data

Different types of users might perform data analytical work at different stages of the overall architecture. 

For example:

- Data scientists might work directly with data files in a data lake to explore and model data.

- Data Analysts might query tables directly in the data warehouse to produce complex reports and visualizations.

- Business users might consume pre-aggregated data in an analytical model in the form of reports or dashboards.

### What Is ETL?

Extract, transform, load (ETL) is a foundational process in data engineering that underpins every data, analytics and AI workload.  “extract, transform, load,” are the three interdependent processes of data integration used to pull data from one database and move it to another. Once loaded, data can be used for reporting, analysis, and deriving actionable business insights.

#### ETL Pipelines

An ETL pipeline is the set of processes used to move data from a source or multiple sources into a database such as a data warehouse.

As data warehouses and data lakes continue to evolve and other technologies like data lakehouses emerge, data engineers also need to continuosly improve a theri understanding of ETLs other might encounter challenges such as handling real-time data ingestion, ensuring data quality, pipeline orchestration and observability to mention but a few.

ETL pipelines purposefully prepares data for analytics and business intelligence in order to provide valuable insights, from source data coming from various systems _(CRMs, social media platforms, Web reporting, etc.,)_ that often needs to be moved, consolidated and altered to fit with the parameters and functions of the destination database.

**An ETL Pipeline is helpful for:**

- Data migration from legacy systems to data warehouses, that way providing a way of centralizing and standardizing data, making it readily available to analysts and decision-makers.

- Deeper analytics after exhausting the insights provided by basic transformation.

- Freeing up developers from technical implementation tasks for data movement and maintenance, allowing them to focus on more purposeful work.

#### Characteristics Of an ETL Pipeline

- The different aspects of ETL including data ingestion, transformation and orchestration.

- Best practices for dealing with pipeline issues, improving efficiency and scalability

The enterprise shift to cloud-built software services combined with improved ETL pipelines offers organizations the potential to simplify their data processing.

 Companies that currently rely on batch processing can now implement continuous processing methodologies without disrupting their current processes. 
 
 Instead of costly rip-and-replace, the implementation can be incremental and evolutionary, starting with certain types of data or areas of the business.

Ultimately, ETL pipelines enable businesses to gain competitive advantage by empowering decision-makers.

**To do this effectively, ETL pipelines should:**

- Provide continuous data processing
- Be elastic and agile
- Use isolated, independent processing resources
- Increase data access
- Be easy to set up and maintain

#### How Does ETL work?

- **Extract**

The first step of this process is extracting data from the target sources that are usually heterogeneous such as business systems, APIs, sensor data, marketing tools, and transaction databases, and others. As you can see, some of these data types are likely to be the structured outputs of widely used systems, while others are semi-structured JSON server logs.

**There are different ways to perform the extraction, and here are three Data Extraction methods to consider:**

1. **Partial Extraction** – The easiest way to obtain the data is if the if the source system notifies you when a record has been changed.

2. **Partial Extraction (with update notification)** - Not all systems can provide a notification in case an update has taken place; however, they can point to those records that have been changed and provide an extract of such records.

3. **Full extract** – There are certain systems that cannot identify which data has been changed at all. In this case, a full extract is the only possibility to extract the data out of the system. This method requires having a copy of the last extract in the same format so you can identify the changes that have been made.

- **Transform**

The second step consists of transforming the raw data that has been extracted from the sources into a format that can be used by different applications. In this stage, data gets cleansed, mapped and transformed, often to a specific schema, so it meets operational needs.

This process entails several types of transformation that ensure the quality and integrity of data Data is not usually loaded directly into the target data source, but instead it is common to have it uploaded into a staging database. This step ensures a quick roll back in case something does not go as planned.

During this stage, you have the possibility to generate audit reports for regulatory compliance, or diagnose and repair any data issues.

- **Load**

Finally, the load function is the process of writing converted data from a staging area to a target database, which may or may not have previously existed. Depending on the requirements of the application, this process may be either quite simple or intricate. Each of these steps can be done with ETL tools or custom code.

### Data Mining and Machine Learning

Data mining is the process of analyzing data to find previously unknown and interesting trends, patterns, and associations in order to make decisions. Generally, data mining is accomplished through automated means against extremely large data sets, such as a data warehouse.

An example of data mining can be A basketball organisation's scouting team aggregating data that may find that high school and college players with specific statistics in TS%, rebounding, assist, steals,  low TO% among other intangibles make for more successful professional league players than one-dimensional players.

One data mining method that organizations are using to do these analyses is called machine learning.

Machine learning is used to analyze data and build models without being explicitly programmed to do so. Two primary branches of machine learning exist: supervised learning and unsupervised learning.

- Supervised learning occurs when an organization has data about past activity that has occurred and wants to replicate it. For example, if they want to create a new marketing campaign for a particular product line, they may look at data from past marketing campaigns to see which of their consumers responded most favorably. Once the analysis is done, a machine learning model is created that can be used to identify these new customers. It is called “supervised” learning because we are directing (supervising) the analysis towards a result (in our example: consumers who respond favorably). Supervised learning techniques include analyses such as decision trees, neural networks, classifiers, and logistic regression.

- Unsupervised learning occurs when an organization has data and wants to understand the relationship(s) between different data points. For example, if a retailer wants to understand purchasing patterns of its customers, an unsupervised learning model can be developed to find out which products are most often purchased together or how to group their customers by purchase history. Is it called “unsupervised” learning because no specific outcome is expected. Unsupervised learning techniques include clustering and association rules.

The increasing power of data mining has caused concerns for many, especially in the area of privacy. In today’s digital world, it is becoming easier than ever to take data from disparate sources and combine them to do new forms of analysis.

In fact, a whole industry has sprung up around this technology: data brokers. These firms combine publicly accessible data with information obtained from the government and other sources to create vast warehouses of data about people and companies that they can then sell.

## CHOOSING A DATABASE PLATFORM

There are hundreds of databases and data-related platforms on the market, and equally  many ways to narrow down the scope of choices.

Often times, the first question you will likely need to answer is, **_“Do I want to use a relational database?”_** And if so, **_what are the features I think I need in a relational database versus what I can have with a NoSQL database?_** Relational databases or relational database management systems (RDBMS) represent the bigger chunk of the operational database market.

## CONCLUSION

Through out this Database Administration we have gone various concepts about Databases especially how:

- Data is made up of facts of the world.

- A database is an organized collection of related data. Relational databases are the most widely used type of database, where data is structured into tables and all tables must be related to each other through unique identifiers. It is used to define a central system in which data can be stored and queried. In a simplistic sense, the file system on which files are stored is a kind of database; but when we use the term in a professional data context, we usually mean a dedicated system for managing data records rather than files.

- Databases serve an important function for many individuals and companies, by providing effective and practical ways to organize and store information using or on a computer. Business Analysts, QAs, Database Administrators and developers among other *'technical actors'* use database languages to design, maintain and monitor databases and their related management systems.

- A  relational database is a type of database that organizes data into  structured tables, also known as relations. These tables consist of rows  (records) and columns (fields).

- For a relational database to work properly, it is important that only one person be able to manipulate a piece of data at a time, a concept known as record- locking. But with today’s large-scale databases (think Google and Amazon), this is just not possible. A NoSQL database can work with data in a looser way, allowing for a more unstructured environment, communicating changes to the data over time to all the servers that are part of the database.

- A database management system (DBMS) is a software application that is used to create and manage databases, and can take the form of a personal DBMS, used by one person, or an enterprise DBMS that can be used by multiple users.

- DBMS packages generally provide an interface to view and change the design of the database, create queries, and develop reports. Most of these packages are designed to work with a specific type of database, but generally are compatible with a wide range of databases.

- Some fundamental RDBMS concepts every DBA should know are table, row, column, primary key, foreign key, join, index, view and that all the RDBMS like ***MySQL, Informix, Oracle, MS Access*** and **Microsoft SQL Server** use SQL as their standard database language which also allows users to query databases in a number of ways, using English-like statements.

- Relationships between tables play a key role in defining how data is connected. The main types of relationships are One-to-One Relationship, One-to-Many Relationship, and Many-to-Many Relationship.

- When it comes to choosing a database the biggest decision is picking a relational (SQL) or non-relational (NoSQL) data structure. SQL databases are primarily called Relational Databases (RDBMS); whereas NoSQL databases are primarily called non-relational or distributed databases.

- A data warehouse is a special form of database that takes data from other databases in an enterprise and organizes it for analysis.

- Data mining is the process of looking for patterns and relationships in large data sets. Many businesses use databases, data warehouses, and data-mining techniques in order to produce business intelligence and gain a competitive advantage.

- An **Insertion Anomaly**, is where redundant data is inserted into a table for every new row, e.g ***saving two different but related pieces of data in the same table(Data Repetition).***

- SQL is a language used by database administrators among other database users to work with a relational database, from simple requests for data to a complex update operations, and most applications that work with databases use of SQL as a way to analyze and manipulate relational data. It can also be embedded in many computer languages that are used to develop platform-independent web-based applications and supports fundamental operations for data manipulation,  data definition, and data control.

- SQL is used in various applications such as web development, data analysis, and backend systems. It is used extensively in business applications for analysing customer data, managing inventory, and even tracking sales among other things.

- Data analysis and reporting tools leverage the power of SQL to extract insights, perform calculations, and generate reports from large datasets for business intelligence and timely decision making and action.

- Most traditional Web applications and content management systems that are are not NoSQL based utilize SQl to store and retrieve data for user accounts, articles, and other web content.

- Joins  act as bridges, connecting different tables based on their  relationship. They are extremely useful when you need to retrieve data  from multiple tables. The 3 main types of joins are Inner Join, Right Outer Join, Left Outer Join

- Perhaps the most interesting new development is the concept of NoSQL (from the phrase “not only SQL”). NoSQL arose from the need to solve the problem of large-scale databases spread over several servers or even across the world.

- The SQL query execution order refers to ***the order in which the SQL clauses*** or ***how the query clauses*** are evaluated by the requirements or how to optimize database search results. AND this order is ***𝗙𝗥𝗢𝗠, 𝗪𝗛𝗘𝗥𝗘, 𝗚𝗥𝗢𝗨𝗣 𝗕𝗬, 𝗛𝗔𝗩𝗜𝗡𝗚, 𝗦𝗘𝗟𝗘𝗖𝗧, 𝗢𝗥𝗗𝗘𝗥 𝗕𝗬, 𝗟𝗜𝗠𝗜𝗧***.

- Query optimization is a common task performed by database administrators and application designers to tune a database system's performance. Therefore to achieve better performance we need to use best, faster and efficient queries and one of the best way to tune query performance is to write queries in a number of different ways and compare their reads and execution plans.

- SQL indexes are vital tools in database management even though indexing can be a double-edged sword. For one it can significantly speeds up queries, but can also takes up storage space and adds overhead to operations, yet balancing performance & optimal storage is crucial to get the most out of your database without introducing inefficiencies.

- Indexing can Enhance Data Retrieval but needs to be used cautiously meaning, to get the most out of your database, you should use the right index type for the job. Forexample, When you are indexing a table, make sure to carefully select the columns to be indexed based on the most frequently used columns in WHERE clauses.

- Data warehousing is the process of building data warehouses which are designed to store massive ammounts of historical data useful for performing large-scale analysis on complex data sets.

- Dimensional form is a data modelling approach that comprise of facts, tables at the center along with a set of dimensional tables as its look up tables.

## SQL CHEATSHEET

### Data Types

- Numeric: ***INTEGER/INT, SMALLINT, DECIMAL(a,b)***.
- String: ***CHAR, CHAR(n), VARCHAR(n)***.
- Bit String: ***BIT, BIT(n)***.
- Date and Time: ***DATE, TIME, TIME(t)***.
- TIMESTAMP: ***TIMESTAMP***.

- **ARITHMETIC OPERATORS** Add (+), Subtract(-), Multiply(*), Divide(/)

### SQL Essentials

- SQL ``ALIAS`` ---- AS.
- SQL ``GROUP BY`` ---- GROUP BY COLUMN, HAVING.
- SQL ``ORDER BY`` ---- ORDER BY (ASC/DESC).
- SQL ``JOINS`` ---- INNER, LEFT, RIGHT, FULL JOINS.
- SQL ``FUNCTIONS`` ---- AVG(), SUM(), COUNT(), MIN(), MAX().
- SQL ``WHERE`` ---- LIKE, IN, BETWEEN, ANY, EXISTS, AND,OR,NOT.

### Query

- **CREATE** used to create a new database or table.

```sql
CREATE DATABASE <DATABASE_NAME>
CREATE TABLE <TABLE_NAME>
```

- **DROP** used to delete an exsisting database or table.

```sql
DROP DATABASE <DATABASE_NAME>
DROP TABLE <TABLE_NAME>
```

- **TRUNCATE** used to delete information in the table but doesn't delete the table itself.

```sql
TRUNCATE TABLE <TABLE_NAME>
```

- **ALTER** used to delete, add or modify constraints or columns in a table.

```sql
ALTER TABLE <TABLE_NAME>
ADD <COLUMN NAME> <DATA_TYPE>

ALTER TABLE <TABLE_NAME>
DROP COLUMN <COLUMN_NAME>

ALTER TABLE <TABLE_NAME>
ALTER COLUMN <COLUMN_NAME> <DATA_TYPE>
```

- **BACKUP** used to create a backup on an exsisting database.

```sql
BACKUP DATABASE <DATABASE_NAME>
TO DISK = '<PATH>'
```

- **INSERT** used to insert new tuples (rows) in a table.

```sql
INSERT INTO <TABLE_NAME> (COLUMN1,...COLUMNn)
VALUES (VALUE1,...VALUEn)
```

- **DELETE** used to delete tuples(rows) from a table.

```sql
DELETE FROM <TABLE_NAME>
WHERE <CONDITION>
```

- **UPDATE** used to modify exsisting records in a table.

```sql
UPDATE <TABLE_NAME>
SET <COLUMN_NAME> = <NEW_VALUE>
WHERE <CONDITION>
```

- **SELECT** used to select data from a table

```sql
SELECT <ATTRIBUTE LIST>
FROM <TABLE_NAME>
WHERE <CONDITION>
```

- **UNION, INTERSECT, EXCEPT** is equivalent to the set operations; union, intersection and difference.

```sql
<FIRST SELECT STATEMENT>
UNION / INTERSECT / EXCEPT
<SECOND SELECT STATEMENT>
```

- **IN** compares a value with a set of values, returns true if the value is one of the elements of the set.

```sql
SELECT <ATTRIBUTE LIST>
FROM <TABLE_NAME>
WHERE <VALUE> IN <ANOTHER SELECT QUERY>
```

- **NULL** used to check whether a value is null.

```sql
<ATTRIBUTE NAME> IS (NOT) NULL
```

- **JOIN** used to join two tables based on a related column between them.

```sql
SELECT <ATTRIBUTE LIST>
FROM <TABLE A> JOIN <TABLE B>
ON <JOIN CONDITION>
WHERE <SELECTION CONDITION>
```

- **ASSERTION** used to ensure a certain condition is always met in the database.

```sql
CREATE ASSERTION <ASSERTION_NAME>
CHECK (<CONDITION>)
```

- **TRIGGERS** are activated when a defined action is executed for the table.

```sql
CREATE TRIGGER <TRIGGER_NAME>
BEFORE / AFTER
INSERT / UPDATE / DELETE
ON <TABLE_NAME>
FOR EACH ROW
<TRIGGER BODY>
```

- **REFERENTIAL TRIGGERED ACTION** is used to set what happend on updating or deleting a tuple(row) in the database that references another row

```sql
ON DELETE <OPTION>
ON UPDATE <OPTION>
```

**OPTIONS**:

- *SET NULL*
- *SET DEFAULT*
- *CASCADE*

- **RENAMING (ALIASING)**- Relations and attributes can be renamed for conenience or to remove ambiguity using the keyword ``AS``.

```sql
<TABLE_NAME> AS <NEW_TABLE_NAME>
(<NEW_ATTRIBUTE 1 NAME>,....)
```

- **CROSS PRODUCT** (,) used to produce a result table that has the number of rows of the first table multiplied by the number of rows of the second table.

```sql
SELECT <ATTRIBUTE LIST>
FROM <TABLE 1>, <TABLE 2>
```

- **DUPLICATES** - *DISTINCT* used to eliminate duplicates & *ALL* used to allow duplicates.

```sql
SELECT ALL <ATTRIBUTE LIST>
FROM <TABLE_NAME>

SELECT DISTINCT <ATTRIBUTE LIST>
FROM <TABLE_NAME>
```

- **STRING COMPARISION** using ``LIKE`` where (%) replaces an arbitrary number of characters and (_) replaces on character.

```sql
<ATTRIBUTE> LIKE <PATTERN>
```

- **ORDERING**
  - *ORDER BY* is used to order the resulting tuples.
  - The Keyword ``ASC``(Ascending) and ``DESC`` can be used.

```sql
<SELECT STATEMENT>
ORDER BY <ATTRIBUTE> <ASC / DESC>
```

- **SET COMPARISIONS**
  - ``ANY`` and ``ALL`` can be used with (=, >, >=, <, <=, <>) to compare a value with a set.
  - ``CONTAINS`` compares two sets and returns true if one set contains the other.
  - ``EXISTS`` checks whether the result of a nested query is empty or not.
  - ``UNIQUE`` checks if the table has duplicates.

```sql
SELECT <ATTRIBUTE LIST>
FROM <TABLE NAME>
WHERE <VALUE> > ALL / ANY <ANOTHER SELECT QUERY>
```

- **AGGREGATE FUNCTIONS**
  - ``COUNT`` function counts how many rows in a particular column.
  - ``SUM`` function adds together all the values in a particular column.
  - ``MIN`` funtion returns the minimum value in a column.
  - ``MAX`` function returns the maximum value in a column.
  - ``AVG`` function returns the average of a group of selected values.
  
## SQL INTERVIEW QUESTIONS

### Basic SQL Questions

- What is database?
- What is SQL?
- What is the Difference between SQL vs NoSQL?
- Primary, Unique, composite, foreign keys
- What is a Foreign Key?
- What is a Primary Key?
- What are the different types of Keys?
- What are the different types of operators?
- What is the Difference Between 'CHAR' And 'VARCHAR'?
- What is the difference between VARCHAR and NVARCHAR?

### Intermediate SQL Questions

- What are contraints and their types.
- What are the different types of constraints?
- What is a JOIN? Explain The Different Types Of Joins.
- What is the Difference Between ``WHERE`` and ``HAVING`` clauses?
- Explain the use of ``GROUP BY`` and ``ORDER BY`` clauses.
- Difference between ``GROUP BY`` and ``WHERE``?
- what is the difference between ``DML``, ``DDL`` and ``DCL``?
- What Are the Diferent Types of SQL Statements?
- What are views?
- What is a Subquery?
- What is faster between CTE and Subquery?
- What are Indexes and Indexing?
- Explain the order of execution of SQL.

### Advanced SQL Questions

- what are triggers in SQL?
- What are Stored Procedures?
- What are B+ Trees, B Trees & How they work?
- What is Normalisation and denormalisation? Explain the different Normal Forms.
- What is a Trigger?
- What is Database Hashing?
- Explain the concept of ACID properties.
- What is a Transaction? Explain the Different states of a Transaction.
- Explain all the types of windows functions? (Mainly rank, row_num, dense_rank, lead & lag)
- What are aggregate function and when do we use them?

## FREQUENTLY ASKED QUESTIONS (FAQ)

- **What is SQL?**
SQL stands for Structured Query Language, a programming language used for managing and manipulating relational databases.

- **What's the difference between SQL and MySQL**
SQL is a language used for interacting with relational databases, and MySQL is a specific implementation of a relational database management system that uses SQL. MySQL is just one example of an RDBMS that supports SQL.

- **What is a database?**
A database is an organized collection of data stored and accessed electronically. It provides a way tostore, organize, and retrieve large amounts of data efficiently.

- **What is a Relational Database?**
A relational database is a type of database that organises data into one or more tables, with each table consisting of a set of rows and columns. The tables are related to one another through the use of a key, allowing for easy data retrieval and manipulation.

- **What is the purpose of a primary key in a relational database?**
A Primary key is a unique identifier for each row in a table. It is used to enforce the integrity of the data by ensuring that each row has a unique value, and it is also used to establish relationships with other tables through foreign keys.

- **What is normalisation in a relational database?**
Normalisation is the process of organising data in a database into seperate tables based on their logical relationships. The goals of normalisation is to minimise data redundancy and improve data integrity by ensuring that each piece of data is stored in only one place.

- **What is a join in a relational database?**
A join is a query that cobines rows from two or more tables based on a related column between them. There are several types of joins, including inner join, left join, and right join.

- **What is ACID in a relational database?**
ACID is an acronym that stands for Atomicity, Consistency, Isolation, Durability. These are the four properties that ensure that database transactions are processed reliably. 
  - **Atomicity** _guarantees that a transaction is treated as a single, indivisible operation_.
  - **Consistency** _ensures that a transaction brings the database from one valid state to another_.
  - **Isolation** _ensures that concurrent transactions do not interfere with one another_.
  - **Durability** _guarantees that once a transaction has been committed, it will survive permanently_.

- **How do you handle concurrency in a relational database?**
Concurrency can be handled through the use of locking mechanisms, such as pessimistic locking and optimistic locking.
  - **Pessimistic locking** involves preventing other users from accessing a piece of data while it is being updated, while **Optimistic locking** involves allowing multiple users to access the data at the same time and then handling conflicts that may arise when the data is being updated.
Additionally, using a transaction isolation level can also help to control concurrency issues.

- **What is an index in a relational database?**
An Index is a data structure that helps to quickly locate and retrieve specific rows in a table. It is typically created on one or more columns and can be used to improve the performance of queries.

- **What is a view in a relational database?**
A view is a virtual table that is based on the result of a SELECT statement. It does not store data itself, but rather provides a way to access data from one or more tables in a specific way.

- **What is the difference between a database and a schema?**
A **database** is a container that holds multiple objects,such as tables, views, indexes, and procedures, representing a logical grouping of related data whereas a **schema**, on the other hand, is a container within a database that holds objects and defines their ownership, providing a way to organize and manage database objects.

- **What is the difference between a temporary table and a table variable?**
A **temporary table** is a table that is created and existsonly for the duration of a session or a transaction and can be explicitly dropped or is automatically dropped when the session or transaction ends whereas a **table variable** is a variable that can store a table-like structure in memory. It has a limited scope within a batch, stored procedure, or function and is automatically deallocated when the scope ends.

- **What is the difference between the CHAR and VARCHAR data types?**
CHAR stores fixed-length character strings, while VARCHAR stores variable-length character strings. The storage size of CHAR is constant, while VARCHAR adjusts dynamically.

- **What is ACID in the context of database transactions?**
ACID stands for **Atomicity**, **Consistency**, **Isolation**,and **Durability**. It is a set of properties that guarantee reliable processing of database transactions.

  - **Atomicity** ensures that a transaction is treated as a single unit of work, either all or none of the changes are applied.
  - **Consistency** ensures that a transaction bringsthe database from one valid state to another._
  - **Isolation** ensures that concurrent transactionsdo not interfere with each other._
  - **Durability** ensures that once a transaction is committed, its changes are permanent and survive system failures.

- **What is a primary key?**
A primary key is a column or combination of columns that uniquely identifies each row in a table. It enforces the entity integrity rule in a relational database.

- **What is a foreign key?**
A foreign key is a column or combination of columnsthat establishes a link between data in two tables. It ensures referential integrity by enforcing relationships between tables.

- **What is the difference between a primary keyand a unique key?**
A primary key is used to uniquely identify a row in atable and must have a unique value. On the otherhand, a unique key ensures that a column or combination of columns has a unique value but does not necessarily identify the row.

- **What is the difference between a primary keyand a candidate key?**
A primary key is a chosen candidate key that uniquely identifies a row in a table whereas a candidate key is a set of one or more columns that could potentially become the primary key.

- **What is an ALIAS command?**
ALIAS command in SQL is the name that can be givento any table or a column. This alias name can bereferred in WHERE clause to identify a particulartable or a column.

- **What is normalization?**
_Normalization is the process of organizing data in adatabase to minimize redundancy and dependency.It involves breaking down a table into smaller tables and establishing relationships between them.

- **What are the different types of normalization?**
The different types of normalization are:

- First Normal Form (1NF).
- Second Normal Form (2NF).
- Third Normal Form (3NF).
- Boyce-Codd Normal Form (BCNF).
- Fourth Normal Form (4NF).
- Fifth Normal Form (5NF) or Project-Join Normal Form (PJNF).

- **What is a transaction in SQL?**
A transaction is a sequence of SQL statements that are executed as a single logical unit of work. It ensures data consistency and integrity by either committing all changes or rolling them back if an error occurs.

- **Why are SQL functions used?**
SQL functions are used;-
  - To perform some calculations on the data.
  - To modify individual data items.
  - To manipulate the output.
  - To format dates and numbers.
  - To convert the data types.

- **What is the purpose of the COALESCE function?**
The COALESCE function returns the first non-null expression from a list of expressions. It is often used to handle null values effectively.

- **What is the purpose of the ROW_NUMBER() function?**
_The `ROW_NUMBER()` function assigns a unique incremental number to each row in the result set. It is commonly used for pagination or ranking purposes.

- **What is a join in SQL?**
A join is an operation used to combine rows from twoor more tables based on related columns. It allows you to retrieve data from multiple tables simultaneously.

- **What is a self-join?**
A self-join is a join operation where a table is joined with itself. It is useful when you want to compare rows within the same table based on related columns. It requires bined result set.

- **What is the difference between UNION and UNION ALL?**
**UNION** and **UNION ALL** are used to combine the result sets of two or more SELECT statements. **UNION** removes duplicate rows from the combined result set whereas **UNION ALL** includes all rows, including duplicates.

- **What is the difference between a cross join and an inner join?**
A **cross join (Cartesian product)** returns the combination of all rows from two or more tables whereas an **inner join** returns only the matching rows base don a join condition.

- **What is the difference between the UNION and JOIN operators?**
UNION combines the result sets of two or moreSELECT statements vertically, while JOIN combinescolumns from two or more tables horizontally basedon a join condition.

 **What is the difference between a natural join and an inner join?**
A natural join is an inner join that matches rows based on columns with the same name in the joined tables. It is automatically determined by the database.

- **What is the difference between the HAVING clause and the WHERE clause?**
The **WHERE** clause operates on individual rows and is used to filter rows based on a condition before the data is grouped or aggregated whereas The **HAVING** clause, on the other hand, is used to filter grouped rows based on a condition after the data is grouped or aggregated using the **GROUP BY** clause.

 **What is the purpose of the GROUP BY clause?**
The **GROUP BY** clause is used to group rows based on one or more columns in a table. It is typically used in conjunction with aggregate functions, such `asSUM`, `AVG`, `COUNT`, etc., to perform calculations on grouped data.

- **What is the difference between DELETE and TRUNCATE in SQL?**
The **DELETE** statement is used to remove specific rows from a table based on a condition. It can be rolled back and generates individual delete operations for each row while **TRUNCATE** statement, on the other hand, is used to remove all rows from a table. It cannot be rolled back, and it is faster than **DELETE** as it deallocates the data pages instead of logging individual row deletions.

- **What is the purpose of the CASCADE DELETE constraint?**
The CASCADE DELETE constraint is used toautomatically delete related rows in child tableswhen a row in the parent table is deleted.

- **What is the difference between a clusteredand a non-clustered index?**
A clustered index determines the physical order of data in a table. It changes the way the data is stored on disk and can be created on only one column. A table can have only one clustered index.

A non-clustered index on the other hand does not affect the physical order of data in a table. It is stored separately and contains a pointer to the actual data. A table can have multiple non-clustered indexes.

- **What is a deadlock?**
A deadlock occurs when two or more transaction sare waiting for each other to release resources,resulting in a circular dependency. As a result, none of the transactions can proceed, and the system may become unresponsive.

- **What is a stored procedure?**
A **stored procedure** is a set of SQL statements that are stored in the database and can be executed repeatedly. It provides code reusability and better performance.

- **What is a subquery?**
A subquery is a query nested inside another query. It is used to retrieve data based on the result of an inner query.

- **What is a view?**
A view is a virtual table based on the result of an SQL statement. It allows users to retrieve and manipulate data as if.

- **What is the purpose of the COMMIT statement?**
The COMMIT statement is used to save changes made in a transaction permanently. It ends the transaction and makes the changes visible to other users.

- **What is the purpose of the ROLLBACK statement?**
The ROLLBACK statement is used to undo changes made in a transaction. It reverts the database to its previous state before the transaction started.

- **What is the purpose of the NULL value in SQL?**
NULL represents the absence of a value or unknown value. It is different from zero or an empty string and requires special handling in SQL queries.

- **What is the difference between a view and a materialized view?**
A materialized view is a physical copy of the view's result set stored in the database, which is updated periodically. It improves query performance at thecost of data freshness.

- **What is a correlated subquery?**
A correlated subquery is a subquery that refers to a column from the outer query. It executes once for each row processed by the outer query.

- **What is the purpose of the DISTINCT keyword?**
The DISTINCT keyword is used to retrieve unique values from a column or combination of columns in a SELECT statement.

- **What is the difference between the IN and EXISTS operators?**
The IN operator checks for a value within a set of values or the result of a subquery. The EXISTS operator checks for the existence of rows returned by a subquery.

- **What is the purpose of the TRIGGER statement?**
The TRIGGER statement is used to associate a set of SQL statements with a specific event in the database. It is executed automatically when the event occurs.

- **What is the difference between a unique constraint and a unique index?**
A unique constraint ensures the uniqueness of values in one or more columns, while a unique index enforces the uniqueness and also improves query performance.

- **What is the purpose of the TOP or LIMIT clause?**
The TOP (in SQL Server) or LIMIT (in MySQL) clause isused to limit the number of rows returned by a query. It is often used with an ORDER BY clause.

- **What is a data warehouse?**
A data warehouse is a large, centralized repository that stores and manages data from various sources. It is designed for efficient reporting, analysis, and business intelligence purposes.

- **What is the purpose of the GRANT statement?**
The GRANT statement is used to grant specific permissions or privileges to users or roles in a database.

- **What is a correlated update?**
A correlated update is an update statement that refers to a column from the same table in a subquery. It updates values based on the result of the subquery for each row.

- **What is the purpose of the CASE statement?**
The CASE statement is used to perform conditional logic in SQL queries. It allows you to return different values based on specified conditions.

- **What is the difference between the EXISTS and NOT EXISTS operators?**
The EXISTS operator returns true if a subquery returns any rows, while the NOT EXISTS operator returns true if a subquery returns no rows.

- **What is the purpose of the CROSS APPLY operator?**
The CROSS APPLY operator is used to invoke a table-valued function for each row of a table expression. It returns the combined result set.

## GLOSSARY

- **Sublanguages:** A sublanguage is a subset of a language. Sublanguages occur in natural language, computer programming language, and relational databases.
- **IBM System R:** is a database system built as a research project at IBM's San Jose Research Laboratory beginning in 1974. [System R](https://en.wikipedia.org/wiki/IBM_System_R) was a seminal project: it was the first implementation of SQL, which has since become the standard relational data query language.
- **Edgar F. Codd (19 August 1923 – 18 April 2003):** was an English computer scientist who, while working for IBM, invented the relational model for database management, the theoretical basis for relational databases and relational database management systems. He made other valuable contributions to computer science, but the relational model, a very influential general theory of data management, remains his most mentioned, analyzed and celebrated achievement.
- **Raymond F. Boyce (1946–1974):** was an American computer scientist who was known for his research in relational databases. He is best known for his work co-developing the SQL database language and [Boyce-Codd normal form](https://en.wikipedia.org/wiki/Boyce%E2%80%93Codd_normal_form).
- **Donald D. Chamberlin:** is an American computer scientist who is one of the principal designers of the original SQL language specification with Raymond Boyce. He also made significant contributions to the development of [XQuery](https://en.wikipedia.org/wiki/XQuery). Chamberlin was elected a member of the [National Academy of Engineering](https://www.nae.edu/) in 1997 for contributions to the SQL database query language.
- **SQUARE (Specifying Queries in A Relational Environment):**, *but it was difficult to use due to subscript/superscript notation.-- SQUARE is a set-oriented data sublanguage for expressing queries to a database consisting of a collection of time-varying relations that mimics how people use relations or tables to obtain information.*
- **XQuery (XML Query):** is a query and functional programming language that queries and transforms collections of structured and unstructured data, usually in the form of XML, text and with vendor-specific extensions for other data formats (JSON, binary, etc.).

## RESOURCES AND REFERENCES

- [Early History Of SQL](https://github.com/piusmwilson/business-information-technology-library/blob/main/resources/Early_History_of_SQL.pdf)
- [A Relational Model Of Data For Large Shared Data Banks](https://github.com/piusmwilson/business-information-technology-library/blob/main/resources/A%20Relational%20Model%20of%20Data%20for%20Large%20Shared%20Data%20Banks-codd.pdf)
- [SQUARE (Specifying Queries in A Relational Environment)](https://github.com/piusmwilson/business-information-technology-library/blob/main/resources/SQUARE%20(Specifying%20Queries%20in%20A%20Relational%20Environment).pdf)
- [SQL Roadmap](https://roadmap.sh/sql)
- [History of SQL](https://medium.com/@yidigeng95_64319/history-of-sql-bc92a4981d60)
- [We Learn SQL](https://www.youtube.com/playlist?list=PLVaK3MTZWeZCW__qXkqlV0FesBi9lCPiF)
- [A Relational Model of Data for Large Shared Data Banks](https://github.com/piusnmuhumuza/bootcamp/blob/master/Database%20Adminstration/docs/A%20Relational%20Model%20of%20Data%20for%20Large%20Shared%20Data%20Banks-codd.pdf)
- [Understanding Database Character Sets and Collations”](https://blog.fourninecloud.com/database-character-set-charset-collation-and-their-relationship-explained-227bd5155c48)
- [Data Normalization: Definition, Importance, and Advantages](https://coresignal.com/blog/data-normalization/)
- [SQL Querying for Beginners Tutorial](https://www.youtube.com/watch?v=AFY3z4FwRg0&t=1568s&ab_channel=LearnitTraining)
- [MySQL Tutorial for Beginners [Full Course]](https://www.youtube.com/watch?v=7S_tz1z_5bA&ab_channel=ProgrammingwithMosh)
- [10 Best Practices to Write Readable and Maintainable SQL Code](https://towardsdatascience.com/10-best-practices-to-write-readable-and-maintainable-sql-code-427f6bb98208)
- [Introduction to XQuery](https://www.ibm.com/docs/en/db2/11.5?topic=data-introduction-xquery)
- [XQuery Language Reference (SQL Server)](https://learn.microsoft.com/en-us/sql/xquery/xquery-language-reference-sql-server?view=sql-server-ver16)
- [McJones et al. “The 1995 SQL Reunion: People, Projects and Politics”](http://www.scs.stanford.edu/~dbg/readings/SRC-1997-018.pdf)
- [XML Query Language](https://www.techopedia.com/definition/2671/xml-query-language-xquery)
- [Structured Query Language (SQL)](https://www.techtarget.com/searchdatamanagement/definition/SQL)
- [SQL | DDL, DQL, DML, DCL and TCL Commands](https://www.geeksforgeeks.org/sql-ddl-dql-dml-dcl-tcl-commands/)
- [Types of SQL Commands: DDL, DQL, DML, DCL, TCL](https://trainings.internshala.com/blog/different-types-of-sql-commands/)
- [Types of Database Languages and Their Uses](https://sahil-miglani.medium.com/types-of-database-languages-and-their-uses-1a4b84b89e72)
- [SQL vs. NoSQL: The Most Important Differences](https://blog.udemy.com/nosql-vs-sql/?utm_source=adwords&utm_medium=udemyads&utm_campaign=DSA_Catchall_la.EN_cc.ROW&utm_content=deal4584&utm_term=_._ag_88010211481_._ad_535397282064_._kw__._de_c_._dm__._pl__._ti_dsa-393987629421_._li_9076814_._pd__._&matchtype=&gclid=CjwKCAiAxreqBhAxEiwAfGfndIYj8JDvQdOheiaOnsJIcefnvmkjzBjc2waeVjVad-tMmKJjrYXWhxoCNJkQAvD_BwE)
- [SQL vs. NoSQL Databases: What’s the Difference?](https://www.ibm.com/blog/sql-vs-nosql/)
- [Relational Databases Explained](https://architecturenotes.co/things-you-should-know-about-databases/)
- [Database Sharding Explained](https://architecturenotes.co/database-sharding-explained/)
- [What is a relational database?](https://www.ibm.com/topics/relational-databases)
- [Paakasa](https://github.com/piusnmuhumuza/paakasa) / [dumpFile](https://github.com/piusnmuhumuza/bootcamp/blob/master/Database%20Adminstration/db-backups/DumpPaakasa.sql)
- [12 Intermediate Database Administrator and Developer Interview Questions on Indexing](https://javarevisited.blogspot.com/2022/12/12-database-sql-index-interview.html)
- [Database Indexing Explained](https://x.com/levelupcoding_/status/1802571855875965034?s=46)
- [Extract, transform, and load(ETL)](https://learn.microsoft.com/en-us/azure/architecture/data-guide/relational-data/etl)
- [A Complete Guide on Building an ETL Pipeline for Beginners](https://www.analyticsvidhya.com/blog/2022/06/a-complete-guide-on-building-an-etl-pipeline-for-beginners/)
- [SQL CTEs: Usage, Advantages, and Drawbacks](https://www.stratascratch.com/blog/sql-ctes-usage-advantages-and-drawbacks/)
- [CTE in SQL](https://docs.getdbt.com/terms/cte)
- [How To Learn SQL?](https://newsletter.techworld-with-milan.com/p/how-to-learn-sql)
- [SQL Beginner to Advanced in One Hour](https://www.youtube.com/watch?v=oreAsJTNcsA) by [Career Foundry](https://careerfoundry.com/) & [Alex Freberg](https://www.linkedin.com/in/alex-freberg/).
- [Static Hashing in DBMS](https://byjus.com/gate/static-hashing-in-dbms-notes/)
- [Dynamic Hashing in DBMS](https://byjus.com/gate/dynamic-hashing-in-dbms-notes/)
- [What Is Hashing, and How Does It Work?](https://www.codecademy.com/resources/blog/what-is-hashing/)
- [DBMS - Hashing](https://www.tutorialspoint.com/dbms/dbms_hashing.htm)
- [What Goes Around Comes Around](https://github.com/piusmwilson/business-information-technology-library/blob/main/resources/What%20goes%20around-SH05.pdf) by Michael Stonebraker & Joseph M. Hellerstein.
- [What Goes Around Comes Around... And Around...](https://github.com/piusmwilson/business-information-technology-library/blob/main/resources/whatgoesaround-sigmodrecord2024.pdf) by Michael Stonebraker & Andrew Pavlo.
- [Query Optimization Techniques - Tips For Writing Efficient And Faster SQL Queries](https://github.com/piusmwilson/business-information-technology-library/blob/main/resources/sql_query_optimization_techniques-Jean_Habimana.pdf) by Jean HABIMANA.
- [10 Ways to Improve SQL Query Performance](http://www.developer.com/db/10-ways-to-improve-sql-query-performance.html)
- [15 Ways to Optimize Your SQL Queries](http://hungred.com/useful-information/ways-optimize-sql-queries/)
- [Optimize SQL Server queries with these advanced tuning techniques](http://www.techrepublic.com/blog/the-enterprise-cloud/optimize-sql-server-queries-with-these-advanced-tuning-techniques/)
- [Making Queries Run Faster](https://sqlschool.modeanalytics.com/advanced/faster-queries.html)
- [Query Optimization Techniques in Microsoft SQL Server](http://www.dbjournal.ro/archive/16/16_4.pdf)
- [SQL Tuning or SQL Optimization](http://beginner-sql-tutorial.com/sqlquery-tuning.htm)
- [SQL Server Optimization Tips](http://santhoshgudise.weebly.com/uploads/8/5/4/7/8547208/sql_server_optimization_tips-1.doc)
- [Efficient SQL Statements](https://oracle-base.com/articles/misc/efficient-sql-statements)
- [Best Way to Write SQL Query](http://www.ifadey.com/2010/11/best-way-to-write-sql-query/)
- [SQL Tuning Guidelines for Oracle - Simple yet Effective!](http://askanantha.blogspot.com/2007/10/sql-tuning-guidelines-for-oracle-simple.html)
- [What are the most common SQL Optimizations](http://stackoverflow.com/questions/1332778/what-are-your-most-commonsql-optimizations)
- [Top 10 performance tuning tips for relational databases](http://web.synametrics.com/top10performancetips.htm)
- [Database Systems Research](https://enhancedformysql.github.io/tech-explorer-hub/reading/database/index.html)

## KEYWORDS

``Data``,  ``Data Management``, ``Information``, ``Information``, ``Databases``, ``System R``, ``SQUARE``, ``QUEL``, ``SEQUEL``, ``Structured English QUEry Language``, ``SQL``, ``NoSQL``, ``SQLite``, ``Structured Query Language``, ``Database Administration``, ``Database Administrator``, ``Relational Databases``, ``Query``, ``Querying``, ``SQL Querying``, ``Normalization``, ``De- Normalization``,``Normal Form``, ``Database Character Sets``, ``SQL Server``, ``XQuery``, ``PostgreSQL``, ``MySQL``,``DBMS``, ``RDBMS``, ``Indexes``, ``Indexing``, ``ETL``, ``ELT``, ``Pipelines``, ``Data Pipelines``, ``Data Lakes``, ``Data Warehouses``, ``Data Warehousing``, ``CTE``, ``Common Table Expressions``, ``No-SQL``,  ``Database Querying``, ``Database Systems``, ``Database Character Sets``, ``SQL Commands``, ``Transactions``, ``DDL``, ``DML``,``DCL``, ``TCL``, ``DQL``, ``SQL Statement``, ``MongoDB``, ``Database Security``, ``Database Design``, ``Database Architecture``, ``Data Architect``, ``Database Developer``, ``Query Optimization``, ``Relation Types``, ``One-to-One Relationship``, ``One-to-Many Relationship``, ``Many-to-Many Relationship``, ``Joins``, ``Database Joins``, ``SQL Process``, ``SQL query execution order``, ``Query Tuning``, ``Query Optimization``, ``optimization Engine``, ``Query engine``, ``Query Dispatcher``, ``Query Optimizer``, ``Query Performance``, ``Query Execution Plan``, ``SQL Automation``, ``CAP Theorem``
