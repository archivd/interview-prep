# SQL Topics

<details>
  <summary><strong>FAQs</strong></summary>

<!-- ################################################### The FAQ list starts here ################################################### -->

<details>
  <summary><strong>1. What are ACID properties in a database?</strong></summary>

  <p>ACID ensures reliable database transactions.</p>

  - **Atomicity**: Transactions are all-or-nothing (rollback on failure).  
  - **Consistency**: Ensures data integrity before and after the transaction.  
  - **Isolation**: Concurrent transactions don’t interfere; controlled by isolation levels.  
  - **Durability**: Once committed, data is permanent even after failures.
</details>

<details>
  <summary><strong>2. What is the CAP theorem?</strong></summary>

  <p>CAP explains trade-offs in distributed databases, stating that only 2 of the 3 guarantees can be provided simultaneously:</p>

  - **Consistency**: Every read receives the most recent data.  
  - **Availability**: Every request receives a response, even if not most recent.  
  - **Partition Tolerance**: System continues working even if communication between nodes fails.

  Example:  
  - MongoDB prioritizes AP.  
  - Traditional RDBMS prioritize CP.
</details>

<details>
  <summary><strong>3. What are SQL constraints?</strong></summary>

  <p>Constraints enforce rules on table data to maintain integrity.</p>

  Common constraints:  
  - **NOT NULL**: prevents null values.  
  - **UNIQUE**: ensures unique values.  
  - **PRIMARY KEY**: unique + not null.  
  - **FOREIGN KEY**: links tables.  
  - **CHECK**: enforces condition (e.g., salary > 0).  
  - **DEFAULT**: sets default value.
</details>

<details>
  <summary><strong>4. Explain different types of keys in SQL?</strong></summary>

  - **Primary Key**: uniquely identifies rows.  
  - **Candidate Key**: any column that can qualify as PK.  
  - **Super Key**: any set of columns that uniquely identify a row.  
  - **Alternate Key**: candidate keys not chosen as PK.  
  - **Foreign Key**: references PK in another table.  
  - **Composite Key**: multiple columns forming unique ID.
</details>

<details>
  <summary><strong>5. What are SQL transactions and transaction isolation levels?</strong></summary>

  <p>A transaction is a unit of work executed as a whole (follows ACID principles).</p>

  **Isolation levels** (to control concurrency anomalies):  
  - **Read Uncommitted**: allows dirty reads.  
  - **Read Committed**: avoids dirty reads, but non-repeatable reads possible.  
  - **Repeatable Read**: prevents non-repeatable reads, but phantom reads possible.  
  - **Serializable**: strictest, prevents all anomalies.
</details>

<details>
  <summary><strong>6. What is the difference between OLAP and OLTP?</strong></summary>

  - **OLTP**: supports day-to-day transactions, normalized schema, fast inserts/updates (e.g., banking apps).  
  - **OLAP**: supports complex querying and analysis, denormalized schema, aggregates (e.g., BI dashboards, data warehouses).
</details>

<details>
  <summary><strong>7. What are Triggers in SQL?</strong></summary>

  <p>Triggers are stored procedures that automatically execute in response to events (INSERT, UPDATE, DELETE).</p>

  Types:  
  - BEFORE Trigger  
  - AFTER Trigger  
  - INSTEAD OF Trigger (on views).

</details>

<details>
  <summary><strong>8. What are Views in SQL?</strong></summary>

  <p>A view is a virtual table created from the result of a query. It does not store data physically but references data from underlying tables.</p>
  <p>Benefits: security, simplification of queries, logical data independence.</p>
</details>

<details>
  <summary><strong>9. Explain Partitioning and Sharding in databases?</strong></summary>

  - **Partitioning**: splitting a large table into smaller parts (horizontal partitions by ranges, vertical partitions by columns).  
  - **Sharding**: distributing partitions across multiple physical machines (used in distributed systems for scalability).
</details>

<details>
  <summary><strong>10. What is Denormalization?</strong></summary>

  <p>Denormalization is the process of introducing redundancy into a database design (opposite of normalization) to improve query performance by reducing joins.</p>
</details>

<details>
  <summary><strong>11. What is difference between clustered vs non-clustered index?</strong></summary>

  - **Clustered Index**: dictates physical order of data in the table, only one per table, faster range queries.  
  - **Non-Clustered Index**: separate structure with pointers to rows, multiple allowed, suitable for searching on non-PK columns.
</details>

<details>
  <summary><strong>12. What is a CTE (Common Table Expression) vs Subquery?</strong></summary>

  - **Subquery**: nested query inside a SQL statement.  
  - **CTE**: a temporary named result set, often used for recursive queries and improving readability.  
  Example: "WITH cte AS ( ... ) SELECT ... FROM cte".
</details>

<details>
  <summary><strong>13. What is the difference between UNION and UNION ALL?</strong></summary>

  - **UNION**: combines results from multiple SELECT queries and removes duplicates.  
  - **UNION ALL**: combines all results including duplicates.  
  Performance-wise UNION ALL is faster since no duplicate check.
</details>

<details>
  <summary><strong>14. What is a Deadlock in SQL?</strong></summary>

  <p>Deadlock occurs when two or more transactions are waiting for each other’s locked resources, resulting in an infinite wait.</p>
  <p>Solutions: deadlock detection by DB engine, query tuning, reducing transaction scope, proper indexing.</p>
</details>

<details>
  <summary><strong>15. What is an Execution Plan in SQL?</strong></summary>

  <p>An execution plan shows how the database will execute a query (order of operations, index usage, join types).</p>

  Tools:  
  - SQL Server Management Studio (SSMS): "Display Estimated Execution Plan"  
  - MySQL/Postgres: `EXPLAIN` keyword.
</details>

<details>
  <summary><strong>16. Explain Window Functions in SQL?</strong></summary>

  <p>Window functions perform calculations across a set of rows related to the current row, without collapsing results (unlike GROUP BY).</p>

  Examples:  
  - ROW_NUMBER(), RANK(), DENSE_RANK()  
  - LEAD(), LAG()  
  - SUM() OVER (PARTITION BY …).
</details>

<details>
  <summary><strong>17. What are Materialized Views?</strong></summary>

  <p>A materialized view physically stores the query result. Unlike normal views, data is stored and can be refreshed on-demand or periodically.</p>
  <p>Useful in OLAP/data warehousing for speeding up aggregation-heavy queries.</p>
</details>

<details>
  <summary><strong>18. What are NoSQL databases and how are they different from SQL databases?</strong></summary>

  - **SQL DBs**: relational, fixed schema, strong ACID compliance.  
  - **NoSQL DBs**: flexible schema, designed for scalability, typically eventual consistency (AP in CAP theorem).  

  <p>Types: key-value stores (Redis), document stores (MongoDB), column stores (Cassandra), graph DBs (Neo4j).</p>
</details>

<details>
  <summary><strong>19. What are Joins vs Self-joins vs Cross-joins?</strong></summary>

  - **Joins**: combine related rows from different tables.  
  - **Self-join**: join of a table to itself (hierarchical data like org chart).  
  - **Cross-join**: Cartesian product (every row with every row).
</details>

<details>
  <summary><strong>20. What is Query Optimization?</strong></summary>

  Query optimization improves performance through:  
  - Indexing properly  
  - Avoiding SELECT *  
  - Using EXISTS instead of IN (in some cases)  
  - Partitioning tables  
  - Reviewing execution plans  

  DB engines use cost-based optimizers to choose best plans.
</details>

<details>
  <summary><strong>21. Transactions in SQL (Beyond ACID basics)</strong></summary>

  <p>A transaction is a logical unit of work composed of one or more SQL statements that succeed or fail as a group.  
  They are controlled by <code>BEGIN</code>, <code>COMMIT</code>, and <code>ROLLBACK</code> statements.</p>
  <p>Internally, databases maintain a transaction log (write-ahead log / WAL) that records all changes before applying them to data files — allowing recovery in case of failure.</p>

  Advanced features:  
  - **Savepoints**: mark intermediate states for partial rollbacks.  
  - **Nested Transactions** (supported in SQL Server but simulated in others via savepoints).  
  - **Autocommit Mode**: in MySQL/Postgres, each statement is automatically committed unless wrapped in an explicit transaction.
</details>

<details>
  <summary><strong>22. Locking Mechanisms in Databases</strong></summary>

  <p>Databases use locks to ensure consistency when multiple users access data concurrently.</p>

  Types of locks:  
  - **Shared Lock (S)**: allows concurrent reads, prevents writes.  
  - **Exclusive Lock (X)**: allows one transaction to modify data, prevents reads/writes by others.  
  - **Update Lock (U)**: used to avoid deadlocks (SQL Server).  
  - **Intent Locks (IS/IX)**: metadata-level locks indicating intention to acquire row/page/table-level locks.  
  - **Row-level** vs **Table-level**: finer granularity prevents contention.  
  - **Optimistic Locking**: check for row version/timestamp before committing, avoids blocking.  
  - **Pessimistic Locking**: acquire lock immediately to block others.

  <p>Deadlock detection: Most RDBMS auto-detect cycles in wait-for graph and abort one transaction to resolve.</p>
</details>

<details>
  <summary><strong>23. Database Isolation Levels (Detailed Mechanisms)</strong></summary>

  <p>Isolation levels define how transactions interact under concurrency, balancing correctness vs performance:  
  </p>

  - **Read Uncommitted**: Highest concurrency, but dirty reads possible.  
  - **Read Committed**: Prevents dirty reads (default in Oracle, SQL Server); achieved via row locks or MVCC snapshots.  
  - **Repeatable Read**: Prevents non-repeatable reads; still allows phantom rows (InnoDB uses gap locks to handle this).  
  - **Serializable**: Full serial execution; prevents all anomalies but reduces concurrency dramatically.

  SQL anomalies:  
  - Dirty Read → reading uncommitted data.  
  - Non-Repeatable Read → same row yields different values in same transaction.  
  - Phantom Read → new rows appear/disappear between queries.  
  - Lost Update → two transactions overwrite each other’s changes.

  Implementation depends on DB:  
  - MVCC (Multi-Version Concurrency Control) in Postgres/MySQL InnoDB.  
  - Lock-based concurrency in SQL Server/Oracle.
</details>

<details>
  <summary><strong>24. Triggers in Databases (Deeper View)</strong></summary>

  <p>A trigger is a special type of stored program that automatically fires in response to events like <code>INSERT</code>, <code>UPDATE</code>, or <code>DELETE</code>.</p>

  Types of triggers:  
  - **Row-level** vs **Statement-level**: applied once for each row vs once per statement.  
  - **BEFORE Trigger**: modify/check data before persistence.  
  - **AFTER Trigger**: used for audit logs, cascaded operations.  
  - **INSTEAD OF Trigger**: common on views, substitute an operation (e.g., break down a view INSERT into multiple base tables).

  <p>Use cases: auditing changes, enforcing complex business rules, maintaining derived columns.  
  Best practice: use carefully, as triggers can introduce hidden logic → making debugging and performance tuning difficult.</p>

  <p>Advanced scenario: Recursive/cascading triggers (trigger firing another trigger) – supported but often limited due to risk of infinite loops.</p>
</details>


<!-- #################################################### The FAQ list ends here #################################################### -->

</details>
