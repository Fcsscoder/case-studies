# Backend & Distributed Systems Case Studies

This category groups engineering case studies focused on distributed tracing, telemetry propagation, high-reliability document ingestion, clean hexagonal microservice architectures, and concurrency-safe transactional state machines.

---

## Case Studies in this Track

### 1. [High-Throughput Node.js Distributed Tracing & Structured Logging Library](distributed-observability-lib/README.md)
* **Core Themes:** Distributed Systems, Telemetry, Node.js AsyncLocalStorage, HTTP Context Propagation.
* **Key Challenges:** Preserving correlation IDs across asynchronous event loops and muting high-frequency container health check probes without dropping failure diagnostics.
* **Technologies:** TypeScript, Node.js, Pino, Axios Interceptors, Express Middleware.

### 2. [Fault-Tolerant Unstructured Document Ingestion Pipeline & Hardened API Gateway](fault-tolerant-ingestion-gateway/README.md)
* **Core Themes:** Automated Ingestion, PDF Data Extraction, Fail-Fast Supervisor, Nginx Gateway Hardening.
* **Key Challenges:** Parsing complex multi-column tabular PDFs with 31 regression test suites and preventing automated sync runs from overwriting manual administrative overrides via ownership fencing.
* **Technologies:** Python 3, PyPDF, Docker Compose, Nginx, MongoDB.

### 3. [Hexagonal Architecture Identity & Access Management Microservice](hexagonal-auth-service/README.md)
* **Core Themes:** Clean Architecture, Ports & Adapters, Cryptographic Token Security, Mutation Testing.
* **Key Challenges:** Preventing false-positive session revocation during parallel AJAX refresh token handshakes and mathematically verifying multi-tenant authorization policies via mutation testing.
* **Technologies:** TypeScript, Node.js, Express, PostgreSQL, JWT, Jest, Stryker patterns.

### 4. [Concurrency-Safe Editorial Workflow Engine with Formal State Machines](concurrency-safe-editorial-engine/README.md)
* **Core Themes:** Finite-State Machines (FSM), Database Concurrency, Transactional Locking.
* **Key Challenges:** Eliminating race conditions during simultaneous multi-party review approvals using PostgreSQL row-level locks under `READ COMMITTED` isolation.
* **Technologies:** TypeScript, Node.js, Express, PostgreSQL (`SELECT FOR UPDATE`), Finite-State Machine Pattern.
