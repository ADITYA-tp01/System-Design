# 📐 Distributed Systems & System Design Handbook

> A comprehensive, battle-tested curriculum and deep-dive reference for modern distributed systems, infrastructure architecture, scalability mechanics, and Staff/Principal-level system design interview mastery.

---

## 🧭 Repository Overview

This repository houses an in-depth, production-oriented system design knowledge base structured into **24 core chapters**. Every concept is designed to bridge high-level architectural abstractions with low-level kernel, OS, and hardware realities (page layouts, connection tracking, CPU cache lines, I/O amplification, and consensus protocols).

### Core Highlights
- **Intuition-First Learning:** Clear, high-signal mental models and analogies before diving into complex mechanics.
- **Production Truths:** Practical engineering choices, failure modes, and post-mortems from companies like Netflix, AWS, Uber, Google, and Cloudflare.
- **ASCII Visual Architecture:** Zero-dependency, terminal-friendly ASCII diagrams illustrating packet flows, memory layouts, and topological funnels.
- **AI/ML Infrastructure Included:** Modern workloads integrated into every topic (LLM serving, KV-cache routing, GPU Direct Storage, vector indexes).
- **Standardized Framework:** Predictable, high-yield structure across all topics with interview questions, revision cheat sheets, and hands-on exercises.

---

## 🗺️ System Design Roadmap (24 Chapters)

| # | Chapter | File | Focus Areas | Status |
| :-: | :--- | :--- | :--- | :-: |
| **01** | **System Design Basics** | [`01.Basics.md`](01.Basics.md) | Scaling, Latency/Throughput, Networking, DNS, Proxies, ACID/BASE | ✅ Complete |
| **02** | **Load Balancing** | [`02.LoadBalancing.md`](02.LoadBalancing.md) | L4 vs L7, Algorithms (P2C, Smooth WRR), Health Checks, Consistent Hashing, Sharding, AI Load Balancing | ✅ Complete |
| **03** | **Data Stores** | [`03.DataStores.md`](03.DataStores.md) | Storage Engines (Pages/Extents/Heaps), B+ Trees, LSM/SSTables, WAL, MVCC, Relational/NoSQL, Consensus, CDC | 🟡 In Progress |
| **04** | **Consistency vs Availability** | `04.Consistency_vs_Availability.md` | CAP Theorem, PACELC, Linearizability, Eventual Consistency, Quorums | ⏳ Planned |
| **05** | **Message Queues** | `05.MessageQueues.md` | Kafka, RabbitMQ, SQS, Pull vs Push, Partitioning, Exactly-Once Semantics | ⏳ Planned |
| **06** | **DevOps Concepts** | `06.DevOpsConcepts.md` | CI/CD, Containerization, Kubernetes, Infrastructure as Code, GitOps | ⏳ Planned |
| **07** | **Caching** | `07.Caching.md` | Cache Strategies (Read-Through, Write-Behind), Eviction (LRU, LFU, ARC), Stampede Prevention | ⏳ Planned |
| **08** | **Microservices** | `08.Microservices.md` | Service Boundaries, Decomposition, Saga Pattern, Distributed Tracing | ⏳ Planned |
| **09** | **API Gateways** | `09.APIGateways.md` | Reverse Proxies, Authentication, Aggregation, Rate Limiting, Kong, Envoy | ⏳ Planned |
| **10** | **Authentication Mechanisms** | `10.AuthenticationMechanisms.md` | OAuth 2.0, OpenID Connect, JWT, Session Stores, mTLS, RBAC/ABAC | ⏳ Planned |
| **11** | **System Design Trade-offs** | `11.Tradeoffs.md` | Throughput vs Latency, Memory vs CPU, Normalization vs Denormalization | ⏳ Planned |
| **12** | **Practice Problems (Core)** | `12.PracticeProblemsCore.md` | URL Shortener, Rate Limiter, Notification Service, Key-Value Store | ⏳ Planned |
| **13** | **Networking Fundamentals** | `13.NetworkingFundamentals.md` | TCP/UDP, HTTP/1.1 vs HTTP/2 vs HTTP/3 (QUIC), TLS Handshake, WebSockets, gRPC | ⏳ Planned |
| **14** | **Database Indexing & Query Tuning** | `14.DatabaseIndexing.md` | Clustered/Secondary Indexes, Covering Indexes, EXPLAIN Plans, Index Bloat | ⏳ Planned |
| **15** | **API Design Patterns** | `15.APIDesignPatterns.md` | REST, GraphQL, gRPC, RPC, Webhooks, SSE, Idempotency Keys | ⏳ Planned |
| **16** | **Security in Distributed Systems** | `16.SecurityDistributedSystems.md` | Zero Trust, Encryption at Rest/Transit, DDoS Defense, Secret Management | ⏳ Planned |
| **17** | **Monitoring, Logging & Observability**| `17.MonitoringLoggingObservability.md` | OpenTelemetry, Prometheus, Distributed Tracing, RED vs USE Metrics, Log Aggregation | ⏳ Planned |
| **18** | **Rate Limiting & Throttling** | `18.RateLimitingThrottling.md` | Token Bucket, Leaky Bucket, Fixed/Sliding Window, Distributed Redis Limiters | ⏳ Planned |
| **19** | **Event-Driven Architecture** | `19.EventDrivenArchitecture.md` | Event Sourcing, CQRS, Stream Processing (Flink), Idempotency, Dead Letter Queues | ⏳ Planned |
| **20** | **Search Systems Design** | `20.SearchSystemsDesign.md` | Elasticsearch, Inverted Indexes, Tokenization, BM25, Distributed Shard Routing | ⏳ Planned |
| **21** | **Real-Time Systems** | `21.RealTimeSystems.md` | Chat Systems, Live Dashboards, Collaborative Editors (OT & CRDTs), WebRTC | ⏳ Planned |
| **22** | **Deployment Strategies** | `22.DeploymentStrategies.md` | Blue/Green, Canary, Rolling Deployments, Feature Flags, Zero-Downtime DB Migrations | ⏳ Planned |
| **23** | **Cost Estimation & Optimization** | `23.CostEstimationOptimization.md` | Bandwidth, Cloud Storage Tiers, Spot Instances, Egress Costs, FinOps Best Practices | ⏳ Planned |
| **24** | **Advanced Practice Problems** | `24.AdvancedPracticeProblems.md` | Uber/Ride-Hailing, Video Streaming (YouTube/Netflix), WhatsApp, Distributed File System | ⏳ Planned |

---

## 🏛️ The Standardized Topic Blueprint

To maintain consistency and rigorous quality, every topic across all chapters adheres to a standardized **13-part framework**:

```text
┌────────────────────────────────────────────────────────────────────────┐
│                      STANDARDIZED TOPIC BLUEPRINT                      │
├────────────────────────────────────────────────────────────────────────┤
│ 1.  ## Intuition First (The Why)      -> Foundational motivation       │
│ 2.  ## Detailed Explanation           -> Technical internals & theory  │
│ 3.  ## Mental Model and Analogy       -> Intuitive real-world anchors  │
│ 4.  ## ASCII Diagrams                 -> Topology & byte-level layouts │
│ 5.  ## Real-World Examples            -> Production post-mortems       │
│ 6.  ## Internal Working               -> Hidden mechanics & edge cases │
│ 7.  ## Advantages, Disadvantages      -> Trade-off evaluation matrix   │
│ 8.  ## Common Misconceptions          -> Anti-patterns & debunked myths│
│ 9.  ## Interview Questions            -> High-yield Staff-level Q&A   │
│ 10. ## Industry Implementation        -> Tooling (Envoy, K8s, PG, etc) │
│ 11. ## AI/ML System Design            -> GPU, KV-cache & ML pipelines  │
│ 12. ## Revision Sheet                 -> High-speed interview recap    │
│ 13. ## Mini Exercise                  -> Real-world scenario puzzles   │
└────────────────────────────────────────────────────────────────────────┘
```

---

## 🚀 How to Use These Notes

1. **For System Design Interview Prep:**
   - Review **`Intuition First`** and **`Mental Model`** to quickly build clear verbal communication models.
   - Memorize the comparison tables in **`Advantages, Disadvantages, and Trade-offs`** to frame design options dynamically.
   - Study **`Interview Questions`** and review **`Revision Sheet`** 24 hours before your technical loop.
2. **For Day-to-Day Production Engineering:**
   - Refer to **`Internal Working: Mechanics Worth Knowing`** when debugging latency spikes, connection timeouts, or database replication lag.
   - Use the **`ASCII Diagrams`** as starting points for architectural RFCs and engineering design reviews.

---

## 📑 Quick Navigation

- 📌 **Master Index:** [`00.Index.md`](00.Index.md)
- 📗 **Chapter 1: Basics:** [`01.Basics.md`](01.Basics.md)
- 📘 **Chapter 2: Load Balancing:** [`02.LoadBalancing.md`](02.LoadBalancing.md)
- 📙 **Chapter 3: Data Stores:** [`03.DataStores.md`](03.DataStores.md)

