# [Database Management System (DBMS)](https://whimsical.com/dbms-roadmap-by-love-babbar-FmUi8ffVop33t3MmpVxPCo)

# Intruduction

---

# What is Data?

- Data is a collection of raw, unorganized facts and details like text, observations, figures, symbols,
and descriptions of things etc.

- In other words, **data does not carry any specific purpose and has no significance by itself.** Moreover, data is measured in terms of bits and bytes – which are basic units of information in the context of computer storage and processing.

# What is Database ?

- Database is an software where data is store in a way that it can be easily accessed,managed,and updated.
- To make real use data, we need **Database Management System**

# What is DBMS ?

- a database-management System is a collection of **interrelated data and a set of programs to access those data.**

- The primary goal of a DBMS is to provide a way to **store and retrieve database information** that is both convenient and efficient.

- A DBMS is the database itself, along with all the software and functionality. It is used to perform different operations, like **addition, access, updating, and deletion of the data.**

#  Why we need DBMS ?

- A Data Base Management System is a system software for **easy, efficient and reliable data processing and management**
-  It can be used for:-

        -  Creation of a database.
        -  Retrieval of information from the database.
        -  Updating the database.
        -  Managing a database.


# [Difference between File System and DBMS](https://www.javatpoint.com/dbms-vs-files-system)

- File System has major **disadvantage**

-  Data Redundancy and inconsistency
-   Difficulty in accessing data
-  data isolation
-  intergrity problems
-  Atomicity problems
-  Concurrent-access anomalies
- security problems

<img width="522" alt="image" src="https://user-images.githubusercontent.com/78966839/226089475-3be0c129-34b3-4478-a727-918898be054c.png">

# what is DBA and it's function ?

- DBA stands for "Database Administrator".

-  A **person who has central control** of both the data and the programs that access tose data.

-  A DBA is a professional responsible for the installation, configuration, maintenance, and security of databases in an organization.


- **function**:-

        i.Schema Definition
        ii. Storage structure and access methods.
        iii. Schema and physical organization modifications.
        iv. Authorization control.
        v. Routine maintenance
                1. Periodic backups.
                2. Security patches.
                3. Any upgrades.


# DBMS Application Architectures :
- client machinesm on which remote DB users work,and server machines on which DB system runs.
- ### a. **T1** Architecture
- i. The client, server & DB all present on the same machine

- ### b. **T2** Architecture
- i. App is partitioned into 2-components.
- ii. Client machine, which invokes DB system functionality at server end through query
language statements.
- iii. API standards like **ODBC & JDBC** are used to interact between client and server.

- ### c. **T3** Architecture
- i. App is partitioned into 3 logical components.
- ii. Client machine is just a frontend and doesn’t contain any direct DB calls.
- iii. Client machine communicates with App server, and App server communicated with DB
system to access data.
- iv. Business logic, what action to take at that condition is in App server itself.
- v. T3 architecture are best for **WWW** Applications.
- vi. **Advantages:**
- 1. **Scalability** due to distributed application servers.
- 2. **Data integrity,** App server acts as a middle layer between client and DB, which
minimize the chances of data corruption.
- 3. **Security,** client can’t directly access DB, hence it is more secure.
CodeHel

<img width="382" alt="image" src="https://user-images.githubusercontent.com/78966839/226222247-9461af15-50e0-466e-a01d-597a76c0b2f1.png">

# Difference Between Two-Tier And Three-Tier database architecture

<img width="437" alt="image" src="https://user-images.githubusercontent.com/78966839/226221787-e7271f83-695d-4357-bc80-ccca28054fb5.png">

# Database Languages:
- a. **Data definition language (DDL)** to specify the database schema.
- b. **Data manipulation language (DML)** to express database queries and updates.
- c. **Practically,** both language features are present in a single DB language, e.g., SQL language.
- d. **DDL**
- i. We specify consistency constraints, which must be checked, every time DB is updated.

- e. **DML**
- i. Data manipulation involves
- 1. **Retrieval** of information stored in DB.
- 2. **Insertion** of new information into DB.
- 3. **Deletion** of information from the DB.
- 4. **Updating** existing information stored in DB.

ii. **Query language**, a part of DML to specify statement requesting the retrieval of


# imp tarm

### instance

- The **collection of information stored in the DB at a particular moment** is called an **instance** of DB.

### Schemas

- The **overall design of the DB** is called the DB schema

- Schema is **structura** description of data. Schema **doesn’t change frequently.** Data may change
frequently.

- DB schema corresponds to the variable declarations (along with type) in a program.
- We have 3 types of Schemas:
- ** Physical, Logical**, several **view schemas** called subschemas.
- Logical schema is most important in terms of its effect on application programs, as programmers construct apps by using logical schema.
- Physical data independence, physical schema change should not affect logical schema/application programs.

# sub-schema 

- A sub-schema in a database management system (DBMS) is a portion of the overall database schema that is **used to describe a specific part of the database.** 
- It represents a subset of the entire database schema and is typically used to organize and manage complex data structures.

- Sub-schemas can be used to create different views of the same data, provide selective access to specific data to different user groups, and improve the overall performance of the system by reducing the complexity of the database schema.

# How is a DBMS implemented?

A database management system handles the requests generated from the SQL interface, producing or modifying data in response to these requests. This involves a multilevel processing system.

# What is Data Abstraction in DBMS

- Hiding internal details to user and showing require thing is call Abstraction.
- Ex:- That is, the system hides certain details of how the data is stored and maintained.

# what are its three levels of Abstraction ?

- 1. Physical Level
- 2. Conceptual Level
- 3. View Level


###  Physical level / Internal level
- i. The lowest level of abstraction describes how the data are stored.

- ii. Low-level data structures used.

- iii. It has **Physical schema** which describes physical storage structure of DB.

- iv. Talks about: Storage allocation (N-ary tree etc), Data compression & encryption etc.

- v. **Goal:** We must define algorithms that allow efficient access to data.

### e. Logical level / Conceptual level:
- i. The conceptual schema describes the design of a database at the conceptual level,describes **what** data are stored in DB, and what **relationships** exist among those data.
- ii. User at logical level does not need to be aware about physical-level structures.

- iii. **DBA,** who must decide what information to keep in the DB use the logical level of abstraction.

- iv. Goal: ease to use.
#### f. View level / External level:
- i. Highest level of abstraction aims to **simplify users’ interaction with the system** by providing different view to different **end-user.**

- ii. Each **view schema** describes the database part that a particular user group is interested and hides the remaining database from that user group.

- iii. At the external level, a database contains several schemas that sometimes called as **subschema.** The subschema is used to describe the different view of the database.

- iv. At views also provide a **security** mechanism to prevent users from accessing certain parts of DB.

<img width="394" alt="image" src="https://user-images.githubusercontent.com/78966839/226228615-40095bce-5fb0-4462-8901-04689f0687d2.png">






# How is Database accessed from Application programs?
- Apps (written in host languages, C/C++, Java) interacts with DB.
- E.g., Banking system’s module generating payrolls access DB by executing DML statements from
the host language.
- API is provided to send DML/DDL statements to DB and retrieve the results.

          - i. Open Database Connectivity (ODBC), Microsoft “C”.
          - ii. Java Database Connectivity (JDBC), Java.


# Referential Integrity

- Referential Integrity Rule in DBMS is based on Primary and Foreign Key.
-  The Rule defines that a foreign key have a matching primary key. Reference from a table to another table should be valid.

---

# RDBMS

# What is  RDBMS  & How it store n memory ?

- An RDBMS is a type of database management system (DBMS) that stores data in a row-based table structure which connects related data elements.
-  An RDBMS includes functions that maintain the security, accuracy, integrity and consistency of the data. This is different than the file storage used in a DBMS.

- It store memory in tabular form.(row and col)

# Degree of relaction 

### 1 : 1 

-  One to one, Entity in A associates with at most one entity in B, where A & B are entity sets. And an entity of B is associated with at most one entity of A.
1. E.g., Citizen has Aadhar Card.

### 1 : M

-  **One to many,** Entity in A associated with N entity in B. While entity in B is associated with at most one entity in A.
- 1. e.g., Citizen has Vehicle

# Many to one,
- Entity in A associated with at most one entity in B. While entity in B can be associated with N entity in A.
- 1. e.g., Course taken by Professor

# Many to many,
- Entity in A associated with N entity in B. While entity in B also associated with N entity in A.
- 1. Customer buys product.
- 2. Student attend course

# [Types of Keys](https://www.geeksforgeeks.org/types-of-keys-in-relational-model-candidate-super-primary-alternate-and-foreign/)

### Primary key :-

-  PRIMARY KEY: This is an attribute or set of attributes that can uniquely identify each entity in the entity set.
-   The  primary key must contain **unique as well as not null** values.

 ### FOREIGN KEY:
 - Whenever there is some relationship between two entities, there must be some common attribute between them. This common attribute must be the primary key of an entity set and will become the foreign key of another entity set.
 -  This key will prevent every action which can result in loss of connection between tables.

 # Candidate Key (CK):
 - minimum subset of super keys, which can uniquely identify each tuple. It contains no redundant attribute.
- 1. CK value shouldn’t be NULL.


 # Alternate Key (AK)
- **All CK except PK.**

- The alternate key is a combination of one or more columns whose values are unique.

### Super Key

- Any permutation and combination of attributes present in a table which can uniquely identify each tuple.

### secondary key

- A key that **uniquely identifies rows but is not selected as the primary key** is known as a secondary key.

# Database Schema

## 1.Physical Database Schema −
- This schema pertains to the actual storage of data and its form of storage like files, indices, etc. It defines how the data will be stored in a secondary storage.

## 2.Logical Database Schema − 

- This schema defines all the logical constraints that need to be applied on the data stored. It defines tables, views, and integrity constraints.

<img width="446" alt="image" src="https://user-images.githubusercontent.com/78966839/227696036-ea1d42ac-7a13-4bf5-9b0e-c5d8011a439a.png">

# [Mapping from ER Model to Relational Model](https://www.geeksforgeeks.org/mapping-from-er-model-to-relational-model/)

- Both ER-Model and Relational Model are abstract logical representation of real world enterprises. Because the two models implies the similar design principles, we can convert ER design into Relational design.

- Converting a DB representation from an ER diagram to a table format is the way we arrive at Relational DB-design from an ER diagram.

---

# Relational Operators (Not comp)

## SELECT
- The SELECT statement is used to select data from a database.

### RENAME:
- rename DB name, table name, column name etc



---
# SQL
---

# What is sql ?





















