# Elmar

**Backend Engineer · Go / Erlang / Elixir / C**

Commercial backend development in **Go**, concurrent and fault-tolerant services in **Erlang/Elixir**, and low-level, performance-critical components in **C**.

I design distributed backends, develop high-load services, migrate and refactor legacy systems, and optimize latency, throughput, memory usage and database access.

## Technical specialization

| Technology | Work |
| :--- | :--- |
| **Go** | Concurrent services and microservices; goroutines, synchronization, profiling and performance tuning. |
| **Erlang / Elixir** | BEAM-based services, OTP, supervision trees, process messaging, fault tolerance and Phoenix. |
| **C** | Systems programming, low-level components and performance-sensitive code. |
| **PostgreSQL / MySQL** | Schema design, indexing, transactions and query optimization. |

**Service operation:** logging, metrics, tracing, health checks and graceful shutdown.

## Public projects

### [Selfmail](https://github.com/Elmar006/selfmail)

Multi-tenant transactional email backend in Go: PostgreSQL outbox and RLS, RabbitMQ quorum queues with publisher confirms and manual ACK, Redis rate limits, and Postfix delivery. REST, SMTP submission and a Go SDK; AES-256-GCM payload encryption and mTLS. Ambiguous MTA handoffs are recorded as `submission_unknown`.

[Delivery worker](https://github.com/Elmar006/selfmail/blob/main/internal/worker/worker.go) · [Architecture and delivery semantics](https://github.com/Elmar006/selfmail/blob/main/docs/architecture.md)

### [API Gateway / RouteFlow](https://github.com/Elmar006/API-Gateway)

Go reverse proxy with PostgreSQL-backed dynamic routes, a method/path trie, a **16-shard per-IP token-bucket limiter**, and a bounded, non-blocking request-log buffer with batch writes through **`pgx.CopyFrom`**. Separate public and administrative HTTP servers; Tauri/React desktop control plane.

[Rate limiter](https://github.com/Elmar006/API-Gateway/blob/master/backend/internal/infrastructure/limiter/IPLimiter.go) · [Batch persistence](https://github.com/Elmar006/API-Gateway/blob/master/backend/internal/infrastructure/repo/logRepo.go)

### [Энергоконтур / Energokontur](https://github.com/Elmar006/energy_web)

EV charging infrastructure planner. A Python/Pyomo optimization model selects charging sites, equipment, grid upgrades, batteries and solar across multiple investment years. An independent SimPy event simulation models arrivals, queues, power allocation and equipment outages.

[Optimization model](https://github.com/Elmar006/energy_web/blob/main/engine/energy/optimizer.py) · [Event simulation](https://github.com/Elmar006/energy_web/blob/main/engine/energy/simulation.py)

## Product development outside my main work

- **Devora** — AI website generation, background processing, previews and publication. Go, PostgreSQL and Redis.
- **Korger** — automotive-service CRM: scheduling, work orders, inventory, finance, role-based access and SSE updates.
- **NRAV** — coffee ordering: pickup slots, reservations, payments, refunds and staff tools for a website and Telegram Mini App.

These three product repositories are private.

## Stack

**APIs:** REST · gRPC · Protobuf · GraphQL · WebSocket · SSE<br>
**Data & messaging:** PostgreSQL · MySQL · Redis (cache, pub/sub, rate limiting) · RabbitMQ · Kafka (event-driven fundamentals)<br>
**Infrastructure:** Linux · Docker · Docker Compose · Kubernetes · CI/CD with GitHub Actions

## Contact

[Telegram: @viy1ix](https://t.me/viy1ix) · [birembekove@gmail.com](mailto:birembekove@gmail.com)
