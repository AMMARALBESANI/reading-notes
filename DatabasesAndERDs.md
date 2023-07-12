# Introduction to Databases and ERDs

## Database Schema

A database schema is a logical representation of data that depicts how the data is organized and the relationships between tables in a database. It also defines the constraints and rules that govern the data, such as data types, primary keys, foreign keys, and more. A database schema can be visually represented using diagrams or expressed textually using code or syntax.

## What is a Schema?

A schema serves as a framework or blueprint of a database, outlining its structure and organization. It doesn't contain actual data but provides information on how the data is stored and interconnected. A schema is used to create, modify, or delete tables, fields, views, indexes, and other database objects.

## Why do we use them?

Database schemas serve various purposes:

-They assist in designing and planning the database prior to its creation.
- They offer a clear and consistent view of the data and its relationships.
- They enforce data integrity and consistency rules.
- They facilitate data access and manipulation through queries and commands.
- They document the structure and organization of the database for future reference and maintenance.


## What do they look like?

Database schemas can vary in appearance depending on the specific database system and the level of abstraction being represented. There are three primary types of database schemas:

1. Physical schema: This schema describes how data is physically stored in storage devices, such as files, blocks, or sectors. It represents the lowest level of abstraction and is typically defined by the database administrator (DBA). The physical schema may differ based on the hardware and software configuration of the system.

2. Logical schema: This schema outlines the logical organization of data, including tables, fields, data types, relationships, constraints, and more. It represents the most common level of abstraction and is usually defined by the database designer or developer. The logical schema can be independent of the physical schema and can be implemented in various ways.

3. View schema: This schema defines how data is presented to end-users or applications. It represents the highest level of abstraction and is typically defined by the database user or analyst. The view schema can be customized to meet different requirements and preferences.

---

## Database Keys

Database keys are attributes or combinations of attributes that serve to uniquely identify a row or record in a table and establish relationships between tables. Various types of keys exist in a database, including primary, natural, surrogate, composite, alternate, unique, and foreign keys.

### What is a Primary Key?

A primary key is one or more columns in a table that uniquely identify each row. It must have a unique value for every row and cannot contain null values. The primary key is also used to establish relationships with other tables through foreign keys.



### What is a Foreign Key?

A foreign key is a column or set of columns in a table that references the primary key of another table. It establishes a relationship between the two tables and enforces referential integrity. A foreign key can contain null values and duplicate values. Its purpose is to maintain data consistency and integrity across related tables.

### What is a Composite Key?

A composite key is formed by combining two or more columns to create a unique identifier for a row in a table. Rather than relying on a single column, a composite key uses a combination of columns to uniquely identify records. This is useful when no single attribute can uniquely identify a row. A composite key can serve as a primary key or a foreign key, depending on its purpose within the table and its relationship with other tables.

### How are they different? When do you use one over the others?

The key differences lie in their functionality and usage:

- Primary keys uniquely identify individual rows within a table and are typically used to establish relationships with other tables through foreign keys.
- Foreign keys establish relationships between tables by referencing the primary key of another table. They ensure data integrity by enforcing referential constraints.
- Composite keys are employed when a single attribute is insufficient to uniquely identify a row. By combining multiple columns, a composite key provides a unique identifier for each record.

The choice of which key to use depends on the specific requirements of the database design. Primary keys are commonly used to uniquely identify rows, while foreign keys are used to establish relationships. Composite keys come into play when no single attribute can uniquely identify a row, requiring a combination of columns to form a unique identifier.


### Relationships in a Relational Database

In a relational database, data is organized into tables consisting of rows and columns. Each table represents a collection of related entities, while each row represents a specific instance of an entity, and each column represents an attribute of that entity.

### What is a Relationship?

A relationship in a relational database refers to the logical connection or association between two or more tables. It enables users to retrieve combined data from different tables through queries, resulting in a unified view of the data. For instance, in a record store database, relationships would allow you to obtain a table displaying album names, song titles, and artist names for each song.

### How is a Relationship Established?

A relationship is established between tables by using a common attribute or column that links them together. This attribute is referred to as a key. There are various types of keys in a relational database, including primary keys, foreign keys, and candidate keys.

The commonly used keys to establish relationships are primary keys and foreign keys. A primary key is a column or set of columns that uniquely identifies each row in a table. It must have unique and non-null values. A foreign key, on the other hand, is a column or set of columns in one table that references the primary key of another table. A foreign key can have null or duplicate values, but it must match an existing value in the referenced table.

### What are the Types of Relationships?

There are three primary types of relationships in a relational database:

1. One-to-One: This relationship exists when a single record in one table is associated with a single record in another table.

2. One-to-Many: This relationship occurs when a single record in one table is associated with multiple records in another table. It is the most common type of relationship in a relational database.

3. Many-to-Many: This relationship exists when multiple records in one table are associated with multiple records in another table. It is implemented using a bridge or junction table that connects the related tables.

### Why are Relationships Important?

Relationships play a crucial role in a relational database for the following reasons:

- Reducing data redundancy: Relationships help avoid storing the same data multiple times, leading to efficient data storage and improved data consistency.

- Ensuring data integrity: Relationships enforce constraints and rules on the data, such as referential integrity, which maintains the consistency and accuracy of data by ensuring that values in foreign keys match the values in the primary keys.

- Facilitating data access: Relationships enable users to perform queries and operations on the data using SQL. With the ability to join, filter, sort, group, aggregate, and manipulate data from different tables, relationships provide efficient and powerful data retrieval and analysis capabilities.
