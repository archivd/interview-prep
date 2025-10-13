# HLD Topics

- [Striver's System Design Roadmap](https://takeuforward.org/system-design/complete-system-design-roadmap-with-videos-for-sdes)

- [Piyush Garg - System Design Playlist](https://youtube.com/playlist?list=PLinedj3B30sBlBWRox2V2tg9QJ2zr4M3o&si=jqGBQBLOOl6UX4hs)

- [Gaurav Sen - Resources](https://interviewready.io/resources)

----

### Topics

----

<details>
  <summary>Scalability and Load Balancing</summary>
</details>

----

<details>
  <summary>Caching strategies</summary>
</details>

----

<details>
  <summary>Consistent Hashing</summary>

  - [Piyush Garg - Consistent Hashing](https://youtu.be/IC5Y1EE-aj4?si=lXaGJb2yiY-T0uk6)
</details>

----

<details>
  <summary>Database Sharding and Partitioning</summary>
</details>

----

<details>
  <summary>Event-Driven Architecture - Kafka/SQS</summary>
</details>

----

<details>
  <summary>API Gateway and Rate Limiting</summary>

  - [Piyush Garg - Rate Limiting](https://youtu.be/CVItTb_jdkE?si=NMyDp9sgaqxbj8NL)
</details>

----

<details>
  <summary>Consistency and Consensus (ACID Properties, CAP Theorem, Raft)</summary>
</details>

----

<details>
  <summary>Distributed Caching and CDN</summary>
</details>

----

<details>
  <summary>Micro-services vs. Monolith vs. Serverless</summary>
</details>

----

<details>
  <summary>Database selection - SQL vs. NoSQL</summary>
</details>

----

<details>
  <summary>System Observability/Alerting</summary>
</details>

----

## Important HLD questions

----

<details>
  <summary>Q1. What is a Load Balancer. Explain in detail.</summary>

----
A load balancer is an essential architectural component in modern system design interviews, playing a key role in distributing client requests across multiple backend servers for scalability, reliability, and high availability[1][5][6].

### Core Functionality and Components

A load balancer acts as a “traffic cop” sitting between clients and backend servers, routing incoming traffic to available and healthy servers[6][7]. Its core components typically include:

- **Health Checks/Monitors:** Regularly assess which backend servers are healthy and ready to take requests, removing unhealthy instances from rotation[1][2][7].
- **Endpoint Pools:** Groups or pools of servers (endpoints) that the load balancer distributes traffic to, selected based on geographic or functional considerations[2][7].
- **Steering Algorithms:** Defines how traffic is distributed, using algorithms such as round robin, least connections, hash-based, or weighted distribution[6][16].

### Benefits and Interview-Relevant Points

- **Scalability:** Enables horizontal scaling; new servers can be added seamlessly as demand increases[1][8].
- **High Availability:** If a server fails, the load balancer routes requests to other healthy servers, ensuring the application remains available[1][6].
- **Performance:** Efficient distribution prevents server overload and bottlenecks, reducing latency and improving response times[1][6].
- **Session Persistence:** Maintains stateful connections for clients if required (sticky sessions)[1][5].
- **Maintenance Flexibility:** Allows zero-downtime updates by rerouting traffic away from servers undergoing maintenance[6].

### Types and Algorithms

- **Layer 4 (Transport Level) Load Balancers:** Route traffic based on TCP/UDP protocol data.
- **Layer 7 (Application Level) Load Balancers:** Understand HTTP/HTTPS requests; allow smarter routing, SSL termination, URL-based routing, etc.[7][5].
- **Common Algorithms:**
  - *Round Robin:* Evenly distributes traffic sequentially.
  - *Least Connections:* Directs traffic to the server with fewest active connections.
  - *IP Hashing/Consistent Hashing:* Ensures requests from the same user go to the same backend (useful for session persistence)[6][5].

### System Design Interview Approach

- **When to Use:** Whenever a solution needs to support high traffic, high reliability, or scaling beyond a single instance[6].
- **Where to Place:** Describe clearly in your architecture where the load balancer sits (usually front-end, but sometimes between specific tiers or microservices)[6][8][13].
- **Cloud Load Balancer Examples:** Mention built-in solutions like AWS Elastic Load Balancer, GCP Cloud Load Balancing, or Azure Load Balancer[7][9].
- **Stateful vs Stateless:** Know how to handle session persistence and sticky sessions[5].

### Best Practices and Pitfalls

- Monitor server health and configure failover strategies[2][7].
- Avoid single points of failure: sometimes, use multiple load balancers with DNS-based routing[5][6].
- Support SSL/TLS termination and central certificate management for better security[5].
- Account for latency, caching, and connection rebalancing[6].

A solid interview answer will provide practical examples, note trade-offs, and include the load balancer’s position in the system’s architectural diagram, emphasizing improved reliability and scalability[6][8].

Sources  
[1] What is Load Balancer & How Load Balancing works? https://www.geeksforgeeks.org/system-design/what-is-load-balancer-system-design/  
[2] Load Balancing Reference Architecture https://developers.cloudflare.com/reference-architecture/architectures/load-balancing/  
[3] Azure Load Balancer components https://learn.microsoft.com/en-us/azure/load-balancer/components  
[4] What Is a Load Balancer? https://www.f5.com/glossary/load-balancer  
[5] Introduction to Load Balancing https://www.designgurus.io/course-play/grokking-system-design-fundamentals/doc/introduction-to-load-balancing  
[6] Step-By-Step Approach for Load Balancing in System ... https://www.designgurus.io/answers/detail/step-by-step-approach-for-load-balancing  
[7] What is an Application Load Balancer? https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html  
[8] System Design Interview: Load Balancers https://www.tryexponent.com/blog/load-balancers-system-design-interview  
[9] Cloud Load Balancing overview https://cloud.google.com/load-balancing/docs/load-balancing-overview  
[10] Load Balancer - System Design Interview Question https://www.geeksforgeeks.org/system-design/load-balancer-system-design-interview-question/  
[13] Load Balancers and Microservices Architecture https://www.alibabacloud.com/tech-news/a/load_balancer/4oc53uwjeyk-load-balancers-and-microservices-architecture  
[16] Load Balancing Algorithm Explained - AWS - Updated 2025 https://aws.amazon.com/what-is/load-balancing/  
</details>

----

<details>
  <summary>Q2. What is Database Sharding & Replication. Explain in detail.</summary>

----
**Database sharding** and **replication** are complementary techniques used to handle scalability, performance, and availability challenges in distributed systems[1][4].

### Database Sharding

Sharding involves splitting a large dataset into smaller, more manageable parts called “shards,” each stored in separate database instances. Conceptually, it’s *horizontal partitioning* where each shard contains a subset of rows rather than specific columns[2][4].

- **Goal:** Scale writes and reads by distributing data across servers.
- **Shard Key:** A column or composite key used to decide in which shard a given record resides (e.g., `user_id`)[3].
- **Shard Types:**
  - *Range-based:* Data divided by value ranges (e.g., user IDs 1–10K on shard A, 10K–20K on shard B).
  - *Hash-based:* Data distributed by hashing a key to evenly spread load.
  - *Geographic-based:* Data localized by region for low latency.
- **Challenges:**
  - Rebalancing and resharding complexity.
  - Cross-shard joins and transactions.
  - Hotspot issues if shard key distribution is uneven[5].

### Database Replication

Replication involves duplicating data across multiple nodes to increase fault tolerance and read scalability, often keeping one node as the **primary** and others as **replicas**[2][4].

- **Types of Replication:**
  - *Synchronous:* Writes confirmed only after all replicas update (strong consistency, higher latency).
  - *Asynchronous:* Primary updates replicas later (eventual consistency, better latency)[2].
- **Benefits:**
  - High availability and disaster recovery.
  - Improved read performance by serving reads from replicas.
- **Challenges:**
  - Conflict resolution in multi-master setups.
  - Lag between replicas (replication delay).

### Combined Use Case

Modern architectures often **combine both**:
- Sharding → for horizontal scalability.
- Replication → for fault tolerance and read scalability.

### Example (Typical System Design Explanation in Interviews)

Imagine an e-commerce platform:
- Sharding is applied on the `user_id` field across region-based shards.
- Each shard has one primary and two replicas.
- Writes go to primaries, reads distributed to replicas.
- Failover mechanisms promote replicas upon primary failure.

### Best Practices

- Always define a shard key early based on access patterns.
- Automate rebalancing using consistent hashing.
- Use middleware or proxy layers (e.g., Vitess, Citus, or custom routing service).
- Monitor replication lag using metrics (e.g., AWS RDS ReplicaLag metric).

Sources  
[1] Database Sharding Explained https://www.geeksforgeeks.org/system-design-database-sharding/  
[2] Replication in Database Systems https://learn.microsoft.com/en-us/azure/architecture/best-practices/replication  
[3] Shard Key Design - MongoDB Guide https://www.mongodb.com/docs/manual/sharding/  
[4] Database Scaling Patterns https://designgurus.io/course-play/grokking-system-design-scalability/doc/database-scaling  
[5] Horizontal Scaling and Sharding https://aws.amazon.com/nosql/sharding/  
</details>

----

<details>
  <summary>Q3. What are Caching Strategies (Redis, CDN). Explain in detail.</summary>

----
Caching strategies aim to reduce database or origin-server load and improve system response times by storing frequently used data in fast-access layers like **Redis** or **CDNs**[1][5][6].

### In-Memory Caching (Redis)

**Redis** is an in-memory key-value data store often used for low-latency caching in backend systems[2].

#### Common Caching Patterns

- **Cache-aside (Lazy Loading):**
  - Application checks cache first. If data is missing, fetch from the database and populate cache.
  - *Advantage:* Avoids stale data; avoids unnecessary cache fills.
  - *Drawback:* Cache miss latency on first access.

- **Write-through:**
  - Data is written to cache and database simultaneously.
  - *Advantage:* Consistent cache and DB state.
  - *Drawback:* Write latency increases slightly.

- **Write-back (Write-behind):**
  - Writes go to cache first; DB updated asynchronously.
  - *Advantage:* Low write latency.
  - *Drawback:* Risk of data loss if cache fails before DB sync.

- **Time-to-Live (TTL):**
  - Sets expiration for cache entries to manage freshness and avoid stale reads.

### Distributed Cache Considerations

- Use consistent hashing to distribute keys across Redis cluster.
- Handle cache invalidations carefully (e.g., using Pub/Sub or version tags).
- Redis can store objects, serialized JSONs, or computed results.

### CDN (Content Delivery Network) Caching

For static assets (images, JS, video), **CDNs** cache data geographically closer to users, reducing network latency.

- **How it Works:**
  - CDN nodes (PoPs) serve cached responses.
  - On cache miss, fetches content from origin.
- **Cache-Control headers:** Govern browser and edge cache policies (e.g., `max-age`, `no-cache`).
- **Invalidation:** Manually purge or auto-expire outdated assets upon deployment.

### Interview Perspective

- Emphasize caching layers → browser → CDN → application → Redis.
- Discuss cache consistency trade-offs.
- Mention eviction policies (LRU, LFU, FIFO).
- Handle cache stampede via locking or request collapsing.

### Example Short Answer (In System Design):
“In our architecture, user session tokens and frequently accessed profile data could be cached in Redis for low-latency retrieval, while static content like profile pictures would be cached on a CDN to reduce bandwidth and improve load times.”

Sources  
[1] System Design: Caching Strategies https://www.geeksforgeeks.org/system-design-caching-strategies/  
[2] Redis Caching Fundamentals https://redis.io/docs/latest/develop/use/  
[3] CDN Architecture Overview https://aws.amazon.com/what-is/cdn/  
[4] Cache Invalidation Strategies https://designgurus.io/course-play/grokking-system-design-fundamentals/doc/caching  
[5] Cache-aside vs Write-through https://learn.microsoft.com/en-us/azure/architecture/best-practices/caching  
[6] How CDNs Work https://www.cloudflare.com/learning/cdn/what-is-a-cdn/  
</details>

----

<details>
  <summary>Q4. What is a Rate Limiter (Token & Leaky Bucket). Explain in detail.</summary>

----
A **rate limiter** is a mechanism that controls the number of requests a client can make to a server within a specified time window. It prevents abuse, protects backend resources, and ensures fair usage among clients[1][2].

### Core Purpose

- Avoid API overuse or denial of service.
- Maintain system stability by limiting requests per second or minute.
- Enforce quotas and fairness in multitenant architectures.

### Common Algorithms

#### Token Bucket Algorithm
- A bucket holds a fixed number of tokens; each request consumes one.
- Tokens refill at a constant rate.
- **If the bucket is empty**, incoming requests are denied or queued until refilled.
- **Pros:**
  - Allows short bursts (up to bucket size).
  - Smooths traffic over time.
- **Used in:** APIs (AWS API Gateway, Nginx), networking (traffic shaping).

#### Leaky Bucket Algorithm
- Works as a FIFO queue with constant outflow rate.
- Requests fill the bucket but are processed at a steady rate.
- **If full, new requests are dropped** (prevent overflow).
- **Pros:**
  - Enforces constant output rate.
  - Useful for rate smoothing.
- **Cons:**
  - Less flexible for bursty traffic.

### Comparison (Interview-Relevant)

| Feature | Token Bucket | Leaky Bucket |
|----------|--------------|--------------|
| Burst Handling | Allows bursts up to bucket size | Discards if burst exceeds fixed rate |
| Use Case | API rate control | Network shaping / throttling |
| Implementation | Tokens added periodically | Constant drain rate |
| Example | 5 req/sec capacity with 10-token bucket | 5 req/sec outflow, queue of N size |

### Implementation Components

- **Counter Store:** Redis or memory-based counter (atomic increments).
- **Time Window:** Defines the limit period (fixed, sliding, or rolling windows).
- **Decision Layer:** Middleware that blocks, delays, or forwards requests.

### Best Practices

- Use **distributed locks** or atomic counters for concurrency consistency.
- Add **rate-limit headers** (e.g., `X-RateLimit-Remaining`) in responses.
- Combine with backoff and retry for client-side resilience.

Sources  
[1] Rate Limiting in System Design https://www.geeksforgeeks.org/system-design-rate-limiter/  
[2] Token Bucket Explained https://aws.amazon.com/what-is/token-bucket/  
[3] Designing Rate Limiters https://designgurus.io/course-play/grokking-system-design-fundamentals/doc/rate-limiters  
[4] Leaky vs Token Bucket Algorithms https://cloudflare.com/learning/performance/what-is-rate-limiting/  
</details>

----

<details>
  <summary>Q5. What is CAP Theorem. Explain in detail.</summary>

----
The **CAP Theorem** defines the fundamental trade-offs among **Consistency (C)**, **Availability (A)**, and **Partition Tolerance (P)** in a distributed database system[1][2].

### Core Principle

A distributed system can only guarantee **two of the three** properties simultaneously:

1. **Consistency (C):** Every read receives the most recent write or an error.
2. **Availability (A):** Every request receives a non-error response, even if it may not be the most recent data.
3. **Partition Tolerance (P):** The system continues to function despite message loss or network partition.

### Explanation

- In real-world distributed systems, **network partitions are inevitable**, so systems must trade off between *consistency* and *availability*.
- **CP Systems:** Prioritize data correctness over availability during a partition.
- **AP Systems:** Prioritize responsiveness, allowing eventual convergence.

### Examples

| System Type | Example | Explanation |
|--------------|----------|-------------|
| CP | HBase, MongoDB (majority config) | Read/write blocked during partition to maintain consistency |
| AP | Cassandra, DynamoDB | Responds during partitions with eventual consistency |

### Interview Insights

- CAP does not mean choosing two permanently; trade-offs depend on network state.
- It’s mainly relevant under partition failure scenarios.
- In most practical systems, **eventual consistency** ensures reconciliation post-partition.

Sources  
[1] CAP Theorem Explained https://www.geeksforgeeks.org/system-design-cap-theorem/  
[2] Brewer’s CAP Principle https://www.infoq.com/articles/cap-twelve-years-later-how-the-rules-have-changed/  
[3] Distributed Systems Design Trade-offs https://designgurus.io/course-play/grokking-system-design-scalability/doc/cap-theorem  
</details>

----

<details>
  <summary>Q6. What are Consistency Patterns (Eventual, Strong). Explain in detail.</summary>

----
Consistency patterns define how a distributed system ensures that data seen by clients remains correct and up-to-date across multiple replicas over time[1][2].

### Strong Consistency
- Guarantees that once a write completes, **all subsequent reads return the latest value**.
- System behaves as if only one copy of the data exists.
- **Examples:** RDBMS with synchronous replication, HBase (majority quorum).
- **Advantages:**
  - Predictable results and correctness.
  - Good for financial or transactional systems.
- **Disadvantages:**
  - Higher write latency.
  - Reduced availability under partitions.

### Eventual Consistency
- Ensures that given enough time (and no new updates), **all replicas converge to the same state**.
- Writes propagate asynchronously.
- **Examples:** DynamoDB, Cassandra, S3.
- **Advantages:**
  - High availability and performance.
  - Suited for globally distributed systems.
- **Disadvantages:**
  - Temporary stale reads possible.
  - Conflict resolution complexity.

### Other Intermediate Patterns

- **Causal Consistency:** Ensures operations that are causally related are seen in order.
- **Read-Your-Writes:** A user always sees their own updates immediately.
- **Monotonic Reads:** Once a user reads a value, they won’t see an older value later.

### Interview Context

When designing systems like a social feed or inventory tracker:
- Choose *eventual* for high-scale, less strict apps.
- Choose *strong* for monetary or inventory-critical data.

Sources  
[1] Consistency Models in Distributed Systems https://www.geeksforgeeks.org/distributed-systems-consistency-models/  
[2] Eventual Consistency Explained https://aws.amazon.com/what-is/eventual-consistency/  
[3] Strong vs Eventual Consistency https://designgurus.io/course-play/grokking-system-design-scalability/doc/consistency  
</details>

----

<details>
  <summary>Q7. What is Database Indexing. Explain in detail.</summary>

----
Database indexing improves query performance by maintaining a data structure (usually a **B-tree** or **hash index**) that allows quick lookup of rows based on key values[1][4].

### Concept

- Index = Data structure that maps a **key** to physical row locations.
- Without indexes, a table scan checks every row (O(n)).
- With indexes, lookups become O(log n) or O(1) depending on the index type.

### Common Index Types

- **B-tree Index:** Default in most RDBMS; balanced, supports range queries.
- **Hash Index:** Best for equality comparisons.
- **Bitmap Index:** Used in low-cardinality attributes in analytics.
- **Full-text Index:** For text search capabilities.

### Benefits

- Faster SELECT queries.
- Improved performance for JOIN conditions and WHERE clauses.
- Optimized ORDER BY operations when using clustered indexes.

### Trade-offs

- Slower writes (INSERT/UPDATE/DELETE must update the index).
- Additional storage overhead.
- Not beneficial for small tables or high-write workloads.

### Best Practices

- Index columns that are frequently filtered or used in joins.
- Avoid over-indexing; monitor query execution plans.
- Use **composite indexes** carefully (column order matters).
- For NoSQL (MongoDB, Elasticsearch), define secondary indexes based on query patterns.

Sources  
[1] Database Indexing Explained https://www.geeksforgeeks.org/database-indexing/  
[2] SQL Indexes Guide https://learn.microsoft.com/en-us/sql/relational-databases/indexes/  
[3] Index Optimization Tips https://designgurus.io/course-play/grokking-system-design-fundamentals/doc/indexing  
[4] Database Performance Tuning https://aws.amazon.com/blogs/database/index-optimization/  
</details>

----

<details>
  <summary>Q8. What is Leader Election (Raft & Paxos). Explain in detail.</summary>

----
**Leader election** is a distributed systems technique to ensure that one node acts as a coordinator (leader) at a time, making consistent decisions on behalf of the cluster[1][3].

### Purpose

- Coordinate writes and updates in replicated systems.
- Prevent conflicting updates by designating a single leader.
- Enable health monitoring and failover in distributed systems (e.g., ZooKeeper, Kafka).

### Algorithms

#### Raft Consensus Algorithm
- Easier to understand than Paxos; divides tasks into:
  1. **Leader Election**
  2. **Log Replication**
  3. **Safety**
- Election triggered when followers don’t receive heartbeats from leader.
- **Majority Voting:** A new leader is chosen if it gains votes from the quorum.
- Used in: etcd, Consul, Elasticsearch.

#### Paxos Algorithm
- Older, mathematically complex consensus protocol.
- Nodes act as proposers, acceptors, and learners.
- Ensures consensus on single value or state even under faults.
- Used in: Google Chubby, Spanner (modified versions).

### Interview Context

- Explain leader election in terms of maintaining consistency under failure.
- Mention trade-offs:
  - Raft → simpler, engineering-friendly.
  - Paxos → more general but complex to implement.

### Example

Kafka’s controller node is elected through ZooKeeper; when the leader crashes, a new one takes over using Raft-based coordination.

Sources  
[1] Raft Consensus Paper https://raft.github.io/  
[2] Paxos Made Simple (Lamport, 2001) https://lamport.azurewebsites.net/pubs/paxos-simple.pdf  
[3] Leader Election in Distributed Systems https://www.geeksforgeeks.org/system-design-leader-election/  
[4] Raft vs Paxos https://designgurus.io/course-play/grokking-system-design-scalability/doc/leader-election  
</details>

----

<details>
  <summary>Q9. What are Message Queues (Kafka, RabbitMQ). Explain in detail.</summary>

----
**Message queues** decouple producers and consumers, allowing asynchronous communication in distributed systems[1][2].

### Core Components

- **Producer:** Sends messages to the queue.
- **Broker:** Holds and manages message delivery (Kafka, RabbitMQ).
- **Consumer:** Processes messages asynchronously.
- **Topic/Queue:** Logical channel for message grouping.

### Kafka (Log-based Queue)
- Distributed, partitioned, replicated commit log.
- Messages stored persistently and consumed by offset.
- **Advantages:**
  - High-throughput streaming.
  - Replay and persistence features.
  - Horizontal scalability.
- **Used in:** Event-driven architectures, analytics pipelines.

### RabbitMQ (Traditional Broker)
- Implements *AMQP* protocol.
- Message acknowledgment, routing (exchange → queue → consumer).
- **Advantages:**
  - Flexible routing.
  - Reliable delivery with acknowledgment.
  - Simple queue-based pattern.
- **Used in:** Task queues, transactional async systems.

### Comparison

| Feature | Kafka | RabbitMQ |
|----------|--------|-----------|
| Architecture | Log-based | Broker-based |
| Ordering | Partition-level | Not guaranteed globally |
| Message Retention | Persistent | Until acknowledged |
| Use Case | Stream processing | Reliable async task processing |

### Interview Best Practices

- Identify use cases: event sourcing → Kafka; task queue → RabbitMQ.
- Discuss delivery semantics (at-most-once, at-least-once, exactly-once).
- Mention backpressure handling and dead-letter queues.

Sources  
[1] Kafka Messaging Overview https://kafka.apache.org/documentation/  
[2] RabbitMQ Guide https://www.rabbitmq.com/tutorials/  
[3] Message Queues in System Design https://www.geeksforgeeks.org/system-design-message-queues/  
[4] Kafka vs RabbitMQ https://designgurus.io/course-play/grokking-system-design-fundamentals/doc/message-queues  
</details>

----

<details>
  <summary>Q10. What is Data Partitioning (Hash, Range). Explain in detail.</summary>

----
**Data partitioning** is the process of splitting a dataset across multiple databases or servers to improve scalability, performance, and manageability[1][3].

### Purpose

- Handle datasets larger than a single machine’s capacity.
- Distribute load evenly to prevent hotspots.
- Enable parallel processing and fault isolation.

### Types of Partitioning

#### Hash Partitioning
- Applies a hash function to a key (e.g., `user_id % N`) to assign data to partitions.
- **Advantages:**
  - Even data distribution.
  - Simple to implement.
- **Disadvantages:**
  - Difficult to perform range queries.
  - Rebalancing requires data reshuffling.

#### Range Partitioning
- Assigns records to partitions based on ordered key ranges.
  - Example: IDs 1–1M → shard A, 1M–2M → shard B.
- **Advantages:**
  - Efficient range and sorted queries.
  - Natural ordering.
- **Disadvantages:**
  - Risk of hotspot partitions.
  - Repartitioning complexity.

#### Other Types
- **List Partitioning:** Based on discrete field values (e.g., country = “IN”).
- **Composite Partitioning:** Combines hash + range to balance load and query needs.

### Interview Perspective

- Mention that partitioning is fundamental to horizontal scaling.
- Discuss use with distributed systems like Cassandra, HDFS, or SQL sharding.
- Highlight consistent hashing as a modern approach for dynamic partition management.

Sources  
[1] Data Partitioning Strategies https://www.geeksforgeeks.org/system-design-data-partitioning/  
[2] Range vs Hash Sharding https://aws.amazon.com/blogs/database/data-partitioning-best-practices/  
[3] Consistent Hashing Concepts https://designgurus.io/course-play/grokking-system-design-scalability/doc/partitioning  
[4] Horizontal Scalability Using Partitioning https://learn.microsoft.com/en-us/azure/architecture/best-practices/data-partitioning  
</details>

----

<details>
  <summary>Q11. What is Long Polling, WebSockets, Server-Sent Events. Explain in detail.</summary>

----
These are techniques to achieve real-time communication between clients and servers over the web.

### Long Polling
- Client sends a request to the server and **waits** until the server has new data to send, or a timeout occurs.
- When data is received, the client immediately sends a new request.
- **Use case:** Chat applications, notifications.
- **Advantages:** Works with older browsers; simpler to implement.
- **Disadvantages:** Higher latency, more resource consumption due to repeated requests.

### WebSockets
- Protocol that provides **full-duplex**, persistent connection over a single TCP socket.
- Client and server can **send messages at any time** through the open connection.
- **Use case:** Live streaming, multiplayer gaming, collaborative apps.
- **Advantages:** Low latency, efficient, bi-directional.
- **Disadvantages:** More complex setup; some proxies/firewalls block WebSocket traffic.

### Server-Sent Events (SSE)
- Server pushes updates to the client over a single, **long-lived HTTP connection**.
- Clients receive incoming messages automatically but cannot send data through this connection.
- **Use case:** Live news feeds, stock tickers.
- **Advantages:** Simpler than WebSockets, built on standard HTTP.
- **Disadvantages:** One-way communication; limited browser support.

### Choice Considerations
| Technique | Bi-directional | Browser Compatibility | Use Cases |
|--------------|-------------------|---------------------|-------------------|
| Long Polling | No | Broad | Notifications, chat updates |
| WebSockets | Yes | Modern browsers | Gaming, live feeds |
| SSE | No | Modern browsers | Real-time dashboards |

### Summary
- Use **long polling** where simplicity is key and browser support is limited.
- Use **WebSockets** for interactive, low-latency applications.
- Use **SSE** for unidirectional updates when simplicity and compatibility suffice.

Sources  
[1] Long Polling Tutorial https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events  
[2] WebSocket Protocol https://developer.mozilla.org/en-US/docs/Web/API/WebSocket  
[3] Server-Sent Events (SSE) https://html.spec.whatwg.org/multipage/server-sent-events.html  
[4] Real-time Communication Techniques https://www.geeksforgeeks.org/system-design-real-time-communication-methods/  
</details>

----

<details>
  <summary>Q12. What is Circuit Breaker & Retry Logic. Explain in detail.</summary>

----
**Circuit Breaker** and **Retry Logic** are fault tolerance patterns used to improve system resilience and prevent cascading failures.

### Circuit Breaker
- Prevents repeated execution of failing calls to a downstream service.
- Similar to an electrical circuit breaker; trips when failures exceed threshold.
- States:
  - **Closed:** Normal operation.
  - **Open:** Requests fail immediately without calling the service.
  - **Half-Open:** Test requests allow system to recover gradually.
- **Use case:** Prevent overload of failing services, rapid failure detection.

### Retry Logic
- Automatically retries failed operations (e.g., network call) after a delay.
- Often combined with **exponential backoff** to avoid overwhelming the service.
- **Use case:** Temporary glitches, transient network issues.
- **Trade-offs:** Too many retries can worsen overload; must balance retry count and delay.

### Integrating Both
- When failures detected, circuit breaker trips to avoid further stress.
- After cooling-off period, half-open state tests whether the system is healthy.
- If healthy, resets to closed; if not, remains open.

### Implementation Hints
- Use metrics like failure rate, latency.
- Configure thresholds (failure count/time window).
- Use circuit breaker libraries or middleware (Hystrix, Resilience4j).

### Example Scenario
- A payments API experiencing outages trips the circuit breaker.
- Clients get immediate fallback responses or errors.
- After a cooldown, system attempts recovery with limited requests.

Sources  
[1] Circuit Breaker Pattern https://martinfowler.com/bliki/CircuitBreaker.html  
[2] Retry Pattern https://docs.microsoft.com/en-us/azure/architecture/reliability/retry-or-circuit-breaker  
[3] Fault Tolerance in Distributed Systems https://aws.amazon.com/blogs/architecture/fault-tolerance-patterns-in-microservices/  
[4] Implementing Circuit Breaker https://resilience4j.readme.io/docs/circuitbreaker  
</details>

----

<details>
  <summary>Q13. What is Write-through, Write-back Cache. Explain in detail.</summary>

----
**Write-through** and **Write-back** are caching strategies that define how data is transferred from cache to persistent storage.

### Write-through Cache
- Data is **written to cache** and **simultaneously written to** the backing store (database or persistent storage).
- Ensures data consistency between cache and storage.
- **Advantages:** Always consistent, simple to implement, easy recovery.
- **Disadvantages:** Higher write latency, throughput bottleneck.

### Write-back Cache
- Data is **written to cache only** initially.
- The cached data is **persisted to storage asynchronously** after some time or upon eviction.
- Uses a **dirty bit** to track modified data.
- **Advantages:** Faster writes, reduces load on backend.
- **Disadvantages:** Risk of data loss if cache fails before write-back, complexity in managing consistency.

### Usage Scenarios
| Strategy | Best For | Trade-offs |
|------------|-------------|--------------|
| Write-through | Data correctness, low risk | Slower write performance |
| Write-back | High performance, infrequent writes | Potential data loss |

### Summary
- Use **write-through** for critical data where consistency is paramount.
- Use **write-back** for high-throughput, low-latency caching where occasional data loss is acceptable, or additional recovery mechanisms exist.

Sources  
[1] Cache Write Strategies https://www.geeksforgeeks.org/cache-coherence-in-computer-architecture/  
[2] Write-Through vs Write-Back https://aws.amazon.com/blogs/database/write-back-cache-vs-write-through-cache/  
[3] Caching Techniques https://designgurus.io/course-play/grokking-system-design-fundamentals/doc/cache-strategies  
</details>

----

<details>
  <summary>Q14. What is Horizontal vs Vertical Scaling. Explain in detail.</summary>

----
**Horizontal** and **Vertical Scaling** are two primary approaches to handling increased load in system architecture.

### Vertical Scaling (Scale Up)
- Involves **adding more resources** (CPU, RAM, storage) **to a single machine or server**.
- Simple to implement; just upgrade existing hardware.
- **Advantages:** Easy to set up; no need for distributed system complexity.
- **Disadvantages:** Limited by hardware capacity; bottleneck risk; costly beyond a point.

### Horizontal Scaling (Scale Out)
- Involves **adding more machines or nodes** to distribute load.
- Requires load balancers, distributed databases, and partitioning.
- **Advantages:** Virtually unlimited scalability; fault tolerance.
- **Disadvantages:** More complex in design; network latency and data consistency challenges.

### Use Case Summary
| Approach | Best For | Constraints |
|------------|--------------|--------------|
| Vertical | Small, simple apps, low to moderate load | Hardware limits, cost scalability |
| Horizontal | Large-scale, cloud-native systems | Complexity, consistency, deployment |

### Practical Examples
- Vertical: Upgrading a database server's CPU/RAM.
- Horizontal: Adding more web servers behind a load balancer or sharding a database.

### Final Note
- Modern cloud systems favor **horizontal scaling** due to flexibility and robustness.
- Combining both is common for hybrid architectures.

Sources  
[1] Horizontal vs Vertical Scaling https://aws.amazon.com/answers/architecture/horizontal-vs-vertical-scaling/  
[2] Scaling Techniques in System Design https://www.geeksforgeeks.org/system-design-scaling-techniques/  
[3] Cloud Scalability Strategies https://cloud.google.com/architecture/scale-architecture  
</details>

----

<details>
  <summary>Q15. What is CDN and Geo-Distributed Systems. Explain in detail.</summary>

----
A **Content Delivery Network (CDN)** is a distributed network of servers strategically placed across various geographic locations to deliver content to users with high availability and performance[1][3].

### How CDN Works

- CDN caches static content (images, videos, scripts) on edge servers near the user.
- Requests are routed to the nearest CDN node (PoP – Point of Presence) for faster delivery.
- Reduces latency and offloads traffic from origin servers.
- Supports caching strategies and cache invalidation for content freshness.

### Geo-Distributed Systems

- Systems that are deployed across multiple geographic regions or data centers.
- Aim to improve fault tolerance, reduce latency by serving users from nearby regions.
- Handle data replication, consistency, and network partitioning challenges.
- Often use techniques like **geo-replication**, **regional failover**, and **multi-master replication**.

### Benefits and Challenges

| Aspect | Benefits | Challenges |
|---------|------------|------------|
| CDN | Reduced latency, offload origin, scalability | Cache invalidation, data freshness |
| Geo-Distributed Systems | High availability, disaster recovery | Data consistency, network latency |

### Use Cases

- CDN: Websites, streaming platforms, software downloads.
- Geo-distributed: Global SaaS platforms, financial trading systems.

Sources  
[1] What is a CDN? https://aws.amazon.com/cdn/  
[2] Geo-Distributed Systems Overview https://www.geeksforgeeks.org/system-design-geo-distributed-systems/  
[3] Content Delivery Network Explained https://www.cloudflare.com/learning/cdn/what-is-a-cdn/  
</details>

----

<details>
  <summary>Q16. What is Microservices vs Monolith. Explain in detail.</summary>

----
### Monolithic Architecture
- All components and functionalities reside within a **single codebase** and deploy as one unit.
- Easy to develop initially, simple to test and deploy.
- **Drawbacks:**
  - Scaling requires duplicating entire app.
  - Difficult to maintain, update, or adopt new technologies gradually.
  - Single point of failure impacts entire app.

### Microservices Architecture
- Application decomposed into **small, loosely coupled services** that communicate over APIs.
- Each service is independently deployable, scalable, and developed by separate teams.
- **Advantages:**
  - Technology diversity per service.
  - Easier scaling and fault isolation.
  - Faster development cycles with CI/CD.
- **Drawbacks:**
  - Greater operational complexity.
  - Service discovery, versioning, and network communication overhead.
  - Requires robust monitoring, tracing, and security.

### Interview Viewpoint

| Aspect | Monolith | Microservices |
|-------------|-------------|---------------|
| Deployment | Single package | Multiple independent deployments |
| Scaling | Vertical/horizontal as a whole | Per-service horizontal scaling |
| Fault Isolation | Low | High |
| Team Organization | Single team | Multiple small teams |
| Communication | In-process calls | Network calls (REST/gRPC/message queues) |

### Summary

- Monoliths are suitable for startups/small teams.
- Microservices fit large-scale, rapidly evolving systems with complex domains.

Sources  
[1] Microservices vs Monolith https://martinfowler.com/articles/microservices.html  
[2] System Design Microservices https://www.geeksforgeeks.org/system-design-microservices/  
[3] Advantages and Challenges of Microservices https://aws.amazon.com/microservices/  
</details>

----

<details>
  <summary>Q17. What is API Gateway & BFF Pattern. Explain in detail.</summary>

----
### API Gateway

- Acts as a **single entry point** for client requests in microservices architectures.
- Handles request routing, authentication, rate limiting, load balancing, and protocol translation.
- Aggregates multiple backend services into unified APIs.
- Simplifies client interactions by hiding internal service complexity.

### Backend for Frontend (BFF) Pattern

- A **dedicated backend layer** tailored to the needs of a specific frontend (e.g., mobile app, web app).
- Helps avoid over-fetching/under-fetching by customizing API responses.
- Allows frontend teams to iterate independently on API contracts.
- Can reside behind or as part of the API Gateway.

### Benefits

| Pattern | Advantages |
|----------|-------------|
| API Gateway | Centralized cross-cutting concerns; security; traffic control |
| BFF | Frontend-specific logic; better UX; decoupling frontend/backend |

### Use Cases

- API Gateway: Large microservices systems requiring unified access.
- BFF: Multiple frontend channels needing tailored APIs, such as mobile apps and web portals.

### Interview Focus

- Explain how API Gateway and BFF improve scalability, security, and developer experience.
- Discuss potential drawbacks like API Gateway bottlenecks and maintaining multiple BFFs.

Sources  
[1] API Gateway Overview https://aws.amazon.com/api-gateway/  
[2] Backend for Frontend Pattern https://samnewman.io/patterns/architectural/bff/  
[3] API Gateway and BFF in Microservices https://www.geeksforgeeks.org/api-gateway-backend-for-frontend-bff-pattern/  
</details>

----

<details>
  <summary>Q18. What is Authentication & Authorization (OAuth, JWT). Explain in detail.</summary>

----
### Authentication vs Authorization

- **Authentication:** Verifying user identity (e.g., login with username/password).
- **Authorization:** Determining what resources/actions the authenticated user is allowed to access.

### OAuth (Open Authorization)

- A standard protocol for **delegated authorization**, allowing apps to access user data from other services without sharing credentials.
- Roles:
  - **Resource Owner:** User.
  - **Client:** Application requesting access.
  - **Authorization Server:** Issues access tokens.
  - **Resource Server:** Hosts user data.
- **Flow:** User
