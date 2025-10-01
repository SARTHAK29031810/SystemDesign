# System Design Concepts & Keywords

## Concurrency & Synchronization
- **Mutex (Mutual Exclusion)**: Ensures exclusive access to shared resources.
- **DB Transactions**: Prevents conflicts like simultaneous withdrawals from a bank.
- **File Systems**: Prevents concurrent writes to the same file.
- **OS Kernel**: Manages process scheduling to avoid conflicts.
- **Semaphore**: Controls resource access by multiple threads.
- **Database Connection Pooling**: Reuses database connections to reduce overhead.
- **Traffic Lights**: Manages flow, with a set limit for safety.
- **Producer-Consumer Problem**: Balances the speed between producers and consumers.
- **Monitor**: Combines lock and condition variables for synchronization.
- **Deadlock**: Circular wait causing processes to stall.
- **Livelock**: Processes continuously change states without progress.
- **Starvation**: Low-priority processes are blocked indefinitely.
- **Race Condition**: Concurrent processes create inconsistent states.

## Messaging & Communication Patterns
- **Publish-Subscribe (Pub-Sub)**: One-to-many messaging, e.g., stock market feeds.
- **Message Queue (MQ)**: Temporarily stores messages for sequential processing.
- **Event Bus**: Centralized stream for distributing events to subscribers.
- **Point-to-Point Messaging**: One producer to one consumer communication.
- **Event-Driven Architecture**: Triggers actions based on events.

## Scalability & Load Handling
- **Load Balancer (LB)**: Distributes traffic across servers to prevent overload.
- **Horizontal Scaling**: Involves adding more machines to increase capacity.
- **Vertical Scaling**: Adds resources (CPU, RAM) to a single machine.
- **Rate Limiting**: Controls the rate of client requests to avoid abuse.
- **Backpressure**: Slows producers to match consumer speed.
- **Content Delivery Network (CDN)**: Distributes content closer to users to improve performance.

## Storage & Databases
- **Relational DB (SQL)**: Structured data with ACID transactions (e.g., banking systems).
- **NoSQL DB**: Schema-less, flexible for unstructured data (e.g., social media).
- **Sharding**: Splits large datasets across multiple machines.
- **Replication**: Creates copies of data across servers for reliability.
- **CAP Theorem**: Trade-offs between consistency, availability, and partition tolerance.

## Caching
- **Cache**: Stores frequently accessed data for faster retrieval.
- **Write-through Cache**: Updates both the cache and DB simultaneously.
- **Write-back Cache**: Updates the cache first, then syncs with the DB later.
- **Eviction Policies**: Includes LRU (Least Recently Used), LFU (Least Frequently Used).
- **Cache Invalidation**: Ensures cached data is updated or removed when necessary.

## System Architecture Patterns
- **Monolithic Architecture**: Single, unified application structure.
- **Microservices**: Decomposes applications into smaller, independent services.
- **SOA (Service-Oriented Architecture)**: Larger, service-based systems.
- **CQRS (Command Query Responsibility Segregation)**: Separates read and write operations for better scaling.
- **Event Sourcing**: Stores a sequence of events as the source of truth.

## Reliability & Fault Tolerance
- **Failover**: Backup systems take over in case of failure.
- **Consensus Protocols**: Ensures agreement in distributed systems (e.g., Raft, Paxos).
- **Quorum**: Minimum required votes to ensure consistency.
- **Circuit Breaker**: Prevents repeated failures from cascading.
- **Idempotency**: Ensures that repeated requests do not cause inconsistencies.

## Networking & APIs
- **REST API**: Stateless, resource-oriented API design.
- **GraphQL**: Optimized for querying specific data needs.
- **gRPC**: Efficient, binary protocol for microservices.
- **WebSockets**: Enables real-time, bidirectional communication.
- **API Gateway**: Manages and routes client requests to backend services.
- **Reverse Proxy**: Forwards requests to backend servers.

## Monitoring & Logging
- **Logs**: Tracks system activity, errors, and events.
- **Metrics**: Quantitative measurements of system performance (e.g., latency, throughput).
- **Tracing**: Tracks requests across services for troubleshooting.
- **Health Checks**: Verifies the operational status of services.

## Other Important Concepts
- **Throughput**: Measures system capacity (e.g., requests per second).
- **Latency**: The time delay in processing.
- **Availability**: The system's uptime or readiness to serve requests.
- **Durability**: Guarantees data will not be lost.
- **Bloom Filter**: Probabilistic technique for checking membership of data.
