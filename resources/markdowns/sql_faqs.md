# SQL Topics

<details>
  <summary><strong>FAQs</strong></summary>

<!-- ################################################### The FAQ list starts here ################################################### -->

<details>
  <summary><strong>1. What are ACID properties in a database?</strong></summary>
  <br>
  <p>
  ACID ensures reliable database transactions.
  </p>
  <p>
  - **Atomicity**: Transactions are all-or-nothing (rollback on failure).  
  - **Consistency**: Ensures data integrity before and after the transaction.  
  - **Isolation**: Concurrent transactions don’t interfere; controlled by isolation levels.  
  - **Durability**: Once committed, data is permanent even after failures.
  </p>
</details>

<details>
  <summary><strong>2. What is the CAP theorem?</strong></summary>
  <br>
  <p>
  CAP explains trade-offs in distributed databases, stating that only 2 of the 3 guarantees can be provided simultaneously:
  </p>
  <p>
  - **Consistency**: Every read receives the most recent data.  
  - **Availability**: Every request receives a response, even if not most recent.  
  - **Partition Tolerance**: System continues working even if communication between nodes fails.
  </p>
  <p>
  Example:  
  - MongoDB prioritizes AP.  
  - Traditional RDBMS prioritize CP.
  </p>
</details>

<details>
  <summary><strong>3. What are SQL constraints?</strong></summary>
  <br>
  <p>
  Constraints enforce rules on table data to maintain integrity.
  </p>
  <p>
  Common constraints:  
  - **NOT NULL**: prevents null values.  
  - **UNIQUE**: ensures unique values.  
  - **PRIMARY KEY**: unique + not null.  
  - **FOREIGN KEY**: links tables.  
  - **CHECK**: enforces condition (e.g., salary > 0).  
  - **DEFAULT**: sets default value.
  </p>
</details>

<details>
  <summary><strong>4. Explain different types of keys in SQL?</strong></summary>
  <br>
  <p>
  - **Primary Key**: uniquely identifies rows.  
  - **Candidate Key**: any column that can qualify as PK.  
  - **Super Key**: any set of columns that uniquely identify a row.  
  - **Alternate Key**: candidate keys not chosen as PK.  
  - **Foreign Key**: references PK in another table.  
  - **Composite Key**: multiple columns forming unique ID.
  </p>
</details>

<details>
  <summary><strong>5. What are SQL transactions and transaction isolation levels?</strong></summary>
  <br>
  <p>
  A transaction is a unit of work executed as a whole (follows ACID principles).
  </p>
  <p>
  **Isolation levels** (to control concurrency anomalies):  
  - **Read Uncommitted**: allows dirty reads.  
  - **Read Committed**: avoids dirty reads, but non-repeatable reads possible.  
  - **Repeatable Read**: prevents non-repeatable reads, but phantom reads possible.  
  - **Serializable**: strictest, prevents all anomalies.
  </p>
</details>

<details>
  <summary><strong>6. What is the difference between OLAP and OLTP?</strong></summary>
  <br>
  <p>
  - **OLTP**: supports day-to-day transactions, normalized schema, fast inserts/updates (e.g., banking

<!-- #################################################### The FAQ list ends here #################################################### -->

</details>
