# Explain what is MongoDB and its features?

- MongoDB is a NoSQL (not only SQL) database that stores large volumes of data in the form of documents. This offers the developers the flexibility to work with evolving data models.

# What are some alternative NOsql databases to MongoDB?

- cassandra
- redis
- amazon DynamoDB.

# How Does MongoDB Store Bata?

- MongoDB stores data records as documents(specifically BSON documents) which are gathered together in collections.

<img width="406" alt="image" src="https://github.com/pattjoshi/interview-Q-A/assets/78966839/8d2be985-1767-48bf-b011-1dbd2385f4cb">

# MongoDB is a Schema-less database. if Yes, How do you create Schema in MongoDB?

- The schema of a database describes the structure of the data to be stored.
- MongoDB facilitates flexibility in schema design thereby organizing the storage of data as key-value pairs into lightweight BSON documents.

# How is MongoDB different from SQL and better than MYSQL?

- MongoDB IS a document-oriented  NO-SQL database used for high-volume data storage.
- MongoDB  is a database that comes into light around the mid-2000s.
- it comes under the category of no-sql database.

- SQL is a programming language used to communicate with and manipulate relational databases like MYSQL.

<img width="306" alt="image" src="https://github.com/pattjoshi/interview-Q-A/assets/78966839/c48a8033-7cbd-46af-ad67-f77ba7d2302f">

# What is MongoDB Replication and Sharding?

- Replication means duplication of the same data across multiple MongoDB servers.

- Data redundancy & High availability
- Multiple copies across servers
- Data Recovery and Backup option

- Sharding is a method of distributing data across multiple databases MongoDB supports deployments with large data sets and high throughput operations via sharding.

<img width="426" alt="image" src="https://github.com/pattjoshi/interview-Q-A/assets/78966839/58a4d7ab-644f-4dc9-8f0e-e2623f3c11e4">

# Explain Horizontal and Vertical Scaling

<img width="887" alt="image" src="https://github.com/pattjoshi/interview-Q-A/assets/78966839/e5259b09-5e9a-4b83-949c-e4975c0b7bc8">

# When should we embed one document with another?

- You should consider embedded documents (subdocuments) for:
  - When the relationship is one-to-few (not many, not unlimited). For unlimited use cases, you should start considering separating subdocuments into another collection.
  - when retrieval is likely to happen together, that will improve performance.
  - when updating transactions, a single document transaction would be more performant.
  - When the field is rarely updated.

# What are Replica sets? Explain primary and secondary Replica sets.

- MongoDB manages to replicate using Replica sets, which are collections of related MongoDB nodes.

- A Replica set requires a minimum of three MongoDB nodes.
- One of the nodes will be considered the primary node that receives all the write operations.
- The others are secondary nodes that will replicate the data from the primary node.
- if Failed Node.js is recovered, works as a secondary node again

# What is the use of Capped collection?

- Capped collections are flexed-size collections that support high-throughput operations the insert, retrieve, and delete documents based on insertion order.

<img width="425" alt="image" src="https://github.com/pattjoshi/interview-Q-A/assets/78966839/0d1c4b99-75ef-4d47-8a4b-01d5d5089164">

# How can you store images, videos, and other large files (> 16 MB)?

- GridFs is a driver specification for uploading and retrieval of MongoDb files large than 16md.

- GridFs divides large files into equal chunks and store them as separate document.

# Explain Aggregation in MongoDB?

- MongoDB aggregation operations act on groups of values from multiple documents, perform operations on the grouped values and return a single
computed result.
- **3-way perform aggregation**
- Aggregation Pipeline
- Map Reduce Operation
- Single Purpose Aggregation

<img width="422" alt="image" src="https://github.com/pattjoshi/interview-Q-A/assets/78966839/66a0c637-cdda-4385-8977-22af491c30b9">

# What is Meant By _id filed in MongoDB?

- _id is the field that uniquely identifies a document in the MongoDB collection.
- if you insert a document that does not contain the _id field, then MongoDB automatically generated the unique id.

# How Does MongoDB Ensure High Availability of Data?

- MongoDB automatically stores copy sets, and multiple copies of data distributed across servers and data centers. Replica sets help to prevent website downtime using native duplication and automatic failures.

- MongoDB has great support for high availability through ReplicaSets.
- However, deploying a ReplicaSet is not enough for a production-ready system. The latter requires a bit of planning.

### 19 complited

[y2b](https://www.youtube.com/watch?v=EKEpVhi-29Q)

























































