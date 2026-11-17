# Data Engineering & Privacy Case Studies

This category focuses on high-throughput data processing, memory-efficient streaming pipelines, and regulatory data privacy engineering (PII sanitization) in healthcare systems.

---

## Case Studies in this Track

### 1. [Scalable Clinical Record Ingestion & PII Sanitization Architecture](clinical-record-pii-sanitization/README.md)
* **Core Themes:** Data Privacy (LGPD), High-Stakes PII Sanitization, Streaming Ingestion, PostgreSQL Optimization.
* **Key Challenges:**
  - Eliminating national citizen tax IDs and clinical search queries from HTTP URL paths, query parameters, and reverse-proxy access logs.
  - Designing a generator-based streaming CSV ingestion pipeline operating within a strictly bounded $O(1)$ memory footprint, eliminating server out-of-memory crashes on massive municipal datasets.
  - Introducing normalized indexing schemes and composite database indexes to optimize epidemiological risk stratification calculations.
* **Technologies:** Python, Flask, PostgreSQL, Gunicorn, Docker Compose, ReportLab (PDF), OpenAPI.
