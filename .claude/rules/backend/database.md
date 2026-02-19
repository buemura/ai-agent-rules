# Rules for Database

## This file describes the database rules for the project.

The project should use a relational database for data storage (PostgreSQL). The database schema should be designed to ensure data integrity, consistency, and scalability. The following rules should be followed when designing the database:

1. Use meaningful and descriptive names for tables, columns, and constraints to improve readability and maintainability.
2. Use standard data types and avoid using custom data types unless necessary.
3. Normalize the database schema to reduce data redundancy and improve data integrity.
4. Use foreign keys to establish relationships between tables and ensure referential integrity.
5. Implement appropriate indexing strategies to optimize query performance.
6. Use transactions to ensure atomicity and consistency of database operations.

Use an Object-Relational Mapping (ORM) tool to interact with the database. The ORM should be used to abstract away the underlying database operations and provide a higher-level interface for working with the data.

Use migrations to manage database schema changes and ensure that the database schema is consistent across different environments.
