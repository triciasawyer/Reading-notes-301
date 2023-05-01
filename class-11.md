# Reading notes for class 11

## nosql vs sql

**Fill in the chart below with five differences between SQL and NoSQL databases:**

*SQL:*
-Data uses schemas
-Relations
-Data is distributed across multiple tables
-Horizontal scaling is difficult/impossible, vertical scaling is possible
-limitations for lots of (thousands) read and write queries per second

*NoSQL:*
-Schema-less
-No (or very few) relations
-Data is typically merged/nested in a few collections
-Both horizontal and vertical scaling is possible
-Great performance for mass (simple) read and write requests

**What kind of data is a good fit for an SQL database? Give a real world example.**
SQL databases are perfectly suited for storing and processing structured data. Platforms, such as Snapchat and Instagram, make use of SQL to store the profile information of users. The Structured Query Language allows them to update the database of their app when users create new posts or share photos, and it also facilitates the recording of messages, enabling users to retrieve messages later.

**What kind of data is a good fit a NoSQL database? Give a real world example.**
NoSQL databases are better suited for cloud, mobile, social media and big data requirements. They are designed for specific use cases and are easier to use than general-purpose relational or SQL databases for those types of applications. PayPal uses NoSQL which processes real-time big data using multiple techniques. It also apprehends large volumes of raw clickstream data using various models using NoSQL databases.

**Which type of database is best for hierarchical data storage?**
NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.

**Which type of database is best for scalability?**
SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.

## sql vs nosql (Video)

**What does SQL stand for?**
Structured Query Language.

**What is a relational database?**
A type of database that stores and provides access to data points that are related to one another. Relational databases are based on the relational model, an intuitive, straightforward way of representing data in tables.

**What type of structure does a relational database work with?**
SQL databases are primarily called as Relational Databases (RDBMS).

**What is a ‘schema’?**
A schema is a list of logical structures of data. A database user owns the schema, which has the same name as the database manager.

**What is a NoSQL database?**
NoSQL, also referred to as “not only SQL”, “non-SQL”, is an approach to database design that enables the storage and querying of data outside the traditional structures found in relational databases.

**How does it work?**
NoSQL databases store data in documents rather than relational tables. Accordingly, we classify them as "not only SQL" and subdivide them by a variety of flexible data models. Types of NoSQL databases include pure document databases, key-value stores, wide-column databases, and graph databases.

**What is inside of a MongoDB database?**
MongoDB stores data records as documents (specifically BSON documents) which are gathered together in collections. A database stores one or more collections of documents.

**Which is more flexible - SQL or MongoDB? and why.**
Schema restrictions also limit the dynamic classification and storage of hierarchical data. With MongoDB, you don't have such constraints, which makes MongoDB more flexible than SQL Server. Whether your data is formatted or it's completely unstructured, you can easily store it in a non-tabular format.

**What is the disadvantage of a NoSQL database?**
One of the most frequently cited drawbacks of NoSQL databases is that they don't support ACID (atomicity, consistency, isolation, durability) transactions across multiple documents. With appropriate schema design, single-record atomicity is acceptable for lots of applications.

## Things I want to know more about

Databases and all that you can do with them.
