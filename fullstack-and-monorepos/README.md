# Estudos de Caso em Full-Stack e Monorepos

Esta categoria apresenta plataformas web de grande porte estruturadas como monorepos TypeScript, com foco em contratos tipados compartilhados, grafos acíclicos dirigidos (DAGs), mecanismos de tela digital colaborativa e ingestão de eventos analíticos com idempotência.

---

## Estudos de Caso nesta Trilha

### 1. [Motor Gráfico de Matrizes Curriculares e Quadro Branco Colaborativo](academic-curriculum-dag-whiteboard/README.md)
* **Temas Centrais:** Monorepos TypeScript (npm workspaces), Grafos Acíclicos Dirigidos, Persistência de Quadro Branco Colaborativo, Ingestão Idempotente de Eventos.
* **Principais Desafios:**
  - Criação de fila write-behind com escritor único para desacoplar o desenho a 60 FPS da persistência no banco de dados.
  - Otimização do grafo de pré-requisitos curriculares corrigindo árvores de memoização no React e simplificando filtros CSS pesados em dispositivos móveis.
  - Construção de serviço de ingestão idempotente de telemetria com travas transacionais e agregação de retenção por coortes.
* **Tecnologias:** TypeScript, Node.js, Express, React 19, Vite, Prisma ORM, PostgreSQL, MinIO (S3), Docker, Zod.
