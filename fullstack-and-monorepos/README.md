# Full-Stack & Monorepos Case Studies

This category presents large-scale web platforms architected as TypeScript monorepos, focusing on shared type contracts, reactive directed acyclic graphs (DAGs), collaborative whiteboard canvas engines, and idempotent analytics pipelines.

---

## Case Studies in this Track

### 1. [Interactive Degree Curriculum Graph Engine & Collaborative Whiteboard](academic-curriculum-dag-whiteboard/README.md)
* **Core Themes:** TypeScript Monorepos (npm workspaces), Directed Acyclic Graphs, Collaborative Whiteboard Persistence, Idempotent Event Ingestion.
* **Key Challenges:**
  - Designing a single-writer write-behind queue for a digital canvas to decouple 60 FPS drawing strokes from asynchronous database persistence.
  - Optimizing interactive curriculum dependency graphs by profiling React render trees, memoizing expensive subtrees, and flattening heavy CSS glow filters on mobile GPUs.
  - Building an idempotent analytics ingestion service enforcing consistent transactional locks and cohort retention reporting.
* **Technologies:** TypeScript, Node.js, Express, React 19, Vite, Prisma ORM, PostgreSQL, MinIO (S3), Docker, Zod.
