# Engineering Case Studies Portfolio

A curated collection of production case studies detailing software architecture, systems engineering, and problem-solving across diverse engineering domains.

Every case study is fully anonymized to maintain institutional and proprietary confidentiality, focusing exclusively on verifiable engineering achievements, architectural decisions, and concrete technical solutions.

---

## Navigation by Engineering Track

```
case-studies/
├── backend-and-distributed-systems/   # Tracing, Microservices, Hexagonal IAM & State Machines
├── mobile-engineering/                 # React Native, Expo, Accessible UI & Privacy Gates
├── frontend-and-web-apps/              # Next.js 15, Multi-Tenant Portals & Layered Web Apps
├── 3d-graphics-and-simulation/         # Three.js, Rapier 3D (Wasm), Quaternions & WebSockets
├── data-engineering-and-privacy/       # PII Sanitization, Streaming CSV Ingestion & Indexing
├── fullstack-and-monorepos/            # Monorepos (npm workspaces), DAG Graphs & Canvas Queues
└── embedded-systems-and-iot/           # ESP32 C++, MQTT Brokers & SSE Real-Time Streaming
```

---

### 1. [Backend & Distributed Systems](backend-and-distributed-systems/README.md)
* **[High-Throughput Node.js Distributed Tracing & Structured Logging Library](backend-and-distributed-systems/distributed-observability-lib/README.md)**  
  *Stack:* TypeScript · Node.js · Pino · Axios · AsyncLocalStorage  
  *Highlights:* Zero-dependency core library for propagating correlation contexts across microservices, selective health-check log filtering, and error telemetry.

* **[Fault-Tolerant Unstructured Document Ingestion Pipeline & Hardened API Gateway](backend-and-distributed-systems/fault-tolerant-ingestion-gateway/README.md)**  
  *Stack:* Python 3 · PyPDF · Node.js · Express · Docker Compose · Nginx · MongoDB  
  *Highlights:* Robust PDF tabular extraction with 31 regression test suites, automated supervisor orchestrating isolated worker daemons, and security-hardened API gateway.

* **[Hexagonal Architecture Identity & Access Management Microservice](backend-and-distributed-systems/hexagonal-auth-service/README.md)**  
  *Stack:* TypeScript · Node.js · Clean Architecture (Ports & Adapters) · PostgreSQL · JWT  
  *Highlights:* Strict domain/infrastructure boundary separation, concurrent session rotation, token revocation guards, and mutation testing of group authorization policies.

* **[Concurrency-Safe Editorial Workflow Engine with Formal State Machines](backend-and-distributed-systems/concurrency-safe-editorial-engine/README.md)**  
  *Stack:* TypeScript · Node.js · Express · PostgreSQL (`READ COMMITTED`) · State Machine  
  *Highlights:* Formal editorial state machine, mutation-tested transition guards, versioned article submissions, and optimistic concurrency locks.

---

### 2. [Mobile Engineering](mobile-engineering/README.md)
* **[Real-Time Fleet Transit Navigation & Privacy-Preserving Mobile Application](mobile-engineering/campus-mobility-transit-app/README.md)**  
  *Stack:* React Native · Expo · TypeScript · NativeWind · Android Exact Alarms · Jest  
  *Highlights:* Single-stroke transit timeline with animated pulsating origin respecting user accessibility (`reduce motion`), strict regulatory privacy consent barrier, and exact alarm scheduling.

---

### 3. [Frontend & Web Applications](frontend-and-web-apps/README.md)
* **[Multi-Tenant Enterprise Operations Portal with Client-to-Server Error Tracing](frontend-and-web-apps/enterprise-operations-admin-portal/README.md)**  
  *Stack:* Next.js · React · TypeScript · Tailwind CSS · Playwright · Pino  
  *Highlights:* Department-scoped role authorization, drag-and-drop banner sequencing, client-side error boundaries piped directly into server structured logs, and automated container redeployment webhooks.

* **[Strict Layered Architecture Inventory Management & Revenue Platform](frontend-and-web-apps/retail-inventory-analytics-platform/README.md)**  
  *Stack:* Next.js 15 (App Router) · React 19 · TypeScript · Prisma ORM · SQLite / Turso libSQL  
  *Highlights:* Strict four-tier layered architecture (UI → Route Handlers → Domain Services → Prisma), dual-mode SQLite/Turso database switching, and mobile-first inventory analytics.

* **[Full-Stack Community Welfare & Adoption Management System](frontend-and-web-apps/community-welfare-adoption-platform/README.md)**  
  *Stack:* React · Node.js · Express · MongoDB · Docker · Nginx · GitHub Actions  
  *Highlights:* Micro-scale full-stack architecture, configurable multi-origin CORS, role-based review workflows, and containerized cloud deployment.

---

### 4. [3D Graphics, WebGL & Simulation](3d-graphics-and-simulation/README.md)
* **[First-Person 3D WebGL Clinical Laboratory & Physics Simulation](3d-graphics-and-simulation/clinical-lab-webgl-physics-simulation/README.md)**  
  *Stack:* Three.js · React Three Fiber · Rapier 3D (Wasm) · TypeScript · Vite · Playwright E2E  
  *Highlights:* First-person 3D physics interaction, 1:1 camera-aligned quaternion object inspection without gimbal lock or drift, depth-of-field bokeh blur, and centrifuge/incubator finite-state machines.

* **[Multi-User Real-Time Simulation Engine & Space Flight Telemetry](3d-graphics-and-simulation/multiplayer-space-flight-simulation/README.md)**  
  *Stack:* React 19 · TypeScript · Vite · Three.js · Socket.IO · Neon PostgreSQL · Drizzle ORM  
  *Highlights:* Multi-user cooperative planetary outpost survival simulation, interactive launch scene, real-time radiation shielding telemetry calibrated against actual space radiation data.

* **[Zero-Asset Procedural 2D Isometric Healthcare Training Simulation](3d-graphics-and-simulation/procedural-2d-isometric-health-sim/README.md)**  
  *Stack:* JavaScript · React · HTML5 Canvas 2D · Web Audio API  
  *Highlights:* Completely procedural 2D isometric rendering without external image assets, real-time Web Audio API music synthesis, and healthcare community territory navigation.

---

### 5. [Data Engineering & Privacy](data-engineering-and-privacy/README.md)
* **[Scalable Clinical Record Ingestion & PII Sanitization Architecture](data-engineering-and-privacy/clinical-record-pii-sanitization/README.md)**  
  *Stack:* Python · Flask · PostgreSQL · Docker · Nginx  
  *Highlights:* High-stakes patient PII sanitization (eliminating citizen tax IDs from URLs, query strings, and logs), O(1) memory streaming CSV reader for tens of thousands of citizen records, and risk stratification algorithms.

---

### 6. [Full-Stack & Monorepos](fullstack-and-monorepos/README.md)
* **[Interactive Degree Curriculum Graph Engine & Collaborative Whiteboard](fullstack-and-monorepos/academic-curriculum-dag-whiteboard/README.md)**  
  *Stack:* TypeScript · Node.js · Express · React 19 · Vite · Prisma · PostgreSQL · MinIO · Docker · Zod  
  *Highlights:* Monorepo architecture, idempotent analytics event ingestion, real-time concurrency control in digital whiteboard canvas, and graph memoization for degree curriculum flowcharts.

---

### 7. [Embedded Systems & IoT](embedded-systems-and-iot/README.md)
* **[Real-Time Environmental Telemetry Firmware & Event-Driven Dashboard](embedded-systems-and-iot/real-time-air-quality-iot-telemetry/README.md)**  
  *Stack:* C++ · ESP32 · Eclipse Mosquitto MQTT · Node.js · Express · EJS · Server-Sent Events (SSE)  
  *Highlights:* Embedded firmware sampling gas and particulate sensors at 1 Hz with 30s telemetry dispatch, paired with an SSR Node.js dashboard streaming updates via SSE.
