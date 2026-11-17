# Frontend & Web Applications Case Studies

This category showcases web application architectures built with React, Next.js, and TypeScript, focusing on client-to-server error observability, multi-tenant role-based administration, strict layered architectures, and mobile-first analytics.

---

## Case Studies in this Track

### 1. [Multi-Tenant Enterprise Operations Portal with Client-to-Server Error Tracing](enterprise-operations-admin-portal/README.md)
* **Core Themes:** Next.js, Client Observability, Department Scoped RBAC, Layout Shift Optimization.
* **Key Challenges:** Connecting client React error boundaries directly to structured server logs with incoming reverse-proxy correlation IDs, and eliminating layout shift (CLS) using custom-fitted skeleton screens.
* **Technologies:** Next.js (App Router), React, TypeScript, Tailwind CSS, Playwright, Pino.

### 2. [Strict Layered Architecture Inventory Management & Revenue Platform](retail-inventory-analytics-platform/README.md)
* **Core Themes:** Clean Layered Architecture, Decoupled Domain Services, Dual-Mode Database Connectivity.
* **Key Challenges:** Enforcing strict separation across four tiers (UI → Route Handlers → Services → Prisma) and establishing a runtime database factory supporting local SQLite and edge libSQL without code changes.
* **Technologies:** Next.js 15 (App Router), React 19, TypeScript, Prisma ORM, SQLite / Turso libSQL.

### 3. [Full-Stack Community Welfare & Adoption Management System](community-welfare-adoption-platform/README.md)
* **Core Themes:** Full-Stack Architecture, Configurable Multi-Origin CORS, Containerized Cloud Deployments.
* **Key Challenges:** Handling dynamic CORS origins across preview and production environments and managing persistent media volumes with Nginx caching on Linux VPS hosts.
* **Technologies:** React, Node.js, Express, MongoDB, Mongoose, Docker, Nginx, GitHub Actions.
