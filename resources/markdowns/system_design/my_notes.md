# Some key-concepts

- Auth to AWS Lambda: Expose function URLs, IAM roles with Sigv4-based auth: Infra Level
- EC2: App-level authentications using JWT tokens
- EKS: AWS Load Balancer

- API Gateway:
  - Re-directs requests to the different services in a micro-services architecture
  - Rate-limiting
  - Could become single point of failure - solved using multiple availability zones in a single region
  - Auth (JWT)

- CAP Theorem Basics
In network partitions (inevitable in distributed setups), pick two: Consistency (all nodes see same data), Availability (every request gets a response), or Partition tolerance (system keeps running despite network splits). Real-world: CP (consistent, unavailable during splits, e.g., banking); AP (available, eventually consistent, e.g., social feeds)


Step1:
- Gather requirements: Functional/Non-Functional

Step2:
- API Design/ DB Design

Step3:
- High-Level Design

Step4:
- Deep-dive into Scaling

Step5:
- Bottlenecks and Trade-offs



----


URL Shortening

URL shortner - get unique url
URL redirection
Link Analytics


a-z + A-Z + 0-9 = 62 chars
 _    _    _    _    _    _
62 x 62 x 62 x 62 x 62 x 62 ~= 56Bn+

Non-FR
1. Throughput: 100Mn DAU / Peak Q(Queries)PS - Low: <100 (simple CRUD); Moderate: 1k-10k (mid-scale API); High: 100k+ (Netflix-scale feeds).
2. Availability & Reliability: Uptime 99.99% - 99% (~4hr/mo down); 99.9% (“three nines,” 9hr/yr); 99.99% (multi-AZ, ~1hr/yr); “five nines” (52min/yr, enterprise)
3. Read-heavy: 1Bn/day == 10k/sec.
4. Latency SLAs: Minimize redirect latency - p50/p95/p99: 50%/95%/99th percentile response time.
  Low: p99<50ms (caches); Moderate: <200ms (user-facing); High tolerance: <2s (bg jobs)
5. Consistency: Highly Consistent (RDBMS following ACID)


Schema
- Short URL
  - short_url
  - long_url
  - user_id
  - created_at
  - used_count

1 row ~= 1KB
5Bn rows ~= 5TB
=> 1 RDBMS node is sufficient


