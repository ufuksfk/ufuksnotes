---
draft: true
description:
socialDescription:
title: What’s the Difference Between MySQL and PostgreSQL
tags: []
date: 2025-03-05
modified: 2025-08-21
---
author: [[Amazon Web Services, Inc.]]
url: https://aws.amazon.com/compare/the-difference-between-mysql-vs-postgresql/

last highlighted date: [[2025-01#28]]

## Highlights
- Both use structured query language (SQL) as an interface to read and edit data
- Both are open source and have strong developer community support
- Both have a built-in data backup, replication, and access control features
- MySQL offers ACID compliance only when you use it with InnoDB and NDB Cluster storage engines or software modules. PostgreSQL is fully ACID compliant in all configurations.
- MVCC varies by Storage Engine in MySQL. For example, MVCC is fully supported when you use the InnoDB storage engine. MVCC is not supported in the MyISAM storage engine. PostgreSQL supports MVCC in all configurations.
- Databases use indexes to retrieve data faster. You can index frequently accessed data by configuring the database management system to sort and store it differently from the other data.
- MySQL supports B-tree and R-tree indexing that stores hierarchically indexed data. PostgreSQL index types include trees, expression indexes, partial indexes, and hash indexes. There are more options to fine-tune your database performance requirements as you scale.
- Working with PostgreSQL is more intuitive for database developers. PostgreSQL also supports other additional data types like arrays and XML.
- While both MySQL and PostgreSQL support stored procedures, PostgreSQL allows you to call stored procedures written in languages other than SQL
- A trigger is a stored procedure that runs automatically when a related event occurs in the database management system.
- In a MySQL database, you can only use *AFTER* and *BEFORE* triggers for SQL *INSERT*, *UPDATE*, and *DELETE* statements. That means the procedure will run automatically before or after the user modifies the data. In contrast, PostgreSQL supports the *INSTEAD OF* trigger, so you can run complex SQL statements using functions.
- PostgreSQL is better suited for enterprise-level applications with frequent write operations and complex queries.
- PostgreSQL, on the other hand, can be much more challenging for newcomers. It typically requires complex infrastructure setup and troubleshooting experience.
- If your application requires frequent data updates, PostgreSQL is a better choice. However, if you require frequent data reads, MySQL is preferred.
- MySQL uses write locks to achieve real concurrency. For example, if one user is editing the table, another user may have to wait until the operation finishes before changing the table.
- However, PostgreSQL has built-in multiversion concurrency control (MVCC) support without read-write locks. This way, PostgreSQL databases perform better in the case of frequent and concurrent write operations.
